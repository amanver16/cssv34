# 🛠 SourceMod Plugins

This directory contains plugin packs and modules for [SourceMod](../Sourcemod/README.md). These plugins add gameplay features, utility commands, HUD elements, announcements, rewards, and other server behavior changes.

## 📥 How To Install

1. Copy the plugin files into the matching directories inside `cstrike`.
2. Keep the original folder layout when the package includes `addons`, `cfg`, `translations`, or `configs`.
3. Restart the server.
4. Verify the plugin loads with:

```text
sm plugins list
```

## 🗂 Typical Plugin Layout

```text
cstrike/
├── addons/
│   └── sourcemod/
│       ├── configs/
│       ├── data/
│       ├── plugins/
│       │   └── plugin-name.smx
│       ├── scripting/
│       │   └── plugin-name.sp
│       └── translations/
│           └── plugin-name.phrases.txt
└── cfg/
	└── sourcemod/
		└── plugin-name.cfg
```

## 📦 Included Plugin Groups

This repository includes SourceMod plugin content such as:

- `ClientMod`
- `Advertisements`
- `Allow Old`
- `Connect Announce`
- `Death Notice`
- `Enter Sounds`
- `Game Connected`
- `HUD Example`
- `IGN`
- `Menu`
- `Pickup Weapon`
- `Rewards`
- `Share`
- `Show Damage`
- `Tags`

Each plugin package may include a different combination of `.smx`, `.sp`, config, translation, or data files.