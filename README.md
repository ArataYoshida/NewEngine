# NewEngine

## 日本語

NewEngine は、ゲーム制作を始めるための Editor、ランタイム、プロジェクト管理ツールをまとめた Windows 向けゲームエンジンです。NewLauncher から目的のバージョンを選び、インストール後すぐにプロジェクト作成と Editor 起動ができます。

### 主な機能

- シーン編集: Hierarchy、Inspector、Viewport を使ったオブジェクト配置と編集
- コンポーネント編集: Transform、Mesh、Material、回転や入力などの挙動を Editor から調整
- アセット管理: Project View で素材を管理し、モデル、マテリアル、シェーダー、スクリプトを扱うワークフロー
- C# スクリプト: プロジェクト内のスクリプトをコンパイルし、Editor から実行やホットリロードを行う制作サイクル
- NativeAOT 対応: スクリプトを高速なネイティブ実行向けにビルドするワークフロー
- Direct3D ベースの描画: 標準シェーダー、マテリアル、メッシュ表示、ボクセル描画系の基盤
- ROM ビルド: プロジェクトをランタイム実行用パッケージとして出力する機能
- テンプレート: 新規プロジェクト作成時に基本アセットとサンプル挙動を自動配置
- 多言語 UI: 日本語と英語の表示に対応
- バージョン管理: NewLauncher から最新版や過去バージョンを選択してインストール

### 使い方

1. NewLauncher を起動します。
2. `リリース確認` で利用可能な NewEngine バージョンを取得します。
3. 使いたいバージョンを選んで `インストール` を押します。
4. 新規プロジェクトを作成するか、既存プロジェクトを追加します。
5. 使用するエンジンを選び、`プロジェクトを起動` で NewEditor を開きます。

### リリース内容

各リリースには Launcher が読み取る manifest と、Editor / Engine / Runtime を含む Windows x64 パッケージが添付されます。

- `engine-manifest.json`
- `NewGameEngine-<version>-win-x64.zip`

### ライセンス概要

未改造の公式バイナリは商用プロジェクトにも使用できます。
ただし、バイナリの改造、リバースエンジニアリング、再配布は禁止です。
詳細は `LICENSE` を確認してください。

## English

NewEngine is a Windows game engine that bundles an Editor, runtime, and project workflow for building games. NewLauncher lets you choose a version, install it, create a project, and open the Editor quickly.

### Highlights

- Scene editing: place and edit objects through Hierarchy, Inspector, and Viewport workflows
- Component editing: tune Transform, Mesh, Material, rotation, input, and behavior settings from the Editor
- Asset management: manage models, materials, shaders, scripts, and project files in the Project View
- C# scripting: compile project scripts and iterate through Editor-driven run and hot-reload workflows
- NativeAOT workflow: build scripts for fast native execution paths
- Direct3D rendering foundation: standard shaders, materials, mesh rendering, and voxel rendering support
- ROM build flow: package projects for standalone runtime execution
- Project templates: create new projects with default assets and sample behaviors
- Bilingual UI: Japanese and English display support
- Version management: install the latest or older NewEngine versions through NewLauncher

### Getting Started

1. Start NewLauncher.
2. Use `Check Releases` to load available NewEngine versions.
3. Choose a version and press `Install`.
4. Create a new project or add an existing one.
5. Select the engine version and launch the project in NewEditor.

### Release Contents

Each release provides a manifest for NewLauncher and a Windows x64 package containing the Editor, Engine, and runtime files.

- `engine-manifest.json`
- `NewGameEngine-<version>-win-x64.zip`

### License Summary

You may use the unmodified official binaries for commercial projects.
Modification, reverse engineering, and redistribution of the binaries are not allowed.
See `LICENSE` for the full terms.
