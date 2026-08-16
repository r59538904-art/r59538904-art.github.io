# r59538904-art.github.io

`https://r59538904-art.github.io/` として公開される入口ページです。

ここに置いているもの。

| ファイル | 役割 |
|---|---|
| `index.html` | 公開しているツールの一覧 |
| `robots.txt` | クローラー向けの指示。**ドメイン直下にしか置けない**ため、このリポジトリが必要 |
| `sitemap.xml` | 各ページのURL一覧 |

## なぜ別リポジトリなのか

`robots.txt` と `sitemap.xml` は、クローラーも Lighthouse も**ドメイン直下**（`/robots.txt`）しか読みません。
シミュレーター本体は `github.io/tax-scholarship-simulator/` という配下にあるため、
そこに置いたファイルは読まれませんでした。GitHub Pages でドメイン直下を配信できるのは
`ユーザー名.github.io` という名前のリポジトリだけなので、これを作っています。

## 中身の追加

ツールを増やしたら、`index.html` にカードを1つ足し、`sitemap.xml` に `<url>` を1つ足してください。
外部からファイルを読み込まない作りにしてあります（CSPで禁止しているため、CDN等を足すと表示されません）。
