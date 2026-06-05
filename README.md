# WorldShot Log

WorldShot Log is a Windows desktop app for organizing, reviewing, and preparing VRChat photos.

It supports date and world-based photo management, image adjustments, cropping, privacy masking, and text overlays. Original images are not overwritten; edited images are saved separately.

> WorldShot Log is not an official VRChat Inc. application.

## Features

- Drag and drop import for VRChat photos and folders
- Browse photos by year, month, date, and world
- Filter by favorites, orientation, label, and world name
- Open photo details, original images, containing folders, and VRChat pages when available
- Manage favorites, labels, memos, world names, and World URLs
- Fetch and reuse world metadata after import
- Edit images in-app without overwriting originals
- Adjust light, color, tone curves, blur, privacy masks, crop, rotation, and text overlays
- Save built-in and custom presets
- Back up, restore, export CSV / JSON, regenerate thumbnails, and run data health checks

## Download

Download the latest version from GitHub Releases.

- [Releases](https://github.com/noma-nomoa/vrchat-world-photo-manager/releases)
- [v2.0.0 release notes](./release-notes/v2.0.0.md)

The Windows installer is `WorldShotLogSetup.exe`.

## Install

1. Download the latest `WorldShotLogSetup.exe` from GitHub Releases.
2. Run `WorldShotLogSetup.exe`.
3. WorldShot Log launches after installation completes.

## Development

```bash
npm install
npm start
```

### Windows build

```bash
npm run make:win
```

Build artifacts are written to `out/make/squirrel.windows/x64/`.

## Data Locations

- DB / settings: `C:\Users\<UserName>\AppData\Roaming\WorldShot Log\data\`
- Thumbnails: `C:\Users\<UserName>\WorldShot Log\thumbnails`

## License

WorldShot Log is released under the MIT License. See [LICENSE](./LICENSE) for details.
