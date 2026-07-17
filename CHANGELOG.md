# Changelog

このリポジトリのリリース履歴。Brand Guide §11.4 の Semver に従います。

## [v2.2.1] - 2026-07-17

### Changed
- `screenshots/pro/screenshot_pro_v1.0.0_exec-summary-kpi.png` — 公開Hub向けに明るさ・余白を調整したPro版KPI画面ショットへ差し替え

## [v2.2.0] - 2026-07-17

### Added
- `covers/common/cover_common_v1.0.0_brand.png` — 主要ページ用の共通ブランドカバー画像を追加
- `screenshots/pro/screenshot_pro_v1.0.0_exec-summary-kpi.png` — Pro版エグゼクティブサマリーのKPI画面ショットを追加

## [v2.1.0] - 2026-07-17

### Added
- `illustrations/common/illust_common_v1.0.0_tier-stepup.svg` — 公開用ラインナップHub向けの3ティア移行ステップ図を追加
- Lite → Standard → Pro → 専用CRMへの成長・移行経路を可視化

## [v2.0.0] - 2026-07-14

### Added
- `keyvisuals/pro/keyvisual_pro_v1.4.0.png` — Pro版キービジュアルの最新版を追加

### Changed
- CHANGELOGへv1.5.0〜v1.9.2のリリース履歴を補完

## [v1.9.2] - 2026-06-30

### Fixed
- ブランドアイコン PNG を命名規約準拠・正しいパス（`brand/` 直下）へ修正
  - `brand/icon/square.png` → `brand/appicon_brand_v1.0.0_s-monogram.png`（角丸スクエア / favicon・STUDIO サイトアイコン用, 512x512）
  - `brand/icon/circle.png` → `brand/snsicon_brand_v1.0.0_s-monogram.png`（円形 / note アカウントA・X プロフィール用, 400x400）
  - 空になった `brand/icon/` サブフォルダを削除し、`brand/icons.json` のマニフェスト宣言とパス・ファイル名を一致させた

## [v1.9.1] - 2026-06-30

### Added
- `brand/icons.json` — ブランドアイコン（S モノグラム）定義マニフェスト
- ブランドアイコン PNG 実体を追加（S モノグラム / 背景 #0F94B4・前景 #FFFFFF, Plus Jakarta Sans Bold）
  - App Icon（角丸スクエア, 512x512, favicon・STUDIO 用）
  - SNS Icon（円形, 400x400, note A・X 用）
  - ※ 初回アップロード時のパス・名称が命名規約と不一致だったため v1.9.2 で修正

## [v1.9.0] - 2026-06-24

### Added
- `illustrations/lite/image.svg` — Lite 版イラストを追加（※ ファイル名が命名規約 `{asset-type}_{scope}_{semver}_{descriptor}` 非準拠。要リネーム）

## [v1.8.0] - 2026-06-17

### Added
- `illustrations/standard/illust_standard_v1.0.0_legal-counsel.svg` — Standard 版イラスト（`undraw_legal-counsel.svg` を §11.1 準拠にリネームして追加）

## [v1.7.0] - 2026-06-17

### Added
- `illustrations/pro/illust_pro_v1.0.0_data-trends.svg` — Pro 版イラスト（data-trends）

## [v1.6.0] - 2026-06-17

### Added
- `illustrations/standard/illust_standard_v1.0.0_environmental-study.svg` — Standard 版イラスト（environmental-study）
- `illustrations/standard/illust_standard_v1.0.0_spreadsheets.svg` — Standard 版イラスト（spreadsheets）

## [v1.5.0] - 2026-06-17

### Added
- `illustrations/pro/illust_pro_v1.0.0_docs-fullview.png` — Pro 版イラスト（docs-fullview）

## [v1.4.0] - 2026-06-17

### Added
- `note-covers/note/`, `note-covers/column/` — コラム / note 記事カバー原本のカテゴリを新設
- `og/note/` — OGP 画像カテゴリを新設
- 命名規約に `{scope}` 一般化ルール（記事カバー用 `{asset-type}_{scope}_{semver}_{descriptor}`）を追加（README / Brand Guide §11.1）

## [v1.3.0] - 2026-06-03

### Added
- `keyvisuals/pro/keyvisual_pro_v1.3.0.png` — Pro 版キービジュアルをアップロード（プレースホルダーから実アセットへ）

## [v1.2.4] - 2026-05-29

### Fixed
- ルートに残存していた `Lite概要修正版.srt` の最終削除（v1.2.3 で削除漏れ）

## [v1.2.3] - 2026-05-29

### Fixed
- ルートに残っていた `Lite概要修正版.srt` の重複コピーを削除
- `undraw_judge_hyqv (1).svg` → `undraw_judge.svg` にリネーム（命名規約準拠）
- `undraw_legal-counsel_kdnh.svg` → `undraw_legal-counsel.svg` にリネーム（命名規約準拠）

## [v1.2.2] - 2026-05-29

### Fixed
- `captions/lite/caption_lite_v1.0.0_ep01-overview_ja.srt` を正しいパス・命名規約に修正（v1.2.0/v1.2.1 で漏れていた）

## [v1.2.1] - 2026-05-29

### Fixed
- `keyvisuals/lite/keyvisual_lite_v1.0.0_excel-graduation.png` を正しいパス・命名規約に修正
- `captions/lite/caption_lite_v1.0.0_ep01-overview_ja.srt` を正しいパス・命名規約に修正

## [v1.2.0] - 2026-05-29

### Added
- `keyvisuals/lite/` — Lite 版キービジュアル（excel-graduation）
- `keyvisuals/standard/`, `keyvisuals/pro/` — 将来用プレースホルダー
- `captions/lite/` — Lite 概要編 SRT 字幕（ep01-overview_ja）
- `thumbnails/lite/` — YouTube サムネ・OGP 用プレースホルダー
- `icons/lucide/` — Lucide ベースアイコン用プレースホルダー
- `brand/colors.json` — Scale-Ready ブランドカラーパレット
- `illustrations/standard/` — Standard 版イラスト 24 種
- `illustrations/pro/` — 将来用プレースホルダー
- README.md・CHANGELOG.md を整備

## [v1.1.0] - 2026-05-26

### Changed
- `undraw_terms.svg` リネーム

## [v1.0.0] - 2026-05-26

### Added
- `illustrations/lite/` — Lite 版イラスト初版
