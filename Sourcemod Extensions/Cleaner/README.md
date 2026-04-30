# 🧼 Cleaner

Cleaner is a SourceMod extension that reduces console noise by filtering unnecessary output. It is useful when you want a more readable server console during normal operation.

## 📥 Installation

1. Extract and copy the `addons` folder into your `cstrike` directory.
2. Add the following line to the bottom of `addons/sourcemod/configs/core.cfg`:

```text
"Cleaner"        "on"
```

3. Restart the server.

## ✅ Verification

Run the following command in the server console:

```text
sm exts list
```

Confirm that the extension is loaded and that console output is cleaner after restart.