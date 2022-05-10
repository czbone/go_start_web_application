# 概要

GoのWebアプリケーションを VSCode + Docker + Remote Containers で開発するためのプロジェクトです。

## 動作環境

- Windows10/11
- Docker Desktop
- VSCode(拡張機能: Go, Remote Containers)

## 使い方

1. Docker Desktopを起動します。完全に起動するまで待ちます。

2. 「PowerShell起動」ファイルをダブルクリックしてディレクトリを開きます。VSCodeを起動します。

```
> code .
```

3. VSCode起動直後に以下のメッセージのダイアログが表示されます。「Reopen in Container」ボタンでDockerコンテナを起動します。  
Dockerコンテナ環境が起動するとVSCodeがリモート接続状態(画面左隅に表示)になります。

```
Folder contains a Dev Container configuration file. Reopen folder to develop in a container (learn more)
```

4. 追加モジュールのインストールダイアログが表示された場合は「Install All」ボタンでインストールします。

5. サイドバーを「実行とデバッグ」ビューに切り替え、メニューから「Launch Server」(F5)を実行します。サーバが起動されWebブラウザでアクセス可能な状態になります。  
Webブラウザからアクセスします。

http://localhost:8080

6. アプリケーションのログは、「ターミナル」タブ(Ctrl+@)を表示しメニューから「Go Debug Terminal」を選択すると参照できます。
