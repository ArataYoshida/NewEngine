# Release Guide

## 日本語

NewEngine のリリースは、NewLauncher が自動検出できる manifest と Windows x64 パッケージで構成されます。

### ファイル

- `engine-manifest.json`: バージョン、チャンネル、SHA256、パッケージ名、対応 Launcher バージョンを記録します。
- `NewGameEngine-<version>-win-x64.zip`: NewEditor、Engine ランタイム、ROM 実行環境、標準テンプレートを含む実行パッケージです。

### 公開手順

```powershell
.\build_all.bat
powershell -NoProfile -ExecutionPolicy Bypass -File .\tools\package-release.ps1 -Version <version>
$env:GITHUB_TOKEN = "<repo token>"
powershell -NoProfile -ExecutionPolicy Bypass -File .\tools\publish-release.ps1 -Version <version>
```

## English

NewEngine releases are made of a manifest that NewLauncher can detect automatically and a Windows x64 package.

### Files

- `engine-manifest.json`: Records version, channel, SHA256, package name, and the required Launcher version.
- `NewGameEngine-<version>-win-x64.zip`: Runtime package containing NewEditor, Engine runtime files, ROM runtime, and default templates.

### Publishing

```powershell
.\build_all.bat
powershell -NoProfile -ExecutionPolicy Bypass -File .\tools\package-release.ps1 -Version <version>
$env:GITHUB_TOKEN = "<repo token>"
powershell -NoProfile -ExecutionPolicy Bypass -File .\tools\publish-release.ps1 -Version <version>
```
