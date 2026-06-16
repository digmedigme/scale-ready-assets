# Scale-Ready CRM Assets

Notion テンプレート **Scale-Ready CRM**（Lite / Standard / Pro）配布用のアセットリポジトリ。
jsDelivr CDN 経由でテンプレ内に直接埋め込んで使用します。

## CDN ベース URL

形式：

    https://cdn.jsdelivr.net/gh/digmedigme/scale-ready-assets@{tag}/{path}

- `{tag}` は **必ず Semver タグを指定**（例：`v1.2.0`）
- `main` 参照は配布済みテンプレ互換性の観点から非推奨

## ディレクトリ構成

| パス | 用途 |
|---|---|
| `keyvisuals/{tier}/` | キービジュアル（SVG / PNG 1920x1080） |
| `thumbnails/{tier}/` | YouTube サムネ・OGP 兼用（PNG 1280x720） |
| `captions/{tier}/` | 動画字幕（SRT） |
| `illustrations/{tier}/` | undraw 系イラスト（SVG） |
| `icons/lucide/` | Lucide ベースのアイコン |
| `brand/` | カラー・タイポ・Brand Guide |
| `note-covers/{scope}/` | コラム・note 記事カバー（PNG, note 1280x670 / 汎用 1500px幅） |
| `og/{scope}/` | OGP・SNS シェア画像（PNG 1200x630） |

`{scope}` は配信チャネル / 用途（`note` / `column` / `og` 等）。

## 命名規約（Brand Guide §11.1）

形式：

    {asset-type}_{tier}_{semver}_{descriptor}.{ext}

例：

- `keyvisual_lite_v1.0.0_excel-graduation.png`
- `caption_lite_v1.0.0_ep01-overview_ja.srt`
- `thumbnail_lite_v1.0.0_ep01-overview.png`

### 記事カバー（製品アセット以外）

コラム・note 記事・OGP など製品ティアに紐づかないアセットは、`{tier}` を `{scope}`（配信チャネル / 用途）に読み替える：

    {asset-type}_{scope}_{semver}_{descriptor}.{ext}

例：

- `notecover_note_v1.0.0_crm-failure-patterns.png`
- `ogimage_og_v1.0.0_crm-failure-patterns.png`

- `descriptor` は記事管理 DB の `slug` と**完全一致**させる（記事↔画像の追跡性確保）
- サイズはファイル名に含めず、カテゴリ（フォルダ）単位で規定する
- 連番・自動命名（`star1.svg` 等）は §11.1 違反として是正対象

## バージョニング

Brand Guide §11.4 の Semver（Major / Minor / Patch）準拠。
新規バージョンは git tag で打ちます：

    git tag v1.x.0
    git push origin v1.x.0

## ライセンス

LICENSE ファイルを参照。
