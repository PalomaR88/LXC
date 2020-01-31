# Virtualización legera o por contenedores
Común en sistemas Solaris o FreeBSD desde hace años. Todas las máquinas virtuales utilizan el kérnel del anfitrión.

En Linux durante mucho tiempo que quiso hacer una aplicación para hacer contenedores, pero con grandes limitaciones porque no se consigue implementar en el kernel. Hasta que se desalló los espacios de nombre en el kernel (namespaces) y creando los grupos de control ya se tenía las herramientas para desarrollar aplicaciones de contenedores en linux: lxc (de linux), systemd-nspawn (los de systemd).
