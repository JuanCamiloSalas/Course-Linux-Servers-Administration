# 1. Introducción a los servidores
## 1.1. Iniciar en el mundo de los servidores Linux
### ¿Por qué aprender Linux?
Los conocimientos en Linux son de los requisitos más demandados.

### ¿Qué necesito saber para tomar el curso?
- [*Importante*] Conceptos básicos de ingeniería de software.
- [*Importante*] Manejo básico de la terminal.
- [*Opcional*] Saber Shell o Python.
- [*Opcional*] Conocimiento de redes computacionales.

### ¿Linux es poco usado?
Falso, 80% de los servidores lo usan, supercomputadoras y casi todos los servidores en la nube.

### ¿Qué conocimientos tendré al finalizar el curso?
- Conocerás los diferentes tipos de servidores.
- Sabrás los conceptos clave de un sistema Linux.
- Sabrás administrar de manera básica un servidor Linux.
- Tendrás los conocimientos de como funciona el sistema por dentro.

## 1.2. Habilidades y roles de un administrador
### Habilidades clave
- Control de accesos.
- Monitoreo del sistema.
- Administración de recursos.
- Troubleshooting.
- Instalación y mantenimiento de software.
- Creación de respaldos.
- Documentación.

### Roles que se pueden desempeñar:
- DevOps Engineer: Se enfocan en los procesos y metodologías para la correcta liberación en el proceso de desarrollo de software.

- Site Reliability Engineer: Se enfocan en que los sistemas de software operen de manera correcta y con el mayor grado de confiabilidad posible.

- Security Operations Engineer: Encargados de mantener la seguridad de los sistemas a nivel de red y aplicaciones.

- Algunos otros roles:
    - Network Engineer.
    - Database Administrator.
    - Network Operation Center Engineer.
    - MLOps Engineer.
    - Cloud Engineer.

## 1.3. ¿Qué son los servidores?
Un servidor es un **grupo de recursos tecnológicos** (hardware y software) que cumplen con uno o varios propósitos. Estos usualmente reciben **peticiones de un cliente** y luego otorgan una **respuesta**.

**Algunos tipos de servidores:**
- Web (frontend, backend).
- Bases de datos.
- De pruebas.
- Videojuegos.
- Medios.
- Email.
- Impresión.
- Archivos y recursos (SFTP, SMB).
- VoIP.
y existen muchos mas...


## 1.4. ¿Qué es un sistema Linux/UNIX?
### ¿Qué es un Sistema Operativo?

En la clase anterior exploramos el concepto de servidor y sus distintos tipos. Ahora nos adentraremos en el mundo de los sistemas operativos, empezando por entender qué es un sistema en sí mismo.

### El Kernel: Corazón del Sistema

El término "Linux" hace referencia al kernel de un sistema operativo. ¿Qué es un kernel? Esencialmente, actúa como el corazón de cualquier sistema operativo, facilitando la comunicación entre el hardware y el software. Es el encargado de coordinar y gestionar los recursos del sistema.

### GNU/Linux: Una Asociación Importante

Los sistemas operativos basados en Linux suelen denominarse "GNU/Linux". "GNU" representa un sistema operativo de software libre que se originó en los años 80. Esta asociación abarca toda la capa de aplicaciones del sistema operativo.

### Distribuciones de Linux

Las diferentes versiones de sistemas Linux se conocen como distribuciones. Algunas de las principales son:

- **Red Hat (RHEL):** Conocida como "Red Hat Enterprise Linux".
- **Ubuntu:** Basada en Debian, es una distribución popular para servidores.
- **Debian:** Otra distribución estable y confiable.

Cada distribución tiene sus propias características, ventajas y desventajas, algunas son gratuitas mientras que otras requieren pago.

### Diferencia entre Linux y UNIX

Es común escuchar sobre la diferencia entre sistemas Linux y UNIX. Linux es solo una parte del sistema operativo, mientras que UNIX es un sistema operativo completo. UNIX se desarrolló en 1969 en los Laboratorios Bell de AT&T. Algunas distribuciones de UNIX incluyen FreeBSD y macOS, que utiliza UNIX en parte de su sistema operativo.

