# reCAPTCHA Demo

![reCAPTCHA Demo](https://img.shields.io/badge/demo-live-brightgreen) ![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

日本語対応のシンプルなreCAPTCHA v2デモアプリケーションです。Google reCAPTCHAを使用してユーザーが人間であることを確認します。

## 🚀 機能

- **日本語UI**: 完全日本語対応のユーザーインターフェース
- **reCAPTCHA v2統合**: Googleの信頼性の高いボット検出システム
- **レスポンシブデザイン**: モバイル・デスクトップ対応
- **モダンUI**: グラスモーフィズム効果とスムーズなアニメーション
- **軽量**: 依存関係なし、純粋なHTML/CSS/JavaScript

## 🎨 スクリーンショット

セキュリティ確認画面では、洗練されたグラデーション背景と直感的なカードデザインでユーザーエクスペリエンスを向上させています。

## 🛠 技術スタック

- **HTML5**: セマンティックマークアップ
- **CSS3**: モダンなスタイリング（Flexbox、グラデーション、アニメーション）
- **JavaScript**: バニラJS（フレームワーク不使用）
- **Google reCAPTCHA v2**: ボット検出API
- **Google Fonts**: Poppinsフォント

## 📁 プロジェクト構成

```text
reCAPTCHA/
├── index.html          # メインHTMLファイル
├── style.css           # CSSスタイルシート
├── script.js          # JavaScript機能
├── README.md          # プロジェクト説明書
└── .github/
    └── copilot-instructions.md  # AI開発ガイドライン
```

## 🚀 使用方法

### ローカル環境での実行

1. リポジトリをクローン:

```bash
git clone https://github.com/sizimi920/reCAPTCHA.git
cd reCAPTCHA
```

1. `index.html`をブラウザで開く:
   - ファイルエクスプローラーから直接開く
   - または任意のWebサーバーでホスト

### 本番環境でのデプロイ

静的ファイルホスティングサービスで簡単にデプロイできます：

- **GitHub Pages**: リポジトリ設定でPages機能を有効化
- **Netlify**: ドラッグ&ドロップでデプロイ
- **Vercel**: GitHubと連携して自動デプロイ

⚠️ **重要**: 本番環境では`index.html`内のreCAPTCHA Site Keyを自分のキーに変更してください。

## 🔧 カスタマイズ

### reCAPTCHA設定

1. [Google reCAPTCHA Console](https://www.google.com/recaptcha/admin/)でサイトキーを取得
2. `index.html`の`data-sitekey`属性を更新:

```html
<div class="g-recaptcha" data-sitekey="YOUR_SITE_KEY_HERE" data-callback="onHumanVerified">
```

### デザインカスタマイズ

- **カラーテーマ**: `style.css`のグラデーション色を変更
- **フォント**: Google Fontsのリンクを変更
- **アニメーション**: CSS keyframesを調整

## 📝 開発メモ

- デモ用サイトキー（`6Lc6CLMrAAAAADz0W43HhfzahZV14C3ErwQh2FC-`）は開発・テスト専用
- ファイルプロトコル（`file://`）でも動作確認可能
- HTTPSは開発環境では不要、本番環境では推奨

## 🙏 謝辞

このプロジェクトは、YouTubeチャンネル「ラムダ技術部」(@yoidea) の動画を参考にして作成されました。丁寧で分かりやすい技術解説に感謝いたします。

## 📄 ライセンス

このプロジェクトはMITライセンスの下で公開されています。詳細は[LICENSE](LICENSE)ファイルをご覧ください。

## 🤝 コントリビューション

プルリクエストやイシューの報告を歓迎します！改善提案がありましたらお気軽にお声かけください。

---

Inspired by yoidea
