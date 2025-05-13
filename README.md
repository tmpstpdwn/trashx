# Trashx - A simple trash management tool.

`trashx` is a simple trash management tool for trashing, listing, and restoring files.

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
                 Example: trashx -t myfile.txt
  -e, --empty   : Empty the trash
                 Example: trashx -e
  -l, --list    : List the contents of the trash
                 Example: trashx -l
  -r, --restore : Restore a file from the trash
                 Example: trashx -r
  -h, --help    : Show this help message
```

## License

This project is licensed under the GPL3 [LICENSE](LICENSE).
