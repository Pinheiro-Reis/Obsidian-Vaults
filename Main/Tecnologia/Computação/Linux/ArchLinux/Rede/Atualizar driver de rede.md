 **1. instalando o driver do AUR (altera o AUR helper se você utiliza outro)**

> yay -S < driver novo >

**2. Bloqueando a versão que vem no kernel**

> echo 'blacklist < driver velho >' | sudo tee -a '/etc/modprobe.d/blacklist.conf'`

**3. Reinicie o sistema**

**R1. caso de algum problema, para reverter o processo:**

> sudo pacman -R < driver novo >

**R2. removendo o driver do blacklist**

> sudo rm -rf /etc/modprobe.d/blacklist.conf