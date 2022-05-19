# About

This is just a mirror of https://aur.archlinux.org/zig-static.git, with modifications to point to a more recent build of the Zig compiler. I use this to install Zig on my Steam Deck, which runs an ArchLinux distribution.

# How to use

```sh
# clone repository
git clone -b develop https://github.com/code-disaster/aur.zig-static.git zig-static
cd zig-static

# make & install
makepkg
sudo pacman -U zig-static-{version}.zst

# test install
zig version
```
