# fabsetup-theno-termdown

Install or update termdown.

This is a fabsetup addon.

## Usage

```bash
# task info
fabsetup -d theno.termdown

# run task
fabsetup theno.termdown
```

## Installation

As a pypi package with command pip (recommended way):

```bash
pip install  fabsetup-theno-termdown
```

Or as a git repository checkout:

```bash
mkdir -p ~/.fabsetup-addon-repos
git clone https://github.com/theno/fabsetup-theno-termdown.git  ~/.fabsetup-addon-repos/fabsetup-theno-termdown

# now, fabsetup loads the addon
fabsetup -d theno.termdown

# you can also run the task directly
cd ~/.fabsetup-addon-repos/fabsetup-theno-termdown
fab -d theno.termdown

# or from a checked out fabsetup repo
cd ~/.fabsetup
fab -d theno.termdown
```

## Development

https://github.com/theno/fabsetup/blob/master/howtos/fabsetup-addon.md

```bash
# save changes
git commit -am 'I describe my changes'

# upload to github
git push origin master

# update version number in fabsetup_theno_termdown

# create and publish package at pypi
fab -f fabfile-dev.py  pypi

# clean up
fab -f fabfile-dev.py  clean
```
