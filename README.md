# archlive

Custom Arch Linux Live Images

## Building

After installing [Archiso](https://wiki.archlinux.org/index.php/Archiso), copy the `airootfs/etc/pacman.d/custom_repo/` directory to `/etc/pacman.d/`.  Then run:

```
# mkarchiso -v -w /tmp/archiso-tmp .
```

## Upgrading

- Copy files from `/usr/share/archiso/configs/releng/`

## Included Packages

- [Google Chrome](https://aur.archlinux.org/packages/google-chrome/)
- [Teamviewer](https://aur.archlinux.org/packages/teamviewer/)
- [Alfa AWUS036AC Wireless Adapter Drivers](https://aur.archlinux.org/packages/rtl88xxau-aircrack-dkms-git/)
