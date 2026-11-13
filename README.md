# bibmd releases

Prebuilt releases of **bibmd**, a zen Markdown reader that edits a block in place when it
is clicked. Wayland, one Native AOT binary for x86_64 Linux, no runtime.

## Arch Linux

Add the pacman repository to `/etc/pacman.conf`:

```ini
[bibmd]
SigLevel = Optional TrustAll
Server = https://github.com/relu24/bibmd-releases/releases/download/repo
```

then

```sh
sudo pacman -Sy bibmd-bin    # or: yay -S bibmd-bin
```

`pacman -Syu` keeps it up to date. It installs `bibmd` and `md`: `md notes.md` opens (or
creates) a file.

## Other distributions

Download `bibmd-<version>-x86_64.tar.gz` from the [releases](https://github.com/relu24/bibmd-releases/releases)
and put `bibmd` on your PATH. It needs wayland, libxkbcommon, freetype, harfbuzz and fontconfig.

## License

MIT. The embedded iA Writer Mono S font is under the SIL Open Font License (OFL.txt in each tarball).
