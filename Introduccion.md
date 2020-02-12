# Virtualización legera o por contenedores
Común en sistemas Solaris o FreeBSD desde hace años. Todas las máquinas virtuales utilizan el kérnel del anfitrión.

En Linux durante mucho tiempo que quiso hacer una aplicación para hacer contenedores, pero con grandes limitaciones porque no se consigue implementar en el kernel. Hasta que se desarrolló los espacios de nombre en el kernel (namespaces) y creando los grupos de control ya se tenía las herramientas para desarrollar aplicaciones de contenedores en linux: lxc (de linux), systemd-nspawn (los de systemd).

LXC para controlar los contenedores en bruto. LXD maneja los mismo contenedores pero en vez de utilizar el fichero de almacenamiento del anfitrion utiliza un ficheros de imagen, como docker. 

Una de las ventajas de LXC frente a una máquina virtual es para ahorrarse la reserva de los recursos de la máquina anfitriona. No compite con Docker porque son cosas diferentes, no son para despliegue, etc. 

Los ficheros de los contenedores se encuentrasn en **/var/lib/lxc/...**.
