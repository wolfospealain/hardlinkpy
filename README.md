# Hardlink
Scan for and hardlink identical files.

## Install (Linux)
```sudo python3 ./hardlink.py --install```

## Usage

```
usage: hardlink.py [-h] [--install] [-d] [-f] [-n] [-p] [-P] [-q] [-o]
                   [-s MINIMUM_SIZE] [-S MAXIMUM_SIZE] [-T] [-v LEVEL]
                   [-x REGEX] [-m PATTERN]
                   [directories [directories ...]]

hardlink.py version 18.07. Scan for and hardlink identical files.

positional arguments:
  directories           one or more search directories

optional arguments:
  -h, --help            show this help message and exit
  --install             install to Linux destination path (default:
                        /usr/local/bin)
  -d, --debug           debugging mode
  -f, --filenames-equal
                        filenames have to be identical
  -n, --dry-run         dry-run only, no changes to files
  -p, --print-previous  output list of previously created hardlinks
  -P, --properties      file properties have to match
  -q, --no-stats        skip printing statistics
  -o, --output          output list of hardlinked files
  -s MINIMUM_SIZE, --min-size MINIMUM_SIZE
                        minimum file size
  -S MAXIMUM_SIZE, --max-size MAXIMUM_SIZE
                        maximum file size
  -T, --timestamp       file modification times have to be identical
  -v LEVEL, --verbose LEVEL
                        verbosity level (0, 1 default, 2, 3)
  -x REGEX, --exclude REGEX
                        regular expression used to exclude files/dirs (may
                        specify multiple times)
  -m PATTERN, --match PATTERN
                        shell pattern used to match files
```

## Compatibility

Tested on Linux.
