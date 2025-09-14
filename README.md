# Trashx - A simple trash management tool.

`trashx` is a simple trash management tool.

## Dependancies

- `uuidgen` : for unique ID generation for better trash management.
- `fzf`     : for listing, searching through and selecting trashed items.

## Installation

```bash
git clone https://github.com/tmpstpdwn/trashx.git
cd trashx
mv src/trashx ~/.local/bin
```

- Make sure that `~/.local/bin` is in `$PATH`.

## Usage

``` bash
Usage: trashx <Action> <Arg>

Action         | Arg
----------------------------------------------------------------------------
  -t, --trash  | <path1> <path2> ... : Move a file or directory to the trash
  -e, --empty  |                     : Empty the trash
  -l, --list   |                     : List the contents of the trash
  -h, --help   |                     : Show this help message

```

- This program uses fzf to interface with trashed data.
- You can use `--list` action to view, search and restore trashed data via fzf.
- Following are the fzf keybindings.

| Key Combo   | Description                                   |
|-------------|-----------------------------------------------|
| `Ctrl + T`  | Toggle selection of the current item          |
| `Ctrl + I`  | Toggle selection of **all** items             |
| `Ctrl + A`  | Select **all** items                          |
| `Ctrl + D`  | Deselect **all** items                        |
| `Esc`       | Exit without making a selection               |
| `Enter`     | Restore current selection(s) if there are any |

## License

This project is licensed under the MIT [LICENSE](LICENSE).
