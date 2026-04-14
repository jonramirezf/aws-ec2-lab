# Día 1 - Primer despliegue en AWS EC2

Hoy hice mi primer laboratorio en AWS creando una instancia EC2 desde cero.

Seleccioné Amazon Linux 2023 como sistema operativo y una instancia t3.micro para mantenerme dentro del Free Tier. También generé un par de claves (.pem) para poder conectarme de forma segura.

Después de lanzar la instancia, me conecté usando EC2 Instance Connect desde el navegador. Ya dentro del servidor, probé comandos básicos de Linux como `ls`, `whoami` y `pwd` para entender el entorno.

Intenté iniciar el servicio httpd, pero me apareció un error porque no estaba instalado. Esto me ayudó a entender mejor el proceso, ya que primero hay que instalar el servicio antes de iniciarlo. Luego lo instalé correctamente.

También aprendí la diferencia entre IP pública e IP privada, y cuándo usar cada una.

Finalmente, por seguridad y para evitar costos, eliminé la instancia.

Este laboratorio me ayudó a entender en la práctica cómo funciona IaaS usando EC2, además de reforzar conceptos básicos de Linux y cloud.
