# Yocto / OpenEmbedded Layer for Google Noto fonts.

This layer aims to allow installing only specific font styles, since you may not want to install all available fonts due to disk space requirements.

## Dependencies

OE-Core only. The recipes will simply install fonts into the filesystem. You may wish to install graphical applications that can display these fonts however.

## Features
* Separate package for every font style for granularity and disk space savings
* Only downloads the files for the fonts you want, not the full >1GB font package

## Todos
* [ ] Set up packaging system for CJK fonts (they don't follow the 4 width x n weights convention) : https://www.google.com/get/noto/help/cjk/
* [ ] Add rest of the fonts
* [ ] Set up packagegroups for commonly used groups
* [ ] Submit layer to layers.openembedded.org
* [ ] Test against multiple yocto releases, perhaps set up branches
* [ ] CI against Yocto / OE-Core

## Bugs, Fixes, etc

Please submit a pull request for any bugs or improvements.
I am especially looking for an example on how to implement CI for a layer (most CI stuff I find for Yocto is for testing end product, not a publicly-available layer).

