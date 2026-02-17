# X (Twitter) Vertical Display Optimizer

縦ディスプレイ（ポートレートモード）でX.comを快適に閲覧するためのカスタムCSS。

## 変更内容

| 要素 | デフォルト | 適用後 |
|---|---|---|
| 左ナビ | 275px（テキスト付き） | 88px（アイコンのみ） |
| タイムライン | 600px | 残りスペース全幅 |
| 右サイドバー | 350px | そのまま |

- `@media (orientation: portrait)` 使用 — 縦ディスプレイでのみ適用
- 横ディスプレイでは通常のXレイアウトがそのまま使われます

## インストール

### Stylus（推奨）

1. [Stylus](https://chromewebstore.google.com/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne) Chrome拡張をインストール
2. [`x-vertical-display.user.css`](x-vertical-display.user.css) を開く
3. 「Raw」ボタンをクリック → Stylusが自動検出してインストール画面を表示
4. 「インストール」をクリック

### 手動

1. Stylusアイコン → 「スタイルを管理」
2. 「新しいスタイルを作成」
3. CSSファイルの `@-moz-document` ブロック内をコピーして貼り付け
4. 保存

## 注意事項

- X.comのUI更新により `data-testid` セレクタが変わる可能性があります
- 動作しなくなった場合はDevToolsで現在のセレクタを確認してください
- `.r-f8sm7e` はタイムラインの `max-width: 600px` に対応するクラスです（変更される可能性あり）

## License

MIT
