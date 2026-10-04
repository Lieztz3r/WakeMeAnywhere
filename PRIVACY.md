# Política de privacidad — Wake Me Anywhere

*Vigente desde el 3 de octubre de 2026.*

Wake Me Anywhere es una alarma por ubicación. Funciona sin cuentas, sin anuncios, sin analítica y
sin Google Play Services. Esta política explica qué datos usa la app y adónde van.

## Datos que se quedan en tu teléfono

- **Ubicación.** La app lee la ubicación del teléfono (GPS y red) para saber cuándo llegas a un
  destino o sales de él, incluso con la pantalla apagada. El seguimiento que activa las alarmas se
  procesa en el teléfono. No se envía una ruta de viaje al desarrollador.
- **Alarmas, favoritos, historial y ajustes.** Se guardan en el almacenamiento privado de la app.
  No se incluyen en los respaldos en la nube de Android. Solo salen del teléfono si tú los
  exportas a un archivo.

## Servicios externos que usa la app

| Servicio | Cuándo | Qué recibe |
|---|---|---|
| [OpenFreeMap](https://openfreemap.org) | Al mostrar o mover el mapa | Solicitudes de teselas para las zonas visibles y la dirección IP del teléfono |
| [Nominatim de OpenStreetMap](https://nominatim.org) | Cuando buscas un lugar o pides el nombre de un punto del mapa | El texto de búsqueda y, si está disponible, una zona aproximada alrededor de tu posición para ordenar resultados; al pedir el nombre de un punto sin etiqueta, sus coordenadas. También recibe la dirección IP ([su política](https://osmfoundation.org/wiki/Privacy_Policy)) |
| [ntfy](https://ntfy.sh) u otro servidor que elijas | Solo si activas *Compartir ubicación en vivo* o sigues a otra persona | En el caso de compartir, tu posición **cifrada de extremo a extremo** (AES-256-GCM), un tema aleatorio y la dirección IP. El servidor no puede leer la posición, pero sí ve metadatos de conexión y mensajes cifrados. Las personas con las que compartes necesitan la invitación para descifrarla |

El desarrollador no recibe estas solicitudes ni mantiene una cuenta o servidor de usuarios. Los
proveedores anteriores reciben los datos descritos cuando usas esas funciones.

## Compartir ubicación en vivo

Es opcional y se activa a mano. Tú decides con quién compartir (mandando la invitación) y durante
cuánto tiempo. *Nueva llave* invalida todas las invitaciones anteriores. Desactivar el
compartir detiene el envío de inmediato. Las posiciones compartidas se cifran en el dispositivo
antes de enviarse; el servidor de relevo aún puede observar la IP, el tema aleatorio, los tiempos y
el tamaño de los mensajes cifrados.

## Permisos

- **Ubicación (también en segundo plano):** para que la alarma suene aunque la app esté cerrada o
  la pantalla apagada.
- **Notificaciones, pantalla completa y alarmas exactas:** para mostrar y hacer sonar la alarma
  sobre la pantalla de bloqueo.
- **Internet:** para el mapa, la búsqueda y la ubicación en vivo.
- **Linterna, vibración e iniciar al encender:** para despertarte y para reanudar las alarmas
  armadas después de reiniciar el teléfono.

## Niños

La app no está diseñada específicamente para menores. La ubicación es un dato sensible de Android:
el seguimiento del viaje se procesa en el teléfono, pero las búsquedas y los nombres de puntos
pueden enviar los datos indicados arriba a OpenStreetMap/Nominatim. No se debe seleccionar un
público objetivo ni completar declaraciones de privacidad en Google Play sin revisar las prácticas
de todas las funciones y servicios externos.

## Borrar tus datos

Desinstalar la app borra todos sus datos del teléfono. Como el desarrollador no guarda datos tuyos,
no hay nada más que borrar.

## Contacto y cambios

Preguntas o solicitudes: abre un issue en
<https://github.com/Lieztz3r/WakeMeAnywhere/issues>.
Si esta política cambia, se publicará aquí con una nueva fecha.
