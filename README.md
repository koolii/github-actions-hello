# github-actions-hello

The first Github Actions made by koolii

## `actions/toolkit`

ref: https://github.com/actions/toolkit

JavaScriptアクションを作りやすくするためのパッケージが公開されている

### パッケージ

- @actions/artifact: アーティファクトのアップロード、ダウンロード
- @actions/core: パラメータの読み込み、アウトプットの設定、環境変数の出 力、シークレットの設定、PATH の追加、終了ステータスの変更、ログ、アクションのステート管理
- @actions/exec: コマンドライン実行
- @actions/github: github コンテキストへのアクセス、proxy 設定を読み込む Octokit*4 クライアント
- @actions/glob: glob パターンにマッチするファイル一覧を検索
- @actions/io: ファイルシステム操作
- @actions/tool-cache: ダウンロード、展開、キャッシュ(ジョブ間のキャッシュではなく、そのジョブ内のみで使えるキャッシュ)– 名前がややこしいけど、「2.5 キャッシュ」で出てくるキャッシュとは完全に別物です

パッケージングには `@zeit/ncc` でバンドルするのが良いらしい

### テンプレート

- actions/javascript-action
- actions/typescript-action
- actions/container-action

実際に作るときは、上記のテンプレートリポジトリに移動してリポジトリを作成すれば良い