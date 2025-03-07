**1. para instalar todas as coisas importantes relacionadas:**

> sudo pacman -S pipewire lib32-pipewire pipewire-audio pipewire-pulse pipewire-jack pipewire-alsa qjackctl

e

> systemctl enable pipewire

> systemctl start pipewire

depois [[Instalar Easy Effects Junto Com as Dependências]]

**2. dar reboot**

**3. conferir:**

> systemctl --user list-units | grep pipewire

ou/e

> systemctl --user status pipewire-pulse

ou/e

> systemctl --user status pipewire-audio      

e

> pactl list sinks