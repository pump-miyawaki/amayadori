# Amayadori | CafeBar — サイト制作データ

studio.site（https://amayadori-cafebar.studio.site/）とInstagram（@amayadori_cafebar）の内容をもとに、
pump-works-productsのテンプレート構成を踏襲して制作した1ページ構成のサイトです。

## ファイル構成
```
amayadori/
├── index.html      本体
├── css/style.css   スタイル（デザイントークンはファイル冒頭 :root にまとめています）
├── js/main.js      ヘッダー制御・スクロール演出・モバイルメニュー
└── images/         写真を入れるフォルダ（下記「差し替えが必要な画像」参照）
```

## GitHubリポジトリへの追加方法
1. `amayadori` リポジトリを開く
2. このフォルダの中身一式（index.html / css / js / images）をリポジトリのルートに追加
3. 既存の index.html などがあれば上書き、または `git add . && git commit -m "サイト初版" && git push`
4. GitHub Pagesを使う場合は、リポジトリの Settings → Pages で公開ブランチ／フォルダを指定

## 差し替えが必要な画像
サイト内は現在プレースホルダー（グレーの枠に薄く注記が入った状態）になっています。
下記のファイル名で `images/` に置いて `index.html`内の該当箇所（`class="ph"` の div）を
`<img src="images/○○.jpg" alt="...">` に差し替えてください。

| ファイル名 | 用途 | 推奨サイズ |
|---|---|---|
| hero.jpg | トップのバーカウンター写真 | 1920×1200 |
| about.jpg | About セクションの店内・外観写真 | 900×1100（縦） |
| owner.jpg | 店主（神園様）の写真（任意） | 600×600 |
| gallery-01.jpg | 店内・カウンターの様子 | 横長 |
| gallery-02.jpg | カクテル | 正方形 |
| gallery-03.jpg | ワイン | 正方形 |
| gallery-04.jpg | コーヒー | 正方形 |
| gallery-05.jpg | セミナーの様子 | 横長 |

studio.siteとInstagramの画像は保護されており自動取得できなかったため、
オーナー様がお持ちの元データ（Canvaの素材やInstagram投稿の元画像）を直接ご使用ください。

## 未確定の内容（ご確認ください）
- **Menuセクション**：studio.site側がまだ空欄だったため、Instagramの投稿内容
  （Mixology / Wine / Coffee / Seminarの4本柱、"Peach & Ginger"などの季節カクテル）から
  仮のメニュー構成を作成しています。実際のメニュー名・価格に差し替えてください（`index.html` の
  `id="offerings"` 内、`.offer-card` を編集）。
- **Access**：住所・営業時間・Googleマップは studio.site / Instagram の記載から反映済みです。
  Googleマップの「開く」ボタンは実際の店舗リンク（maps.app.goo.gl/Vsxqd48NCV3fwFjbA）に
  設定しています。

## 使用フォント（Google Fonts／無料）
- Cormorant Garamond（英字見出し）
- Shippori Mincho（和文見出し）
- Zen Kaku Gothic New（本文）

## デザインコンセプト
「雨宿り」というブランド名から着想し、雨（ネイビー・雨のアニメーション）から
晴れ間（アンバー・灯りの色）へと視線が移っていくような配色にしています。
sa-nu.com/weekday を参考に、余白を大きく取った落ち着いたスクロール構成にしました。
