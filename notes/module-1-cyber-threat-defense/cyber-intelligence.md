# Ciberinteligencia

<br></br>
## 1. Introducción

### ¿Qué es la Ciberinteligencia?

Inteligencia enfocada a las amenazas presentes en el entorno digital

### Datos

No estructurados, gran volumen, múltiples fuentes

Por ejemplo:

* logs
* listados de IPs

### Información

Estructurada, centralizada, normalizada

Por ejemplo:

* BBDD

### Inteligencia

Información procesada y analizada, útil de cara a tomar acciones

Por ejemplo:

* IPs vinculadas a un APT

<br></br>
## 2. Fuentes de Inteligencia

Recursos típicos usados por procesos de CTI

* Indicadores de Compromiso(IoCs)
* Redes Sociales
* Información interna (SIEM, EDR, antiguos incidentes)
* Deep/Dark Web
* Plataformas de mensajería (Telegram, Whatsapp)

* Análisis de Malware
* Human Intelligence (HUMINT)
* Geopolítica
* Open Source Intelligence (OSINT)
* Plataformas de intercambio de información

<br></br>
## 3. Ciclo de Inteligencia

Ciclo de vida de la inteligencia de ciber-amenazas

### ¿En qué consiste cada fase?

1. Planificación:

* Definición de llos objetivos y requisitos del ejercicio

2. Recolección:

* Selección de fuentes y obtención de datos

2. Procesado:

* Transformación de los datos obtenidos en información estructurada y normalizada

3. Análisis:

* Aplicación de métodos formales de análisis para producir inteligencia accionable

4. Difusión:

* Envió del producto de inteligencia a los órganos destinatarios correspondientes

<br></br>
## 4. Tipos de Inteligencia

Tipos de Inteligencia según sus objetivos

- Estratégica:

Proporciona una vista a alto nivel del panorama de amenazas y riesgos

Este tipo de inteligencia trabaja estrechamente con los procesos de Gestión de Riesgos.
Su producto se presenta a los niveles directivos de la organizaciones


- Táctica:

Proporciona información detallada de las TTPs de los actores maliciosos

Su objetivo es hacer entender en detalle cómo son atacadas las infraestructuras, con qué objetivos y cómo poder evitarlo o responder efectivamente.

Esta inteligencia es presentada a puestos técnicos como expertos en seguridad, SOC Managers, etc.


- Operativa:

Se utiliza para identificar en tiempo real patrones de ataques concretos

Su objetivo es la correlación de actividades maliciosas en un ataque concreto y la identificación del atacante en el momento de un incidente.

Esta información es presentada al equipo de DFIR para que puedan determinar las capacidades del atacante, el estado actual del ataque  y el posible impacto, así como orientar el análisis y la respuesta de forma más efectiva.


- Técnica:

La inteligencia técnica proporciona indicadores de compromiso a bajo nivel como direcciones IP, URLs, hashes de malware, etc

El objetivo es la detección de estops indicadores para ofrecer respuesta a tiempo real. Aunque por la naturaleza de los entregables, es información que tiene un tiempo de vida relativamente corto.

La inteligencia generada se consume de forma autónoma por los sistemas de monitorización.


<br></br>
## 5. Cyber Kill Chain

Fases de un ataque cibernético (Lockheed Martin)

- Reconocimiento:
Se selecciona, se identifica y se investiga a la víctima

- Armamento:
Se eligen los vectores de ataque para lograr el acceso no auitorizado a los sistemas objetivo

- Entrega:
Se lleva a cabo la campaña de distribución del malware a través del canal elegido

- Explotación:
Se materializa el acceso inicial

- Instalación:
Se establece la presencia en el sistema, asegurando el mantenimiento del control

- C&C:
Se establece un canal de comunicación con un sistema externo controlado por el atacante

- Acciones en Objetivos:
Se consigue el objetivo final


<br></br>
## 6. Tácticas, Técnicas y Procedimientos (TTPs)

Tácticas, Técnicas y Procedimientos

- Tácticas:
Descripción a alto nivel de cuál es el objetivo del atacante

Ejemplo:

* Establecer persistencia


- Técnicas:
Guía de como conseguir el objetivo definido

Ejemplo:

* A través del Registro de Windows


- Procedimientos:
Mecanismos concretos y detallados de cómo desarrollar la actividad

Ejemplo:

* Establecer persistencia mediante la clave RunOnce


<br></br>
## 7. MITRE ATT&CK

Framework MITRE ATT&CK


<br></br>
## 8. Advance Persistent Threats (APTs)

¿Motivación?

1. Grupos Estatales:

- Política
- Destructiva
- Espionaje


2. Hacktivistas:

- Política


3. Ciber-Criminales:

- Económica
- Destructiva


<br></br>
## 9. Difusión de Inteligencia

Estándares STIX y TAXII

- STIX Structured Threat Information eXpression:

1. Lenguaje y formato estructurado enfocado a la difusión de Inteligencia de Ciber-Amenazas

2. Permite definir conceptos complejos como las motivaciones y las capacidades de los actores


- TAXII Trusted Automated Exchange of Intelligence Information

1. Protocolo a nivel de aplicación a modo de API para compartir inteligencia de forma simple y escalable

2. Diseñado específicamente para transmitir datos en formato STIX

3. Soporta diferentes modelos:
    - Colección: Modelo Request-Response
    - Canal: Sistema de feeds a los que el cliente se suscribe o el proveedor publica inteligencia



<br></br>
## 10. Herramientas de Open Source

Plataformas Open-Source

- OpenCTI:

1. Plataforma open-source de Ingesta, Análisis y Difusión de ciberinteligencia

2. En desarrollo constante y soporte actual para la ingestión y enriquecimiento a partir de múltiples fuentes externas

3. Permite exponer feeds TAXII personalizados, exportar objetos STIX e incluso generar informes


- MISP Malware Information Sharing Plataform:

1. Plataforma open-source de Difusión de inteligencia colaborativa

2. Ampliamente utilizado por organizaciones públicas: RNS, FIRST, NATO/OTAN

3. Soporta importar y exportar información en STIX



<br></br>
## 11. Usos de la CTI


### Threat Hunting y Monitorización Continua


- Threat Hunting:
Provee al equipo de Threat Hunting de hipótesis


- Monitorización Continua:
Prioriza la creación de casos de uso y enriquece el contexto de las alertas


### DFIR y Análisis de Malware:

- DFIR:
Orienta la investigación o atribuye el ataque en caso de ser posible


- Análisis de Malware:
Asocia a una familia o APT concreto, produce reglas de detección, mapea las capacidades a Mitre ATT&CK


- Superficie de Ataque (ASM):
Analiza la infraestructura en busca de posibles vectores de entrada en función a TTPs conocidas


- Purple Team:
Orquesta operaciones conjuntas entre los equipos de Red Team(ataque) y Blue Team(defensa)



