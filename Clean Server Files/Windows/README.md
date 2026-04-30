# 🪟 Windows Dedicated Server Files

Use this package to deploy a clean Counter-Strike: Source v34 dedicated server on Windows.

## ⬇️ Download

[Download the Windows server files](https://drive.google.com/file/d/1O-I1M3ilEdbF-7iIr_YTc4-14cVBhoPv/view?usp=drive_link)

## 🧾 Server Version

| Item | Value |
| --- | --- |
| Protocol version | 7 |
| Exe version | 1.0.0.34 (cstrike) |
| Exe build | 17:27:58 Dec 3 2009 (4044) |

## 📥 Installation

1. Download the archive from the link above.
2. Upload the files to your Windows server using Remote Desktop, shared storage, or your preferred transfer method.
3. Extract the files into the directory where you want to run the server.
4. Confirm that all files were extracted correctly before starting the server.

## ▶️ Running the Server

Start the server by running:

```bat
start.bat
```

This launches the dedicated server in a Command Prompt window.

### Useful Notes

- Watch the console output to confirm the server starts correctly.
- The console will show server activity, connected players, and the bound IP and port.
- Stop the server by closing the Command Prompt window or pressing `Ctrl + C`.
- Adjust startup arguments by editing `start.bat` if you need to change the map, player count, or other launch options.

## 🌐 Port Forwarding

Allow inbound traffic for the default game port:

```text
UDP 27015
```

If you are hosting behind Windows Firewall or a provider firewall, make sure this port is open and forwarded to the server.

## ✅ Next Step

After the base server is running, continue with [Metamod:Source](../../Metamod/README.md) and then [SourceMod](../../Sourcemod/README.md).

