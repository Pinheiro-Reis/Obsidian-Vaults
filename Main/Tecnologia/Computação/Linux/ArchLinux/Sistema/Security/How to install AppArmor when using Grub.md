https://youtu.be/-3W2f_JL3yw?si=m7I64g19iNgqxaGk

1. **insert the GRUB parameters to enable AppArmor on Boot**

**File: /etc/default/grub**
   1   │ # GRUB boot loader configuration
   2   │ 
   3   │ GRUB_DEFAULT=0
   4   │ GRUB_TIMEOUT=5
   5   │ GRUB_DISTRIBUTOR="Arch"
   6   │ GRUB_CMDLINE_LINUX_DEFAULT="loglevel=3 quiet audit=1 lsm=landlock,lockdown,yama,integrity,apparmor,bpf"
   7   │ GRUB_CMDLINE_LINUX=""

2. **reload GRUB configs**

> sudo grub-mkconfig -o /boot/grub/grub.cfg

3. install the AppArmor

> sudo pacman -S apparmor

4. enble the AppArmor service

> sudo systemctl enable apparmor

5. Reboot and verify with:

> aa-enabled