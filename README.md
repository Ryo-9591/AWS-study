# AWS勉強用リポジトリ

このリポジトリは、AWSの勉強用です。

### 🚀 自動プッシュスクリプトの実行方法

#### PowerShellの実行ポリシーを変更

初回のみ、PowerShellでスクリプト実行を許可する必要があります。

**方法: 現在のセッションのみ許可**
```powershell
Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process
```

#### スクリプトの起動

プロジェクトディレクトリで以下のコマンドを実行：

```powershell
.\auto-push.ps1
```

スクリプトが起動すると、1分ごとに変更をチェックして自動的にGitHubにプッシュします。

#### スクリプトの停止

`Ctrl + C` を押すとスクリプトが停止します。
