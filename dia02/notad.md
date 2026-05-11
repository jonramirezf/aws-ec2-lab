Modelo ML
aprende patrones usando datos para hacer predicciones 
ej:
ventas,spam,fraude,recomendaciones
Los modelos Ml a veces son "caja negra" la empresa pregunta por que dijo eso?
aca aparece el pdp 

PDP: 
Gráfico de dependencia parcial (Partial Dependence plot)
Función:
“Un PDP es un gráfico que muestra de manera transparente cómo una variable influye en la predicción de un modelo ML.”
Ejemplo de Ml y pdp juntos 
Modelo ML:
predice ventas.

PDP:
muestra si la temperatura aumenta o disminuye las ventas.

finalizar
 Modelo ML  hace predicciones aprendiendo de datos.
PDP  gráfico que ayuda a explicar esas predicciones.
__________________________________________________________________________________________________________________________

CDN: Red de entrega de contenido, Un CDN es un sistema de servidores distribuidos por el mundo que entregan contenido desde el servidor mas
cercano al usuario. 
asi:Carga mas rapida, baja latencia, mejora de video, imagenes y paginas web
CDN entrega contenido desde servidores cercanos para reducir la latencia.
ejemplo: Sin cdn chile cl pide un video a EE.UU us , tarda mas , con cdn video ya guardado servirdor cercano, carga rapido

Amazon cloud front:
Es el servicio CDN de AWS.
Entrega contenido globalmente con baja latencia usando servidores cercanos al usuario.
CloudFront = CDN rápido global
Distribuye contenido rápidamente a usuarios de todo el mundo usando servidores cercanos llamados edge locations.
que entrega cloudfront videos, imagenes,paginas web,archivos,Apis.
Objetivo:reducir latencia 
Edge Locations:Servidores distribuidos globalmente
ejemplo:Empresas con usuarios en chile,japon,alemania con cloudfront cada usuario recibe contenido desde una ubiacion cercana 
CloudFront acelera la entrega global de videos, imágenes y contenido web con baja latencia.
_______________________________________________________________________________________________________________________________

Fiabilidad:Reability 

Es la capacidad del sistema de:
-recuperarse de fallos
-interrupciones
-seguir funcionando
-adaptarse a la demanda
-adquirir recursos dinamicamente 
todo esto es del pilar de la fiabilidad 
ejemplo una aplicación tiene miles de usuarios un servidor falla AWS automaticamente:
remplaza servidores,redire trafico,escala recursos el sistema sigue funcionando

auto scaling: 
adquirir dinámicamente recursos computacionales:aumentar recursos automáticamente cuando sube demanda.
Capacidad de un sistema para recuperarse de fallos y adaptarse automáticamente a la demanda.

AWS Well-Architected Framework es una guía de buenas prácticas para crear arquitecturas seguras, confiables, eficientes y optimizadas en AWS.
Los 6 pilares principales

Security = proteger /Protección de datos, accesos, cifrado, permisos
Reliability = recuperarse /Recuperación de fallos, alta disponibilidad, escalado automático
Performance = eficiencia tecnológica /Tecnologías modernas, rendimiento, serverless, recursos eficientes
Cost = ahorrar /Ahorrar dinero, reducir gastos innecesarios
Operational = operar/mejorar /Automatización, monitoreo, mejoras continuas, operaciones
Sustainability = ecológico /Reducir consumo y impacto ambiental

Migrar a AWS mejora la resiliencia operativa y la agilidad empresarial.
---------------------------------------------------------------------------------------------------------------------------------------
Serverless = no gestionar servidores

AWS Organizations: es un servicio para administrar múltiples cuentas AWS centralizadamente.
Organizations = varias cuentas AWS juntas
----------------------------------------------------------------------------------------------------------------------------------------
Una región AWS es un área geográfica que contiene múltiples Availability Zones
ejemplo region Sao Paulo br
dentro hay :
-sa-east 1a
-sa-east-1b
-sa-east-1c 
Cada una tiene datacenters , energia rebundante,red rebundante
Redundancia significa tener sistemas duplicados o replicados para evitar fallos.
___________________________________________________________________________________________________________________________________________
AWS Lambda
Qué es Lambda?

Lambda es un servicio serverless de AWS, Permite ejecutar código sin administrar servidores.
subes codigo lamdba lo ejecuta automaticamente.

AWS administra servidores , escalado , infraestructura, disponibilidad 
AWS Lambda ejecuta código sin que el usuario administre servidores.
Lambda normalmente funciona por:
archivo en Amazon S3
petición API
cambio en base de datos
mensaje en cola

¿Qué administra AWS?

WS maneja:
servidores,
sistema operativo,
escalado,
disponibilidad,
infraestructura.

¿Qué administra la empresa?

La empresa:
escribe código,
configura permisos,
define memoria/timeout,
monitorea funciones.

La empresa debe:
evitar vulnerabilidades,
validar entradas,
proteger la aplicación.
----------------------------------------------------------------------------------------------------------------------------------------
soluciones de recuperación ante desastres (DR) para instancias Amazon EC2.
AMI = recuperar servidor
Snapshot = recuperar datos
Amazon Machine Image (AMI): Una AMI es una plantilla usada para crear y recuperar instancias EC2 rápidamente.AMI = clonar/recrear EC2


Amazon Elastic Block Store Snapshots:una copia de seguridad (backup) de un volumen EBS.
EBS = Elastic Block Store , Es el disco duro de una instancia:


AMI	Plantilla completa de EC2	SO + configuración + apps + discos asociados	Crear o clonar instancias EC2
 EBS Snapshot	Backup de un volumen EBS	Solo datos del disco	Restaurar datos o discos