1. "iwctl" para entrar na interface "iwd"
2. "device list" dentro do "iwd" para ver os dispositivos, comum o correto ser "wlan0", esse será o dispositivo
3. "station $dispositivo scan" para procurar redes
4. "station $dispositivo get-networks" para ver os nomes das redes que foram encontradas
5. "station $dispositivo connect $SSID" (SSID = nome) para conectar a uma rede