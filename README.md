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

![schema](https://miro.medium.com/v2/resize:fit:700/1*0tuVhpzOB-NHLeTjXtBDBw.png)

# 2. Configuración básica de un servidor remoto
Comandos: 

- **ssh:** lo usamos para confirmar que tengamos instalado openssh en el sistema, en caso de no estar instalado podemos instalarlo con el comando:

`sudo apt install openssh`

Para el caso de ubuntu server, o para el caso de RHEL con el comando:

`sudo dnf install openssh`

- **systemctl status sshd:** Para verificar que el proceso de ssh este activo y corriendo en el sistema (si no les funcione agréguenle la palabra sudo al principio del comando para abrirlo con permisos de superusuario).

- **ip address:** Nos da datos sobre nuestros dispositivos de red, incluyendo la IP interna del servidor.

Ahora, para conectarse al servidor desde un dispositivo en la misma red, se puede usar el comando:

`ssh username@localip`

Desde la PowerShell de Windows o la consola del sistema operativo que estés usando.

Nota: En caso de querer acceder remotamente a un servidor, el comando es el mismo, solo que ahora en vez de usar la ip local se usaría la IP pública, la cual se puede ver desde un navegador en internet buscando myip estando conectado a la misma red del servidor o desde el servidor usando algún comando como lo puede ser el siguiente:

`curl ifconfig.me`

Es importante tener en cuenta que para poder tener este acceso, se debe tener abierto a la red el puerto de internet número 22, adicionalmente es una buena práctica utilizar un firewall para que solo ciertas IPs puedan conectarse al servidor y así evitar accesos no autorizados.

# 3. Sistemas de archivos y particionamiento
## ¿Qué son los sistemas de archivos?
Un sistema de archivos es un método que utiliza un sistema operativo para organizar y gestionar datos en un disco o unidad de almacenamiento. Sus funciones principales incluyen:

1. **Organización de Datos**: Permite almacenar datos en archivos y directorios (carpetas).
2. **Gestión del Espacio**: Administra el espacio del disco, asignando y liberando bloques según sea necesario.
3. **Acceso y Seguridad**: Controla quién puede acceder a los archivos y qué pueden hacer con ellos.
4. **Recuperación de Datos**: Facilita la recuperación de datos en caso de errores o fallos.

### Tipos Comunes de Sistemas de Archivos
- **FAT32**: Común en unidades flash, con limitaciones en el tamaño de archivos y particiones.
- **NTFS**: Usado por Windows, soporta grandes archivos y tiene características avanzadas de seguridad.
- **HFS+** y **APFS**: Usados por macOS, optimizados para almacenamiento moderno.
- **ext4**: Utilizado en Linux, conocido por su eficiencia y fiabilidad.

En resumen, un sistema de archivos organiza, gestiona y asegura los datos en una unidad de almacenamiento, facilitando el acceso y la recuperación de los mismos.

![Comparativa](https://static.platzi.com/media/user_upload/sistemadearchivos-a9552368-750e-48a8-ad0c-ea85c380b05b.jpg)

## Particiones de un Servidor Linux
Las particiones en un servidor Linux son divisiones lógicas del espacio de almacenamiento en un disco. Cada partición puede albergar un sistema de archivos distinto y se utiliza para organizar y gestionar los datos de manera eficiente. Aquí tienes una explicación sencilla y los aspectos más importantes:

- **¿Qué es una Partición?** Es una sección separada del disco duro que puede contener un sistema de archivos independiente. Piensa en ellas como divisiones dentro de una misma bodega, donde cada sección almacena distintos tipos de productos.
- **¿Por Qué Particionar?** Las particiones ayudan a organizar los datos, mejorar el rendimiento y la seguridad del sistema, y facilitar la recuperación en caso de fallo.

### Particiones Comunes en un Servidor Linux
- `/:` Contiene el sistema operativo y la mayoría de los archivos del sistema. Es esencial para el funcionamiento de Linux.
- `/boot:` Almacena los archivos necesarios para el arranque del sistema, como el kernel de Linux y los archivos de configuración del gestor de arranque.
- `/home:` Guarda los archivos personales de los usuarios. Tenerla en una partición separada facilita el mantenimiento y las actualizaciones del sistema.
- `/var:` Contiene archivos variables como registros del sistema, colas de impresión, y archivos de datos temporales. Es importante para servidores web y de bases de datos.
- `/tmp:` Utilizada para almacenar archivos temporales. Limitar el tamaño de esta partición puede evitar que archivos temporales llenen el disco principal.
- `swap:` No es una partición de sistema de archivos, sino un espacio de intercambio utilizado como memoria virtual para el sistema. Es crucial para el rendimiento cuando la memoria RAM se agota.

### Aspectos Importantes
- **Tamaño Adecuado:** Asignar el tamaño correcto a cada partición es crucial. Demasiado pequeño puede causar problemas de espacio, y demasiado grande puede ser un desperdicio de recursos.
- **Seguridad y Recuperación:** Tener particiones separadas ayuda a contener los daños en caso de fallos del sistema. Por ejemplo, si algo sale mal en /home, no afectará a /var.
- **Mantenimiento y Actualización:** Las particiones separadas facilitan las actualizaciones del sistema y el mantenimiento, ya que puedes reinstalar el sistema operativo sin afectar los datos de los usuarios en /home.
- **Rendimiento:** Las particiones pueden mejorar el rendimiento del sistema al reducir la fragmentación y permitir un acceso más rápido a archivos específicos.

### Comando más usados
Comando	   | Descripción                                                       |
|----------|-------------------------------------------------------------------|
`lsblk`    | Lista los dispositivos de bloques y las particiones en el sistema |
`fdisk`    | Herramienta para administrar particiones de disco                 |
`parted`   | Herramienta para crear y administrar particiones de disco         |
`mkfs`     | Formatea una partición con un sistema de archivos                 |
`mount`    | Monta un sistema de archivos en una partición o un directorio     |
`umount`   | Desmonta un sistema de archivos                                   |
`df`       | Muestra el espacio libre y utilizado en las particiones montadas  |
`du`       | Muestra el tamaño de un archivo o directorio                      |
`resize2f` | Ajusta el tamaño de un sistema de archivos ext2, ext3 o ext4      |
`lvcreate` | Crea un volumen lógico en un grupo de volúmenes LVM               |
`lvextend` | Amplía el tamaño de un volumen lógico                             |
`lvresize` | Ajusta el tamaño de un volumen lógico                             |
`lvremove` | Elimina un volumen lógico                                         |
`vgcreate` | Crea un grupo de volúmenes LVM                                    |
`vgextend` | Amplía un grupo de volúmenes LVM                                  |
`vgreduce` | Reduce un grupo de volúmenes LVM                                  |
`pvcreate` | Crea un volumen físico LVM en una partición o dispositivo         |
`pvextend` | Amplía un volumen físico LVM                                      |
`pvresize` | Ajusta el tamaño de un volumen físico LVM                         |
`pvremove` | Elimina un volumen físico LVM                                     |

## Swap
