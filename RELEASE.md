# WorldShot Log Release Procedure

## Release Steps

1. Update `package.json` `version`.
2. Verify app behavior.
3. Commit to `main` and push.
4. Create Windows distribution artifacts.

```bash
npm run make:win
```

5. Create a git tag matching the version.
6. Create a GitHub Release with the same tag name.
7. Attach files from `out/make/squirrel.windows/x64/`:

- `WorldShotLogSetup.exe`
- `worldshot-log-<version>-full.nupkg`
- `RELEASES`

8. Publish the release. Draft releases are not used for automatic updates.

## Automatic Update Requirements

- The app `version` must be greater than the currently published version.
- The GitHub Release tag must match the app version, for example `v1.0.1`.
- `RELEASES` and the `.nupkg` file are required.
- Automatic updates only work in the distributed Windows app.
- Automatic updates do not run during development (`npm start`).

## Current Naming Rules

- App name: `WorldShot Log`
- Tag format: `v<version>`
- Windows installer name: `WorldShotLogSetup.exe`
