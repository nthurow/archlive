# archlive

Custom Arch Linux Live Images

## Building

After installing [Archiso](https://wiki.archlinux.org/index.php/Archiso), copy the `airootfs/etc/pacman.d/custom_repo/` directory to `/etc/pacman.d/`.  Then run:

```
# mkarchiso -v -w /tmp/archiso-tmp .
```

## Upgrading

- Copy files from `/usr/share/archiso/configs/releng/`
- Upgrade custom built packages:
    - Remove old packages from repo: `repo-remove ./airootfs/etc/pacman.d/custom_repo/custom.db.tar google-chrome rtl88xxau-aircrack-dkms-git teamviewer`
    - Remove old packages from local repo: `sudo repo-remove /etc/pacman.d/custom_repo/custom.db.tar google-chrome rtl88xxau-aircrack-dkms-git teamviewer`
    - Remove old package files from `./airootfs/etc/pacman.d/custom_repo`
    - Remove old package files from `/etc/pacman.d/custom_repo`
    - Copy the packages to `./airootfs/etc/pacman.d/custom_repo` and `/etc/pacman.d/custom_repo`
    - Run `repo-add ./airootfs/etc/pacman.d/custom_repo/custom.db.tar ./airootfs/etc/pacman.d/custom_repo/*.pkg.tar*`
    - Run `sudo repo-add /etc/pacman.d/custom_repo/custom.db.tar /etc/pacman.d/custom_repo/*.pkg.tar*`

## Included Packages

- [Google Chrome](https://aur.archlinux.org/packages/google-chrome/)
- [Teamviewer](https://aur.archlinux.org/packages/teamviewer/)
- [Alfa AWUS036AC Wireless Adapter Drivers](https://aur.archlinux.org/packages/rtl88xxau-aircrack-dkms-git/)