## 1.5. Arquitectura de un sistema UNIX/Linux
![Schema](https://th.bing.com/th/id/R.9f8d748414763d71b990301484601acf?rik=KU1cwoRTqpSw6Q&riu=http%3a%2f%2f2.bp.blogspot.com%2f-XxPkuHH1t04%2fVWqJcnamjdI%2fAAAAAAAAB3I%2fL58rK67EcK4%2fs1600%2fEstructuraUnix.png&ehk=hmjmlxLrOtWbs9%2fq9nMkbcHWbmziCHPzwCGTlq8CV9g%3d&risl=&pid=ImgRaw&r=0)


**Capa de Hardware:**
Es la capa central que abarca todos los dispositivos físicos conectados al sistema, como discos, mouse, memoria, procesador y tarjeta de red.

**Capa de Kernel:**
Esta capa es la piedra angular del sistema, controlando todo el hardware y facilitando la comunicación con las capas superiores. Regula aspectos como el uso de la memoria RAM y los ciclos del CPU.

**Capa de Shell:**
Interfaz familiar proveniente del curso de terminal, actúa como un puente entre el kernel y las aplicaciones. Permite enviar instrucciones al kernel y recibir información para su procesamiento.

**Capa de Aplicaciones:**
Es la capa donde interactúa directamente el usuario y los administradores de sistemas. Aquí reside la mayoría del software utilizado, como calculadoras, calendarios, navegadores web y herramientas de utilidad, como comandos para gestionar archivos y realizar copias del sistema.

## 1.6. Breve historia del software libre y el Open Source
![Story line](https://static.platzi.com/media/user_upload/03483589-35105ae1-1941-4ab0-97d7-1871010f7c85.jpg)

### Cuatro libertades del software libre

- 0 - La libertad de ejecutar el programa.
- 1 - La libertad de estudiar el funcionamiento del programa y modificarlo.
- 2 - La libertad de redistribuir.
- 3 - La libertad de distribuir copias de sus versiones modificadas a otras personas.

### OpenSource

El software de código abierto, también conocido como "opensource", comparte similitudes con el software libre en cuanto a la accesibilidad y la transparencia del código fuente. Sin embargo, mientras que el software libre se centra en las libertades de los usuarios, el código abierto se enfoca más en el desarrollo colaborativo y la disponibilidad pública del código fuente. 

Las principales diferencias radican en la filosofía y enfoque: 

- **Filosofía:** El software libre se basa en las cuatro libertades del usuario, mientras que el código abierto se enfoca en la apertura del código para permitir la colaboración y la mejora del software.
  
- **Licencias:** El software libre generalmente se distribuye bajo licencias que enfatizan las libertades del usuario, como la GPL (Licencia Pública General de GNU), mientras que el código abierto puede utilizar una variedad de licencias que permiten diferentes grados de restricción y colaboración.

A pesar de estas diferencias, ambos enfoques comparten el objetivo de promover la libertad, la accesibilidad y la colaboración en el desarrollo de software.

## 1.7. Sistemas operativos y distribuciones
### Distribución
Sistema operativo que interpreta el kernel de Linux, pueden variar en el formato, manejador de paquetes y popularidad.

- **Ubuntu**
- **Red Hat**
- **Debian**
- **FreeBSD**

### Conceptos importantes
- **LTS (Long Term Support):** Garantiza al menos 5 años de soporte para una distribución.
- **Non-free Repositories:** Repositorios de software con licencias no aprobadas por la Debian Free Software Foundation.

### Rolling Release vs. Fixed Release:
**Rolling Release:** Actualizaciones continuas con el riesgo de inestabilidad, se publican al momento de desarrollarse (Arch Linux, Gentoo-based).
- Ventajas: Actualizaciones frecuentes, estabilidad en distribuciones basadas en Red Hat.
- Desventajas: Riesgo de inestabilidad, especialmente en nuevas versiones.

**Fixed Release:** Versiones más estables con actualizaciones probadas y garantizadas (Ubuntu).
- Ventajas: Mayor estabilidad y menos bugs debido a actualizaciones probadas.
- Desventajas: Menos frecuencia de actualizaciones, especialmente en distribuciones gratuitas.

## 1.8. ¿Dónde viven nuestros servidores?
**On premise:** Todo el hardware y software del servidor es alojado y mantenido por la organización. Cloud

**Nube Pública:** Son todos los proveedores de servicios que otorgan recursos de hardware y software para montar los servidores, tales como Google cloud, Azure, AWS, entre otros.

**Nube Privada:** Todos los recursos y software pueden vivir en otro lado pero ningún recurso o servicio se comparte con otra empresa para tener un mayor grado de seguridad. 

**Hybrid (Nube Híbrida):** Es una combinación de servicios on premise y cloud.

## 1.9. Formas de montar un servidor
### Instalación directa
Se instala un sistema operativo para ocupar el 100% de los recursos dedicados (software y hardware) ya sea a un solo servicio o varios.

### Virtualización
Se instala un software que sirve como host conocido como (**hypervisor**) que administra los recursos para crear múltilpes **guests** o versiones virtualizadas.

**Tipos de Hypervisor:**

- Tipo 1 (Bare-metal): Sobre la capa de hardware se monta directamente el hypervisor. (No requiere sistema operativo, se ejecuta directamente en una máquina virtualizada por el hypervisor.)
- Tipo 2: Es más acccesible, sobre el hardware se monta un SO, luego se ejecuta el hypervisor.

Dato curioso: VirtualBox es lo que se denominaría como Hypervisor.
