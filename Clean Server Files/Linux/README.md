# 🐧 Linux Dedicated Server Files

Use this package to deploy a clean Counter-Strike: Source v34 dedicated server on Linux.

## ⬇️ Download

[Download the Linux server files](https://drive.google.com/file/d/1yDhqEkXZPdq9Ln_JHXhFD_oUdNta0YUU/view?usp=drive_link)

## 🧾 Server Version

| Item | Value |
| --- | --- |
| Protocol version | 7 |
| Exe version | 1.0.0.34 (cstrike) |
| Exe build | 10:54:47 Jan 28 2010 (4100) |

## 📥 Installation

1. Download the archive from the link above.
2. Upload the files to your Linux server using FTP, SFTP, WinSCP, FileZilla, or another transfer method.
3. Extract the files into the directory where you want to run the server.
4. Confirm that the files were extracted correctly before continuing.

## 🔐 Set Permissions

Make the startup and server binaries executable:

```bash
chmod +x srcds_run srcds_i486 srcds_i686 srcds_amd start.sh stop.sh session.sh
```

## 📚 Install Dependencies

The server requires 32-bit runtime libraries.

### Debian or Ubuntu

```bash
sudo dpkg --add-architecture i386
sudo apt update
sudo apt install libstdc++6:i386 -y
sudo apt install libgcc-s1:i386 -y
sudo apt install zlib1g:i386 -y
sudo apt install lib32gcc-s1 -y
sudo apt install libc6-i386 -y
sudo apt install lib32stdc++6 -y
sudo apt install lib32z1 -y
sudo apt install screen -y
```

### CentOS or RHEL

```bash
sudo yum install glibc.i686 -y
sudo yum install glibc.i386 -y
sudo yum install libstdc++.i686 -y
sudo yum install zlib.i686 -y
sudo yum install libgcc.i686 -y
sudo yum install screen -y
```

`screen` is used to keep the server running after you disconnect from the terminal.

## ▶️ Running the Server

Start the server with:

```bash
sh start.sh
```

Check or re-attach to the running session with:

```bash
sh session.sh
```

In a standard `screen` session you can detach with:

```text
Ctrl + A, then D
```

You can also attach manually with:

```bash
screen -r css
```

Stop the server with:

```bash
sh stop.sh
```

If you need custom launch parameters, edit `start.sh`.

## 🌐 Port Forwarding

Allow the default game port:

```text
UDP 27015
```

Example `iptables` rules:

```bash
sudo iptables -A INPUT -p udp --dport 27015 -j ACCEPT
sudo iptables -A INPUT -p tcp --dport 27015 -j ACCEPT
sudo iptables-save > /etc/iptables/rules.v4
sudo iptables-save > /etc/iptables/rules.v6
```

If you are using a VPS or dedicated host, also confirm the provider firewall allows the same port.

## ✅ Next Step

After the base server is running, continue with [Metamod:Source](../../Metamod/README.md) and then [SourceMod](../../Sourcemod/README.md).