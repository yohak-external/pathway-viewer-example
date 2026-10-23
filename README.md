# Pathway Viewer Stanza

## Implementation

- stanza フォルダにある js/css を設置
- HTML上でJSへのパスを通す
- `togostanza-pathway-viewer` のタグを任意の位置に挿入
- スタンザのパラメータを設定
- 必要に応じてスタイリングを整える

## Params

- `data-url (required)`
    - json ファイルへのパス
    - `fetch` でアクセス可能なURLで記載する
- `height (optional, default:undefined)`
    - スタンザを描画する高さをピクセル単位で指定できる
    - CSSでの指定を上書きするので注意 (一般的なHTMLタグとは逆の挙動)
- `grid-size (optional, default:75)`
    - グリッド表示をオンにしたときの1グリッドあたりのピクセル数
    - 初期拡大率の調整に使える

## Styling

- `togostanza-pathway-viewer` タグに対して直接参照して指定できる
    - もちろん、class や id を用いることも可能

## Bundled version

- Viewer version: `20261022`
- API schema version: `20251003`
- Source: [v20261022](https://github.com/dbcls/pathway_viewer/tree/v20261022)
- Source commit: `e82141955b1bbd2f3533272e298c8264aaf3ac0b`

`src/stanza/` の JS/CSS とソースマップは、上記タグの `pathway-playground` で `mise exec -- pnpm stanza:build` を実行し、`apps/stanza/dist/` からコピーしたもの。Viewer 内の Info タブでもバージョンを確認できる。
