# Trashx - A simple trash management tool.

`trashx` is a simple trash management system for trashing, deleting, listing, and restoring files.

## Dependancies

- `uuidgen` : for unique ID generation for better trash management.
- `csvlens` : for a prettyfied view of trash data.

## Installation

```bash
git clone https://github.com/tmpstpdwn/trashx.git
cd trashx
mv src/trashx ~/.local/bin
```

- Make sure that `~/.local/bin` is in `$PATH`.

## Usage

``` bash
Usage: trashx <command> [<args>]

Commands:
  -t, --trash   : Move a file or directory to the trash
            Example: trashx -t / --trash myfile.txt
  -e, --empty   : Empty the trash
            Example: trashx -e / empty
  -l, --list    : List the contents of the trash
            Example: trashx -l / --list
  -r, --restore : Restore a file from the trash
            Example: trashx -r / --restore
  -h, --help, * : Show this help message

Note: only -t, --trash command have an argument which
      can be a file or folder path to trash.
```

Example:

``` bash
trashx -t $HOME/Pictures/Screenshots/desktop.png
```

## License

This project is licensed under the GPL3 [LICENSE](LICENSE).
