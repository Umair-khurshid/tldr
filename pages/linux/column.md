# column

> Format `stdin` or a file into multiple columns.
> Columns are filled before rows; the default separator is a whitespace.
> More information: <https://manned.org/column>.

- Format the output of a command for a 30 characters wide display:

`printf "header1 header2\nbar foo\n" | column {{[-c|--output-width]}} {{30}}`

- Split columns automatically and auto-align them in a tabular format:

`printf "header1 header2\nbar foo\n" | column {{[-t|--table]}}`

- Specify the column delimiter character for the `--table` option (e.g. "," for CSV) (defaults to whitespace):

`printf "header1,header2\nbar,foo\n" | column {{[-t|--table]}} {{[-s|--separator]}} {{,}}`

- Fill rows before filling columns:

`printf "header1\nbar\nfoobar\n" | column {{[-c|--output-width]}} {{30}} {{[-x|--fillrows]}}`
