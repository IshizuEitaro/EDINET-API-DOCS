# EDINET API Documentation (Markdown Edition)

[English Edition (README_en.md)](README_en.md)

金融庁が提供する「EDINET API 仕様書」および関連ドキュメントを、閲覧・検索性に優れた Markdown 形式に変換し、クリーンアップしたリポジトリです。

## プロジェクトの概要

本リポジトリは、政府統計や企業開示情報の活用を促進するため、原本の PDF 形式では困難だった「変更箇所の差分管理」「各種ツールとの連携」を容易にすることを目的に作成されました。

単なる自動変換にとどまらず、手動でのレイアウト調整や Mermaid による図解の追加を行っています。

## 収録ドキュメント

- **[EDINET API 仕様書 (ESE140206.md)](ESE140206.md)**
  - EDINET API の利用方法、エンドポイント、認証、レスポンス形式を網羅したメインドキュメント。
- **[様式コードリスト (ESE140327.md)](ESE140327.md)**
  - 提出書類の様式コード（Form Code）の定義リスト。
- **[提出書類一覧のデータ出力例 (ESE140328.md)](ESE140328.md)**
  - 財務局職員による不開示処理など、複雑なユースケースにおける出力データの具体例。

## 付属データ

- **`EdinetcodeDlInfo.csv`**: EDINET コードや提出者名、証券コードなどのリファレンスデータ。
- **`ESE140190.csv`**: API 連携等で使用される、原本に付随するリファレンス CSV。

## 主な特徴と改善点

- **クリーンな Markdown 形式**: PDF からの変換時に発生する改行の断片化やテーブルの崩れを手動で修正。
- **Mermaid 図解**: 原本で図示されていた書類の親子関係や取下げフローを、コードベースで修正可能な Mermaid ダイアグラムに置き換え。
- **最適化されたテーブル**: 大規模なレスポンスフィールド定義などを、Markdown テーブルとして整形し、GitHub 上での閲覧性を向上。
- **画像の整理**: 参照されていない重複画像を削除し、必要な画像のみを `ESE140206_images/` に集約。

## 作成プロセス

1.  **原本**: [EDINET API 仕様書](https://disclosure2dl.edinet-fsa.go.jp/guide/static/disclosure/WZEK0110.html) から PDF を取得。
2.  **変換**: [opendataloader-pdf](https://github.com/opendataloader-project/opendataloader-pdf) を使用して Markdown のベースを生成。
3.  **クリーンアップ**: 変換アーティファクトの除去、テーブルの列順標準化、文字化けの修正を実施。
4.  **エンハンス**: 複雑なフロー図を Mermaid.js 形式で手動実装。

## ライセンス・免責事項

- **原本著作権**: 本ドキュメントの元となる情報の著作権は、[金融庁](https://www.fsa.go.jp/)に帰属します。
- **リポジトリのライセンス**: 本リポジトリにおける Markdown への変換および付加的な構成・ダイアグラムについては [MIT License](LICENSE) の下で公開されています。
- **利用規約への準拠**: 本リポジトリの利用にあたっては、[EDINET 利用規約](https://disclosure2dl.edinet-fsa.go.jp/guide/static/submit/WZEK0030.html) を遵守してください。
