# 🧩 SourceMod Extensions

This directory contains native extensions for [SourceMod](../Sourcemod/README.md). Extensions expand SourceMod with additional engine hooks, helper libraries, or native functionality that some plugins depend on.

## 📥 How To Install

1. Extract the extension files into the correct folders on your server.
2. Restart the server.
3. Verify that the extension loaded successfully with:

```text
sm exts list
```

## 📦 Available Extensions

| Extension | Description |
| --- | --- |
| [Cleaner](Cleaner/README.md) | Filters noisy console output. |
| [ConsoleHook](ConsoleHook/README.md) | Adds console-print support used by some plugins. |
| [Host Manager](Host%20Manager/README.md) | Hides player SteamIDs from the host output. |
| [Sound Info Library](Sound%20Info%20Library/README.md) | Improves sound metadata and duration handling. |

## ⚠️ Note

Some SourceMod plugins require specific extensions to be installed first. Always read the plugin documentation before deployment.