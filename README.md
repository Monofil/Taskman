# Taskman

Taskmanは、個人利用向けのローカル完結型ビジュアルタスク管理デスクトップアプリです。TaskをTimeline、Kanban、WBSで可視化し、Project、依存関係、進捗、期限超過をSQLiteで管理します。

> [!WARNING]
> v0.3.1はAuthenticode未署名です。Microsoft Defender SmartScreenまたはSmart App Controlにより警告・ブロックされる場合があります。Windowsの保護機能を無効化して実行しないでください。

## ダウンロード

- [最新版のRelease](https://github.com/Monofil/Taskman/releases/latest)
- [Windows 11 x64 通常版](https://github.com/Monofil/Taskman/releases/latest/download/Taskman-v0.3.1-windows-x64.zip) — 推奨。NSIS installerとWebView2 offline installerを含みます。
- [Windows 11 x64 standalone版](https://github.com/Monofil/Taskman/releases/latest/download/Taskman-v0.3.1-windows-x64-standalone.zip) — WebView2 Runtime導入済み環境向け。

GitHubが自動表示する`Source code (zip)`は、この配布用リポジトリのREADME等をまとめたものであり、Taskmanアプリ本体ではありません。必ずReleaseの`Assets`から上記の配布ZIPを取得してください。

## v0.3.1の主な変更

- WBSセル編集中の`Enter`／`Escape`後も元のセル選択とfocusを維持
- 優先度と状態をマウスで選択可能
- 優先度と状態は`↑`／`↓`で候補を連続移動し、`Enter`で確定
- 備考編集中は文章全体が見える高さへ入力欄を自動拡張
- SQLite schemaは`0003`のまま。v0.3.0のProject、Task、設定、担当者データを保持して更新

## 対応環境

- Windows 11 x64
- 1 GB以上の空き容量を推奨
- 自動更新なし

通常版は現在のWindowsユーザーへインストールされ、WebView2未導入時は同梱のオフラインinstallerから導入します。standalone版はZIPを展開し、`Taskman.exe`を直接実行します。

## データ保存

Task、Project、Settings等は端末内の次の場所に保存されます。Taskman自身によるクラウド同期はありません。

```text
%APPDATA%\app.taskman.desktop
```

利用前とversion変更前に、このフォルダーをバックアップしてください。

## 署名とハッシュ

v0.3.1は未署名です。Release notesと各ZIP内の`SHA256SUMS.txt`を確認し、取得元とSHA-256が一致することを確認してください。SHA-256は改ざん検知に利用できますが、コード署名の代わりにはなりません。

## リポジトリについて

このPublicリポジトリは、README、利用条件、Release notes、配布物を公開するためのものです。アプリのソースコード、ビルド設定、テスト、開発用ドキュメントはPrivateリポジトリで管理しています。

## 利用条件

[利用条件](TERMS.md)および[ライセンス表示](LICENSE.md)を確認してください。
