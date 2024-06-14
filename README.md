# Trashx - A simple trash management tool.

`trashx` is a simple trash management system for trashing, deleting, listing, and restoring files.

## Why ??

I made this small script to help me manage trash on my system. even though programs already exist for the same, i though it would be a good learning experiance. 
Now i think its at a point where other can use it too.

## Dependancies

- `uuidgen` : for unique ID generation for better trash management.
- `csvlens` : for a prettyfied view of trash data.

## Installation

manually copy/move the script `src/trashx` to a directory under the `$PATH` variable for global access. 

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

## Contributions

Contributions are welcome! Please fork the repository and submit a pull request for any improvements or new features.

## License

This project is licensed under the GPL3 License - see the [LICENSE](LICENSE) file for details.
