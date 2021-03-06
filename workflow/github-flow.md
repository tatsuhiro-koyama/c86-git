# github-flow
git-flowはよく考えられているブランチモデルなのですが、流れが少々複雑であることと、featureブランチをmasterではなく、developブランチから開始するなど多少の課題を抱えています。

そこで、GitHubが使える環境においてはgithub-flowもよく使われます。git-flowに比べ、github-flowのブランチはとてもシンプルで、下記の二つのみです。

- masterブランチ
- featureブランチ

masterブランチは何であれ、いつでもデプロイ可能です。featureブランチはmasterブランチから分岐します。

簡単な流れとしては以下のようになります。

- 新しい何かに取り組む際は説明的な名前のブランチをmasterから作成する
- 作成したブランチにローカルでcommitし、サーバ上の同じ名前のブランチにも定期的に作業内容をpushする
- フィードバックや助言が欲しい時、ブランチをマージしても良いとおもったときは、Pull Requestを作成する
- 他の誰かがレビューをして機能にOKを出してくれたら、コードをmasterへmergeすることができる
- mergeしてmasterへpushしたら、直ちにデプロイをする。
