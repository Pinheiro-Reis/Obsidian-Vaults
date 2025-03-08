1. **edit the GRUB parameters:**

```
# vim /etc/default/grub
```

2. **comment GRUB_DEFAULT=0**
3. **put this below:**

> GRUB_DEFAULT=*advanced_submenu_id*>*kernel_id*

you can discover this IDs with:

```
# grep gnulinux /boot/grub/grub.cfg
```

For example (look the marked sentences):

---
set default="gnulinux-advanced-a33299fc-c52f-4cc3-8a3b-d00fd0d73b76>gnulinux-linux-advanced-a33299fc-c52f-4cc3-8a3b-d00fd0d73b76"
menuentry 'Arch Linux' --class arch --class gnu-linux --class gnu --class os $menuentry_id_option 'gnulinux-simple-a33299fc-c52f-4cc3-8a3b-d00fd0d73b76' {
submenu 'Advanced options for Arch Linux' $menuentry_id_option '==gnulinux-advanced-a33299fc-c52f-4cc3-8a3b-d00fd0d73b76==' {
	menuentry 'Arch Linux, with Linux linux-lts' --class arch --class gnu-linux --class gnu --class os $menuentry_id_option 'gnulinux-linux-lts-advanced-a33299fc-c52f-4cc3-8a3b-d00fd0d73b76' {
	menuentry 'Arch Linux, with Linux linux-lts (fallback initramfs)' --class arch --class gnu-linux --class  gnu --class os $menuentry_id_option 'gnulinux-linux-lts-fallback-a33299fc-c52f-4cc3-8a3b-d00fd0d73b76' {
	menuentry 'Arch Linux, with Linux linux' --class arch --class gnu-linux --class gnu --class os $menuentry_id_option '==gnulinux-linux-advanced-a33299fc-c52f-4cc3-8a3b-d00fd0d73b76==' {
	menuentry 'Arch Linux, with Linux linux (fallback initramfs)' --class arch --class gnu-linux --class gnu --class os $menuentry_id_option 'gnulinux-linux-fallback-a33299fc-c52f-4cc3-8a3b-d00fd0d73b76' { 

---


4. **run:**

```
# grub-mkconfig -o /boot/grub/grub.cfg
```

or, if you've the alias:

```
# update-grub
```

5. **reboot and test**