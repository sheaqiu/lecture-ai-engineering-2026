# 英語版の出典と保存方針

私は最初に公式英語版の `matsuolab/lecture-ai-engineering-2026-en` をforkし、演習のFAQ実験とAdvancedの用語集実験を実行しました。その後、日本語版の主リポジトリをforkし直し、提出資料を移しました。

## 固定した資料

- 実験時の自分のfork：`sheaqiu/lecture-ai-engineering-2026-en`。
- 公式英語版のコミット：`2a89014410768f2307a72d0727d1c6bdb29cd726`。
- [演習の元のノートブック](https://github.com/matsuolab/lecture-ai-engineering-2026-en/blob/2a89014410768f2307a72d0727d1c6bdb29cd726/notebooks/lora_format_tuning.ipynb)。
- [元の用語集](https://github.com/matsuolab/lecture-ai-engineering-2026-en/blob/2a89014410768f2307a72d0727d1c6bdb29cd726/data/glossary.json)：58項目。[今回保存した実験用の写し](../advanced/glossary.json)。
- [元のデータ生成スクリプト](https://github.com/matsuolab/lecture-ai-engineering-2026-en/blob/2a89014410768f2307a72d0727d1c6bdb29cd726/scripts/make_sft_dataset.py)：変更せずに116件の問答を生成しました。
- 提出用の日本語版の基点：`bc41dfac203acff0706b7da10d09339d91830bfe`。

英語のFAQ、質問、定義、共通のシステム指示を使った結果です。日本語版のFAQや用語集に差し替えた実験ではなく、日本語データを使った測定値としては扱いません。元のFAQ演習とAdvanced課題は別の実験で、各実験内で学習前後を比較しています。

## 移行時に変更したもの

提出先、ノートブックの説明・表示文言、リンクと資料の出典説明を変更しました。ノートブックは引き続き `lectures/02/advanced/` の固定した実験資材を読み込みます。リポジトリ直下の日本語版 `data/glossary.json` を読み込む構造には変更していません。

## 実行時のまま保持したもの

`advanced/` の元の9ファイルと `results/` の元の出力は、移行前とバイト単位で同じです。データ、プロンプト、採点規則、モデル出力、ログとファイルハッシュは変更していません。`manifest.json` と `result.json` 内の旧リポジトリ名は実験時の出典を示す記録として保持しています。

`advanced/README.md` は実験前に作成され、結果ZIPにも含まれた英語の資材説明です。「未実行」という記載は資材準備時点の状態を表しています。現在の日本語の説明は [README.ja.md](../advanced/README.ja.md)、実際の実行結果は [レポート](../answer.md) と [結果の説明](../results/advanced/README.md) を参照してください。

ノートブックの説明言語とリンクの変更に伴う再学習は行っていません。保存した測定値は最初の実行時の記録です。
