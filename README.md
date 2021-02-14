# DEPRECATED

This repository is now archived, since the command with the same name and functionality if now distributed with Homebrew by default.

# `brew autoremove`

This repository provides a command for [Homebrew](https://brew.sh) to list and
remove all formulae that were installed as dependencies at some point and are
not needed anymore.

## Usage

```
brew autoremove
```

It will show you the list of formuale to be removed and ask for confirmation.

Options:

* `-f|--force` - do not ask for confirmation before running `brew rm`
* `-l|--list` - do not remove anything, just print the list of formulae that are
  not depended on anymore.

If you see some formula in the output that you'd like to keep, run `brew install`
on it and then re-run `brew autoremove`. `brew install` will tell you that the
formula is already installed, but still update the metadata to state that you
requested it to be installed.

## Installing

```sh
brew tap gelraen/autoremove
```

