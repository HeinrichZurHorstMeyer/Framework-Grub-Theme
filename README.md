# Framework-Grub-Theme
A GRUB2 Theme for Framework laptops

## Installation
Clone the repository into a normal directory:
```
$ git clone https://github.com/HeinrichZurHorstMeyer/Framework-Grub-Theme.git
```

Copy the folders to `/boot/grub/themes/`:
```
# cp -r Framework-Grub-Theme/Framework-Arch /boot/grub/themes/
# cp -r Framework-Grub-Theme/Framework /boot/grub/themes/
```

Change the GRUB theme by setting `GRUB_THEME` in `/etc/default/grub` :
```
# nvim /etc/default/grub
```
_With Arch-Logo:_
```
GRUB_THEME="/boot/grub/themes/Framework-Arch/theme.txt"
```
_Without Arch-Logo:_
```
GRUB_THEME="/boot/grub/themes/Framework/theme.txt"
```

Rebuild the `grub.cfg`:
```
# grub-mkconfig -o /boot/grub/grub.cfg
```

Reboot to see the changes:
```
$ reboot
```

## Editing
Feel free to edit the Krita file in `sources`.
