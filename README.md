# controlies
Actualización de controlies servidor para ejecutarse en una máquina independiente (real o virtual) con Debian Jessie  y paquetes controlies-client para funcionar tanto con equipos clientes con Ubuntu 18 como con Ubuntu 22 con el nuevo paquete para el servidor.

**Aviso**: aunque han sido probados dentro de mis posibilidades no es descartable que todavía tengan fallos o que, dada la casuística de los distintos servidores ldap que tenemos, haya cosas que no están contempladas. Se recomienda antes de instalar el paquete controlies servidor hacer backup de:

- La BBDD ldap: script de Esteban Navas para [hacer backup](https://github.com/algodelinux/backup-ldap) y [restaurar](https://github.com/algodelinux/restore-ldap).
- La BBDD SQLite de controlies: ficheros contenidos en la ruta /var/web2py/applications/controlies/databases del servidor.

**Paquetes**:

- **controlies_0.8.0-2_all.deb**: Paquete para instalar en el servidor (Debian Jessie). Front-end web de gestión para ldap, el seguimiento de los clientes de la red y la importación de usuarios desde Rayuela.
- **controlies-client_0.7.1.deb**: Paquete controlies para instalar en clientes con Xubuntu 18.
- **controlies-client_0.8.1_all.deb**: Paquete controlies para instalar en clientes con Xubuntu 22.
    - **pkpgcounter_3.60_all.deb**: Paquete pkpgcounter para instalar en Xubuntu 22 y Debian 11 Bullseye, ya que el antiguo paquete pkpgcounter ha dejado de funcionar y ya no lo mantiene nadie en los repositorios.

Manual de instalación y explotación: manual (***en proceso de desarrollo, todavía no está completo***) de instalación y uso de la aplicación controlies tanto para el servidor como para las máquinas clientes.
- [Manual de controlies](https://docs.google.com/document/d/1RENFd7v7fPgS3N-Zu4oKzo5c-2wSlLZfDexFtMpegrs).

Guia para descomprimir los paquetes y acceder al código fuente: 
- [Como descomprimir y modificar un paquete .deb](http://2tazasdelinux.blogspot.com/2015/06/descomprimir-modificar-y-comprimir-un.html).

Out!
