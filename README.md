# rewrite-tick

個人用アプリの通知を時刻どおりに出すための、定期実行だけのリポジトリです。

- `tick.yml`：5分ごとに、Secrets の `TICK_URL` へ `x-tick-secret` ヘッダーつきで POST する
- `keepalive.yml`：60日で定期実行が止まらないよう、50日動きが無ければ空のコミットを足す

アプリのコードや個人の内容は置いていません。URL と秘密の値は GitHub の Secrets だけにあります。
