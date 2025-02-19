# ping

> Envía paquetes ICMP ECHO_REQUEST (pings) a equipos (hosts) de la red.
> Más información: <https://manned.org/ping>.

- Envía pings a un host:

`ping {{host}}`

- Envía un número determinado de pings a un host:

`ping -c {{numero}} {{host}}`

- Envía pings a un host especificando el intervalo de tiempo entre peticiones (por defecto 1 segundo):

`ping -i {{segundos}} {{host}}`

- Envía pings a un host sin intentar resolver nombres simbólicos de direcciones:

`ping -n {{host}}`

- Envía pings a un host y emite un sonido cuando un paquete es recibido (si la terminal lo soporta):

`ping -a {{host}}`

- Muestra también un mensaje si no se recibió respuesta:

`ping -O {{host}}`

- Envía una cantidad específica de pings (`-c`), con un tiempo límite (`-W`) para cada respuesta, y un tiempo máximo total (`-w`) para la ejecución del ping completo:

`ping -c {{cantidad}} -W {{segundos}} -w {{segundos}} {{host}}`
