# Atom Editor Configuration

This repository contains my personal Atom editor configuration.

## Usage

It is composed of 2 files:
* [`config.cson`](./config.cson) - this file specifies the settings.
* [`package.list`](./package.list) - this file specifies the list of packages installed.

### 1. Settings

To restore the settings simply replace the `~/.atom/config.cson` file.

### 2. Packages

#### Get a list of packages from an Atom installation

1. Create a file containing the list of packages installed, run:
```bash
apm list --installed --bare > ~/.atom/package.list
```
2. Copy the file into the destination:
```bash
cp -a ~/.atom/package.list .
```
#### Restore the packages to an Atom installation

To restore the packages, add `package.list` to the `~/.atom` directory and run:

```bash
apm install --packages-file ~/.atom/package.list
```
