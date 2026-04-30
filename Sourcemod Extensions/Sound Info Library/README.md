# 🔊 Sound Info Library

Sound Info Library is a SourceMod extension that improves sound metadata handling. It helps calculate sound lengths correctly and can read additional information from sound files that include ID3 metadata.

## ⚠️ Note

VBR-encoded MP3 files may still report inaccurate durations in some cases.

## 📥 Installation

1. Extract and copy the `addons` folder into your `cstrike` directory.
2. Restart the server.

## ✅ Verification

Run the following command in the server console:

```text
sm exts list
```

Confirm that `Sound Info Library` appears in the loaded extensions list.