# ポートフォリオ（GitHub Pages用）

## ファイル構成

```
portfolio/
├── index.html          TOP
├── about.html          About
├── works/
│   ├── index.html      Works一覧
│   ├── work-01.html    詳細ページ（書き方の例文入り）
│   ├── work-02.html    詳細ページ（【 】を埋める記入用）
│   └── work-03.html    詳細ページ（【 】を埋める記入用）
├── css/style.css       全ページ共通のデザイン
└── images/             画像（今は仮のSVG画像が入っています）
```

## 書き換えるところ

1. **名前・連絡先**：全ページの「山田 太郎」「you@example.com」、LinkedInのURL
2. **TOPの一文**：`index.html` の `hero-statement`。仕事で大事にしている考えを一文で
3. **About**：経歴、得意なこと、スキル
4. **Works**：`work-01.html` は例文です。ご自身の実績に置き換えてください。`work-02` と `work-03` は【 】を埋めていきます
5. **画像**：`images/` に自分の画像を入れ、HTMLの `src="…svg"` をそのファイル名に変えます。`alt` も画像の内容に合わせて書き換えます

### 詳細ページの書き方のコツ
- いちばん大事なのは「課題の設計」です。**最初の依頼 → わかったこと → 解くべき課題** の順に書くと、考え方が伝わります
- 「進め方」の各手順には、**決めたこと・捨てたこと**を1行ずつ。判断力が伝わります
- 成果は、できるだけ数字で。出せない場合は「社内でどう使われているか」でも大丈夫です
- 守秘義務のある情報は、社名を伏せる・数字を割合にするなどして、掲載の許可を確認しましょう

### 作品を増やすとき
- `work-02.html` をコピーして `work-04.html` を作る
- `works/index.html`（とTOP）の `<li class="work-item">…</li>` をコピーしてリンク先を変える

### 色を変えるとき
`css/style.css` のいちばん上、`:root` の中の色の値を変えると全ページに反映されます。

## GitHub Pagesで公開する手順

1. GitHubで新しいリポジトリを作る（Public）
   - リポジトリ名を `ユーザー名.github.io` にすると、URLが `https://ユーザー名.github.io/` になります
2. 「Add file」→「Upload files」で、`portfolio` フォルダの**中身**（index.html など）をまとめてドラッグして「Commit changes」
3. 「Settings」→「Pages」→ Branch を `main`、フォルダを `/(root)` にして「Save」
4. 数分待つと、ページ上部に公開URLが表示されます

更新するときは、変更したファイルを同じ場所にアップロードし直すだけです。
