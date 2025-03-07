## Para instalar a fonte:

> sudo pacman -S font_name

e depois, para verificar se foi instalada:

> fc-list | cut -d: -f2 | sort | uniq

e, se deu certo:

> fc-cache

certamente ele a instalou em um diretório em */usr/share/fonts/*

## Para habilitar a fonte

na interface GNOME há como fazer, nas preferências

