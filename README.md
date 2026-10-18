# RoboTrain v0.2 — ロボット手術教育ログ

手術症例の記録、自律度・満足度の推移、メンターコメント、参考文献を扱う試作版です。

## GitHub Pages での公開方法
1. GitHub に新規リポジトリ `robotrain` を作成する（LARS のリポジトリとは別）。
2. このZIPを解凍し、中にある `index.html` と `.nojekyll` をリポジトリのルートにアップロードしてコミットする。
3. リポジトリの Settings → Pages → Build and deployment → Deploy from a branch → `main` / `/(root)` を選択して保存する。
4. 発行されたURL（例: https://manabumaebashi-debug.github.io/robotrain/）をブラウザで開く。URLはGitHubによる発行後に有効になります。

## 注意事項
- v0.2はブラウザ内 localStorage に保存し、サーバーには保存・送信しません。同じ端末・ブラウザ・サイトからの閲覧が必要です。
- HTMLファイルをローカルで開いた時の記録は、GitHub Pages版に自動では移行しません。「症例履歴・出力」でJSONを出力し、新しいサイトでインポートしてください。
- 「メンター」は現時点ではルールベースの文章表示です。外部AI APIは未接続です。
- GitHub Pages上で公開するのはデモ用途のみとし、患者個人情報・実名・対応表・病院機密データは登録しないでください。研究運用前に認証・アクセス制御・保存先の独立性・バックアップ等が必要です。
- GitHub Pagesはリポジトリが別でも同じ `github.io` ホスト配下ではブラウザの保存領域（origin）が同じです。保存キーは別ですが、医療情報の安全な分離ではありません。
