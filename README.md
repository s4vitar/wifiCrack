# wifiCrack

Herramienta ideal para automatizar ataques WiFi (WPA/WPA2 - PSK) destinados a la obtención de la contraseña.

Esta herramienta nos la fuimos desarrollando en un directo que hice en Twitch, a petición de los espectadores decidimos subirlo como repositorio para que todos se la pudieran descargar.

Puedes ver el vídeo completo aquí, donde nos desarrollamos la herramienta paso a paso:

* [https://www.youtube.com/watch?v=Mwt_RbdpJhk](https://www.youtube.com/watch?v=Mwt_RbdpJhk)

La herramienta **wifiCrack** cuenta con 2 modos de ataque. El primero de ellos es el ataque **Handshake**, donde de manera automatizada, se gestiona todo lo necesario para mediante un ataque clásico de de-autenticación y reconexión por parte de una estación, se obtenga un Handshake válido con el que posteriormente poder trabajar para aplicar fuerza bruta.

El segundo modo de ataque, es el **PKMID ClientLess Attack**, que centra su atención en las redes inalámbricas que no disponen de clientes asociados (Método Moderno).

## ¿Cómo se ejecuta la herramienta?

Buena pregunta Mike. Pues bueno... la herramienta cuenta con 2 parámetros, por un lado el parámetro '**-a**' para especificar el modo de ataque (Handshake|PKMID) y por otro lado el parámetro **-n** para especificar el nombre de la tarjeta de red.

De todas formas, la herramienta cuenta con un panel de ayuda tras su ejecución:

```bash
┌─[root@parrot]─[/home/s4vitar/Desktop/Directo]
└──╼ #./s4viPwnWifi.sh 

[*] Uso: ./s4viPwnWifi.sh

        a) Modo de ataque
                Handshake
                PKMID
        n) Nombre de la tarjeta de red
        h) Mostrar este panel de ayuda
```

Ya con estos parámetros definidos, en función del modo de ataque seleccionado... se desplegará todo lo necesario de forma automática.

