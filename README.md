# cursor-in-brackets.el --- move cursor in brackets/quotes when right bracket/quote is inserted

`cursor-in-brackets-mode` は、左括弧・クオートの後に右括弧・クオートが入力されたときにカーソルを括弧・クオートの中に移動させるマイナーモードです。
対象の括弧とクオートは以下の通りです。

- ()
- {}
- []
- <>
- ""
- ''
- \`'
- \`\`
- $$

`cursor-in-brackets-mode` はリージョンに基づく括弧付けにも対応しています。
`transient-mark-mode` のリージョンで右括弧が入力されると、リージョンが括弧付けされてカーソルが右括弧の前に移動されます。
代わりに左括弧が入力されると、リージョンが括弧付けされてカーソルが左括弧の後に移動されます。

# 使い方

    (require 'cursor-in-brackets)
    (global-cursor-in-brackets-mode t)

# バージョン

## 1.0.0 on 26 May 2013

ファーストコミット
