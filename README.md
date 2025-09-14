# Trashx - A simple trash management tool.

`trashx` is a simple trash management tool for trashing, listing, and restoring files.

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

"Usage: trashx <Action> <Arg>                                                 "

"Action         | Arg                                                         "
"---------------------------------------------------------------------------- "
"  -t, --trash  | <path1> <path2> ... : Move a file or directory to the trash "
"  -e, --empty  |                     : Empty the trash                       "
"  -l, --list   |                     : List the contents of the trash        "
"  -h, --help   |                     : Show this help message                "

```

## License

This project is licensed under the MIT [LICENSE](LICENSE).
