---
title: Qiita_CLI
tags:
  - QiitaCLI
private: true
updated_at: '2025-06-01T09:28:40+09:00'
id: effa20c2e2de6efc0873
organization_url_name: null
slide: false
ignorePublish: false
---
## はじめに

便利なのだが、お作法がある。このお作法を守りたいのだが、たまにの投稿だと忘れそう。なので、ここにまとめてみます。

## リンク集
[(GitHub) qiita-cli](https://github.com/increments/qiita-cli)
[Qiitaの記事をGitHubリポジトリで管理する方法](https://qiita.com/Qiita/items/32c79014509987541130)
[Qiitaのタグ一覧(アルファベット順)](https://qiita.com/j5c8k6m8/items/5601e2f8fbe16887de68)

## テンプレの文法エラーの回避

自動生成された新しい記事用のmdファイルで文法エラーが指摘される。Qiita用のヘッダ情報の後に「#が1つ」の文が現れるため。
MD025 - Multiple top-level headings in the same document [MD25](https://github.com/DavidAnson/markdownlint/blob/v0.37.4/doc/md025.md)

``` Qiita CLIのテンプレ
# new article body
```

この指摘を回避するために、##と、#を1つ追加した
