# history

> コマンドラインの履歴です。
> もっと詳しく: <https://www.gnu.org/software/bash/manual/html_node/Bash-History-Builtins.html#index-history>。

- コマンドの履歴一覧を行番号付きで表示する:

`history`

- 直近の20個のコマンドを表示する (Zsh では20個目から始まるすべてのコマンドを表示する):

`history {{20}}`

- コマンド履歴のリストを消去する (現在の Bash シェルに対してのみ):

`history -c`

- コマンド履歴ファイルを現在の Bash シェルのコマンド履歴で上書きする (履歴を削除するために `history -c` と組み合わせることがよくあります):

`history -w`

- 指定されたオフセットの履歴エントリーを削除する:

`history -d {{オフセット}}`
