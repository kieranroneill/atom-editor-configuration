# Atom Editor Configuration

This repository contains my personal Atom editor configuration.

## Usage

It is composed of 2 files:
* [`config.cson`](./config.cson) - this file specifies the settings.
* [`package.list`](./package.list) - this file specifies the list of packages installed.

### 1. Settings

To restore the settings simply replace the `~/.atom/config.cson` file.

### 2. Packages

To get a file containing the list of packages installed, run:
```bash
apm list --installed --bare > ~/.atom/package.list
```

To restore the packages, add `package.list` to the `~/.atom` directory and run:

```bash
apm install --packages-file ~/.atom/package.list
```
