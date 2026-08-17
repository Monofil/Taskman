# Taskman

Taskmanは、個人利用向けのローカル完結型ビジュアルタスク管理デスクトップアプリです。TaskをTimeline、Kanban、WBSで可視化し、Project、依存関係、進捗、期限超過をSQLiteで管理します。

> [!WARNING]
> v0.1.0は未署名のPre-release（個人検証用）です。安定版・正式配布版ではありません。Microsoft Defender SmartScreenまたはSmart App Controlにより警告・ブロックされる場合があります。

## ダウンロード

- [最新版のRelease](https://github.com/Monofil/Taskman/releases/latest)
- [Windows 11 x64 通常版](https://github.com/Monofil/Taskman/releases/latest/download/Taskman-v0.1.0-windows-x64.zip) — 推奨。NSIS installerとWebView2オフラインinstallerを含みます。
- [Windows 11 x64 standalone版](https://github.com/Monofil/Taskman/releases/latest/download/Taskman-v0.1.0-windows-x64-standalone.zip) — WebView2 Runtime導入済み環境向け。

GitHubが自動表示する`Source code (zip)`は、この配布用リポジトリのREADME等をまとめたものであり、Taskmanアプリ本体ではありません。必ずReleaseの`Assets`から上記の配布ZIPを取得してください。

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

v0.1.0は未署名です。Release notesと各ZIP内の`SHA256SUMS.txt`を確認し、取得元とSHA-256が一致する場合に限って使用してください。SHA-256は改ざん検知に利用できますが、コード署名の代わりにはなりません。

## リポジトリについて

このPublicリポジトリは、README、利用条件、Release notes、配布物を公開するためのものです。アプリのソースコード、ビルド設定、テスト、開発用ドキュメントはPrivateリポジトリで管理しています。

## 利用条件

[利用条件](TERMS.md)および[ライセンス表示](LICENSE.md)を確認してください。
