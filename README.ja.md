# Githubプロフィールの爆発アニメーション SVG

日本語 | [English](/README.md)

GitHubプロフィールのREADMEをド派手に飾る、外部依存ゼロの超軽量アニメーションSVGバッジです！

![Demo](./explosion.svg)

---

## ✨ 特徴

- 🚀 **外部サーバー依存なし**: SMIL仕様のインラインSVGで完結。外部APIのサーバーダウンによる画像切れがありません。
- 🔁 **滑らかな無限ループ**: GitHubのプロキシ（Camo proxy）キャッシュ問題を回避する完全ループ設計。
- 🎨 **簡単カスタマイズ**: SVGファイル内のテキストやカラー、速度をテキストエディタで簡単に変更可能。

---

## 🚀 使い方（Quick Start）

### 1. SVGファイルをダウンロード
このリポジトリから [`explosion.svg`](./explosion.svg) をダウンロードし、ご自身のプロフィールリポジトリ（例: `your-username/your-username`）にアップロードします。

### 2. ユーザー名・テキストの変更
アップロードした `explosion.svg` をテキストエディタで開き、末尾付近にある `<text>` タグ内の `YOUR_NAME` をご自身のユーザー名や好きな文字列に変更します:

```xml
<!-- explosion.svg -->
<text x="0" y="0" dominant-baseline="central" text-anchor="middle" class="main-text">
  YOUR_NAME <!-- 👈 ここを自分のユーザー名に変更 -->
</text>
```

### 3. README.md に貼り付け
ご自身のプロフィール用 `README.md` に以下のHTMLタグを貼り付けます:

```html
<div align="center">
  <img src="./explosion.svg" width="100%" alt="Explosion Badge" />
</div>
```

---

## 🎨 カスタマイズ手順

### 色の変更
`explosion.svg` 内のスタイル指定を変更することで、粒子や衝撃波の色を自由に変えられます:

- **背景色**: `.bg` 内の `fill: #0d1117;` を変更
- **文字色**: `.main-text` 内の `fill: #ffffff;` を変更
- **衝撃波**: `.shockwave-color` 内の `stroke: #00f0ff;` を変更
- **粒子**: 各 `<circle>` タグの `fill` 属性を変更

### 文字サイズの調整
ユーザー名が長く枠からはみ出る場合は、`<style>` セクション内のフォントサイズを調整してください:

```css
.main-text {
  font-size: 28px; /* 文字数に合わせて調整 */
}
```

---

## ⭐️ 応援（Star）のお願い

役に立った・気に入っていただけた場合は、ぜひリポジトリへの **Star（⭐️）** をよろしくお願いします！