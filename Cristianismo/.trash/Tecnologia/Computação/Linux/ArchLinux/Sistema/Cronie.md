### Serviços

1. **O *Anacron*** que executa os scripts cujo prazo de repetição é em dias, no caso o *Anacron* vai executar o que deveria ser executado se baseando em quando foi executado pela última vez, ou seja, se não foi executado, mas deveria, ele vai o fazer
2. **E o próprio *Cronie***, que é usaado para os serviços executados com base em configuração de minuto, hora, dia do mês, mês do ano e dia da semana de 0 a 6, respectivamente.

**Configuração dos *jobs*:**
1. ***Anacron:*** *script* -> */etc/anacrontab*
2. ***Cronie:*** *scripts* no diretório -> */etc/cron.d/*

### Diretórios de Scripts a Serem Periodicamente Executados por Padrão

**Por padrão pelo *Cronie*:**
1.  */etc/cron.hourly*

**Por padrão pelo *Anacron*:**
2. */etc/cron.daily*
3. */etc/cron.monthly*
4. */etc/cron.weekly*

# OBS
Os arquivos de script (não inclui os de configuração) têm de estar executáveis para funcionarem