# kotatsuinu-pages

こたつ犬（Kotatsuinu）の個人発信ハブ。Farm Eolica からは緩やかに独立した、ハンドルネーム名義の汎用パブリックページ置き場。

## 公開URL

- ハブ: `https://kotatsuinu.farmeolica.com/`
- 個別: `https://kotatsuinu.farmeolica.com/<コンテンツ名>/`

> ドメインは Farm Eolica のサブドメインを借用。コンテンツの主体は個人（こたつ犬）。

## コンテンツ一覧

| パス | 内容 | 初版 |
|---|---|---|
| `/` | ハブ（コンテンツ一覧） | 2026-05-11 |
| `/values-map/` | 価値観マップ（リベシティ向け公開要約版） | 2026-05-11 |
| `/temoco/` | temoco サポートページ（`/temoco/en/` 英語版） | 2026-09-27 |
| `/temoco/privacy/` | temoco プライバシーポリシー（`/temoco/en/privacy/` 英語版） | 2026-09-27 |

## 構成

```
kotatsuinu-pages/
├── index.html          ← ハブページ
├── values-map/
│   └── index.html      ← 価値観マップ（Markmap描画）
├── temoco/             ← temoco（音声メモアプリ）のサポート・ポリシー
│   ├── index.html      ← サポート（日本語）
│   ├── privacy/index.html
│   └── en/             ← 英語版（index.html / privacy/index.html）
├── _assets/
│   └── styles.css      ← 共通スタイル
├── README.md
└── .gitignore
```

## デプロイ

Cloudflare Pages による static デプロイ。

- Build command: なし（静的サイト）
- Output directory: ルート
- Custom domain: `kotatsuinu.farmeolica.com`

push → 自動デプロイ。

## 新規コンテンツ追加手順

1. `<コンテンツ名>/index.html` を作成
2. `index.html`（ハブ）のコンテンツ一覧に追加
3. push → 自動公開

## 想定する公開内容

- 自己分析・価値観・思考整理（リベシティや個人コミュニティ向け）
- 副業・趣味の単発成果物
- 公開しても問題ない範囲の個人的な発信

> 事業 PR / Farm Eolica の商品案内 → `https://farmeolica.com/`
> 個人の思考・試行錯誤 → このリポジトリ
