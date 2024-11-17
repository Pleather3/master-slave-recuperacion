# Práctica de DNS: Maestro y Esclavo con Subdominios

## Descripción

Esta práctica consiste en la configuración de un sistema de DNS utilizando un servidor maestro y un servidor esclavo.
Se utilizarán subdominios para gestionar las peticiones DNS de manera eficiente. 
Las máquinas virtuales se crearán utilizando Vagrant y se basarán en la imagen de Debian Bookworm.

## Configuración del Vagrantfile
Para configurar el Vagrantfile, se crean dos máquinas virtuales usando Debian Bookworm.
 Se establece un tiempo de espera de arranque (vm.boot_timeout) para que, si no se configura en 60 segundos, se produzca un error.


## Configuración del DNS
Iniciar las máquinas virtuales con vagrant up

# Acceder a la máquina maestra:

vagrant ssh dnsa

## Resolución de preguntas
La utilidad que se describe en el contexto es un sistema de DNS (Domain Name System) configurado con un servidor maestro y
 un servidor esclavo, utilizando subdominios. Esta configuración puede ser muy útil para varias aplicaciones y propósitos:

Gestión de nombres de dominio: Permite resolver nombres de dominio a direcciones IP,
                               facilitando el acceso a servicios en línea mediante nombres más fáciles de recordar en lugar de direcciones IP.

Redundancia y disponibilidad: Con un servidor maestro y uno esclavo, se asegura que si el servidor maestro falla,
 el servidor esclavo puede seguir resolviendo las peticiones DNS, lo que aumenta la disponibilidad del servicio.

Organización de subdominios: Permite gestionar múltiples subdominios de manera eficiente,
 lo que es útil para organizaciones que tienen diferentes departamentos o servicios en línea.

Pruebas y aprendizaje: Para estudiantes y profesionales de IT, 
esta configuración es una excelente manera de aprender sobre administración de redes, DNS, y la configuración de servidores.

Respecto a la protección de datos, es importante considerar lo siguiente:

Seguridad de la información: La configuración de DNS debe incluir medidas de seguridad adecuadas, 
como la implementación de DNSSEC (DNS Security Extensions) para proteger contra ataques como el envenenamiento de caché.

Cumplimiento normativo: Dependiendo de la ubicación y el tipo de datos que maneje el sistema, 
se deben seguir regulaciones de protección de datos, como el GDPR en Europa, que establece requisitos sobre la gestión y
 protección de datos personales.

Acceso restringido: Es fundamental controlar quién tiene acceso a la configuración del servidor DNS y 
a los registros de datos, para evitar accesos no autorizados.

En resumen, la utilidad de un sistema de DNS bien configurado es amplia y puede ser muy beneficiosa para la gestión de redes y
 servicios en línea. Sin embargo, es crucial implementar prácticas adecuadas de seguridad y protección de datos para garantizar que se cumplan las normativas y se protejan los datos sensibles.

