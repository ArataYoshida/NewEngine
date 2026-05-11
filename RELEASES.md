# Release Operation

## 日本語

このリポジトリは GitHub Releases に成果物だけを置くための配布用リポジトリです。
ソースコード、ビルドログ、検証画像、ローカル設定、認証情報はコミットしません。

GameEngine 開発リポジトリ側で以下を実行します。

```powershell
.\build_all.bat
powershell -NoProfile -ExecutionPolicy Bypass -File .\tools\package-release.ps1 -Version <version>
$env:GITHUB_TOKEN = "<repo 権限を持つ token>"
powershell -NoProfile -ExecutionPolicy Bypass -File .\tools\publish-release.ps1 -Version <version>
```

## English

This is a release-only repository. GitHub Releases should contain the distributable artifacts only.
Do not commit source code, build logs, verification screenshots, local settings, or credentials.

Run the following from the private GameEngine development repository.

```powershell
.\build_all.bat
powershell -NoProfile -ExecutionPolicy Bypass -File .\tools\package-release.ps1 -Version <version>
$env:GITHUB_TOKEN = "<token with repository permissions>"
powershell -NoProfile -ExecutionPolicy Bypass -File .\tools\publish-release.ps1 -Version <version>
```
