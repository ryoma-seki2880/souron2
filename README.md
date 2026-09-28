# 総論Ⅱ 〇✕クイズ

柔道整復師国家試験対策の〇✕クイズです(総論Ⅱ:脱臼・筋・腱・靭帯・神経・関節損傷)。
GitHub Pages で公開する静的サイトで、サーバーやGASは使いません。

## ファイル構成

| ファイル | 役割 |
|---|---|
| `index.html` | クイズ本体 |
| `questions.json` | 問題データ(194問) |
| `convert.html` | スプレッドシートのCSVから `questions.json` を作る変換ツール |

## 公開手順(初回)

1. GitHubで新しいリポジトリを作る(例:`soron2-quiz`、Public)
2. リポジトリ画面の「Add file → Upload files」で、上の3ファイルをまとめてドラッグ&ドロップし「Commit changes」
3. 「Settings → Pages」を開き、Source を「Deploy from a branch」、Branch を `main` / `/(root)` にして「Save」
4. 1〜2分待つと `https://<ユーザー名>.github.io/soron2-quiz/` で公開される

## 問題を追加・修正するとき

1. スプレッドシートを編集する(列:カテゴリ / 回答 / 問題文 / 解説)
2. 「ファイル → ダウンロード → カンマ区切り形式(.csv)」でCSVを保存する
3. 公開中の `https://<ユーザー名>.github.io/soron2-quiz/convert.html` を開き、CSVを選んで `questions.json` をダウンロードする
4. リポジトリで「Add file → Upload files」から新しい `questions.json` をアップロードして上書きする

数分で反映されます。反映されない場合はページを再読み込みしてください。

## 補足

- 間違えた問題の記録は、各自の端末のブラウザ内に保存されます(端末をまたいでは共有されません)。
- 問題文を書き換えると、その問題の間違い記録は引き継がれません(問題文で問題を識別しているため)。
- `index.html` をダブルクリックして直接開くと、問題データを読み込めません。確認は公開後のURLで行ってください。
