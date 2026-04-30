# 🎮 Counter-Strike: Source v34 Dedicated Server

This repository collects clean server files, plugin packages, extensions, and setup notes for running a Counter-Strike: Source v34 dedicated server on Windows or Linux.

## 📦 What This Repository Contains

- **Clean Server Files**: base server files for Windows and Linux.
- **Metamod**: the Metamod:Source package required for Metamod plugins.
- **Sourcemod**: the SourceMod package required for SourceMod plugins and extensions.
- **Metamod Plugins**: optional plugins loaded through Metamod:Source.
- **Sourcemod Extensions**: optional native extensions for SourceMod.
- **Sourcemod Plugins**: gameplay and utility plugins for your server.
- **Useful Guides**: extra reference material.

## 🧭 Recommended Setup Order

Follow the documentation in this order:

1. [Linux clean server files](Clean%20Server%20Files/Linux/README.md)
2. [Windows clean server files](Clean%20Server%20Files/Windows/README.md)
3. [Metamod:Source](Metamod/README.md)
4. [SourceMod](Sourcemod/README.md)
5. [Metamod plugins](Metamod%20Plugins/README.md)
6. [SourceMod extensions](Sourcemod%20Extensions/README.md)
7. [SourceMod plugins](Sourcemod%20Plugins/README.md)

## 🗂 Repository Map

| Path | Description |
| --- | --- |
| [Clean Server Files](Clean%20Server%20Files) | Base dedicated server files for both supported operating systems. |
| [Metamod](Metamod) | Metamod:Source package and install notes. |
| [Metamod Plugins](Metamod%20Plugins) | Optional Metamod plugins such as BufferFix and Stripper. |
| [Sourcemod](Sourcemod) | SourceMod package and install notes. |
| [Sourcemod Extensions](Sourcemod%20Extensions) | Native SourceMod extensions. |
| [Sourcemod Plugins](Sourcemod%20Plugins) | Optional SourceMod plugin packs and modules. |
| [Useful Guides](Useful%20Guides) | Additional setup or maintenance references. |

## ⚠️ Notes

- Most packages in this repository are distributed as archives and should be extracted into the correct server folders.
- Read the README in each directory before copying files into your server.
- Always restart the server after installing or updating Metamod, SourceMod, plugins, or extensions.

## ✅ Quick Start

If you are setting up a fresh server:

1. Install the clean server files for your operating system.
2. Install [Metamod:Source](Metamod/README.md).
3. Install [SourceMod](Sourcemod/README.md).
4. Add the plugins and extensions you actually need.
5. Start the server and verify each component from the server console.