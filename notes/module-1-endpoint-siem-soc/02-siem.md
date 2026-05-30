# SIEM


## Que es SIEM

### Security Information and Event Management

1. Recoge logs de multitud de servicios de la organizacion (firewall, aplicaciones, EDR, Eventos de Windows, Active Directory)

2. Procesa y analiza a tiempo real esta informacion para detectar y reportar actividades sospechosas.

3. Correlaciona eventos y alertas para agrupar actividades.

4. El coste de estas herramientas es definido por el volumen de ingesta y el tiempo de retencion.



## Ingesta

### ¿Que podemos ingestar?

- Firewall
- Active Directory
- Aplicaciones
- IDS/IPS
- CTI

- Eventos de Endpoints
- Servicios Cloud
- EDR
- Sensores Fisicos
- WAF


### Normalizacion de Datos

    - Common Event Format(CEF)
        - Common Log Format
            - Extended Log Format(ELF)
                - CSV
                    - Custom
                    
                    - SYSLOG
                - RAW
            - Windows Event Logs(EVTX)
        - XML
    - JSON



### Metodos de Filtrado de Logs

¿Que registramos?

- En el momento de la generacion de los logs hay que decidir que eventos registrar y cuales no.

- Desarrollo de Software, Configuraciones de Aplicaciones y servicios, etc.

- Hay que tener en cuenta las regulaciones, niveles de logging, rotacion de logs, etc.


¿Que enviamos?

- De todos los eventos registrados, se seleccionan cuales son los que se van a enviar al SIEM.

- Evento de Seguridad de Windows, eventos criticos de aplicaciones, resolucion DNS.

- Solo hay que enviar la informacion util para las operaciones de auditoria y seguridad.


¿Que guardamos?

- De llos eventos recibidos, se filtran los que van a formar parte de la retencion.

- Event IDs concretos, Trafico de servidores criticos.

- Se centra en los eventos necesarios para la monitorizacion continua, DFIR y auditoria normativa.



## Monitorizacion


### Casos de Uso

INFO

    - Uso de Disco > 80%
        - Capacidad reducida de espacio para la base de datos de una herramienta.

LOW
    - Carpeta compartida de SharePoint eliminada
        - Borrado de una carpeta con contenido compartida con mas usuarios.

MED

    - Creacion de un usuario privilegiado
        - Creacion de un usuario con permisos de administracion.




HIGH

    - Inicio de sesion exitoso desde una IP de otro pais
        -Inicio de sesion desde un pais poco comun y con una direccion IP de mala reputacion.

CRIT

    - Caida de Servidor Critico
        - Perddida de ingesta y hearbeats del servidor principal de la organizacion durante mas de una hora.

LOW

    - Multiples intentos fallidos de inicio de sesion
        - Posible fuerza bruta de contraseñas desde la misma IP hacia un usuario con MFA.



### Casos de Uso

NOMENCLATURA:

¿Como identificamos los casos de uso?

- Nombres
- Codigos: UMMA-0001
- UUDIs


TIPOLOGIA:

¿De que tipo pueden ser los casos de uso?

- Salud de los Servicios, version soportada de los agentes EDR, ingesta continuada.
- Deteccion de Amenazas, malware, login exitosos.
- Caza Proactiva, zero-days, CVEs concretos, IOCs de un incidente.

