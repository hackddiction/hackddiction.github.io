---
title: "Cyber Kill Chain: El Ciclo de Vida de un Ciberataque"
date: 2023-10-30
categories: [Cybersecurity, General Concepts]
tags: [attack life cycle, general concepts, cyberSec101, cybersecurity]
author: <MH>
comments: false
img_path: /assets/img/postimg/cyberkillchain
image: banner.jpg
lang: es
lang-ref: cyberkillchain
---

En el panorama digital actual, la importancia de la ciberseguridad no puede ser subestimada. A medida que las ciber-amenazas continúan evolucionando, entender las tácticas empleadas por los atacantes es crucial. Un marco que ha demostrado ser muy útil en este esfuerzo es el conocido como **Cyber Kill Chain**. Este modelo describe las etapas de un ciber-ataque, proporcionando un enfoque estructurado para comprender y defenderse contra las amenazas. A continuación, profundizaremos en las siete etapas de la **Cyber Kill Chain** utilizando como referencia una infografía de Lockheed Martin. Puedes ver la [infografía completa aquí!](https://www.lockheedmartin.com/en-us/capabilities/cyber/cyber-kill-chain.html)

![Figura 1](CKC.png)
*Cyber Kill Chain.
Fuente: https://www.lockheedmartin.com/en-us/capabilities/cyber/cyber-kill-chain.html*

## Etapa 1: Reconocimiento

La primera fase, el Reconocimiento, implica la recopilación de información sobre el objetivo. Esta etapa es similar a un atacante investigando un lugar físico antes de planificar un robo. Aquí, **los ciber-delincuentes recopilan datos** sobre la infraestructura del objetivo, su personal y vulnerabilidades. Esto puede incluir la utilización de fuentes de información pública (OSINT), enumeración de sistemas de nombres de dominio (DNS) y técnicas de ingeniería social. Los equipos de seguridad pueden contrarrestar esta fase monitoreando fuentes públicas de información relacionadas a la organización.

![Figura 2](1.jpg)
*OSINT.
Fuente: Google*

## Etapa 2: Armamento

En la fase de Armamento, el atacante **crea un *payload* malicioso**, a menudo en forma de malware, para explotar una vulnerabilidad descubierta durante el reconocimiento. Este *payload* se elabora para **evadir la detección**. Es crucial para las organizaciones mantenerse actualizadas en cuanto a parches de seguridad y proteger dispositivos finales para mitigar los riesgos asociados con esta etapa. [Puedes encontrar un articulo completo sobre malware aquí!](https://hackddiction.github.io/es/cybersecurity/general%20concepts/2023/08/22/Hablemos_Sobre_Malware.html)

![Figura 3](2.jpg)
*Malware.
Fuente: Google*

## Etapa 3: Entrega

La fase de Entrega implica la **transmisión del *payload* malicioso** al objetivo. Esto puede ocurrir a través de **varios canales**, incluidos correos electrónicos, sitios web o incluso medios físicos. Los atacantes pueden emplear técnicas como correos electrónicos de phishing o descargas involuntarias. Implementar filtrado de correos electrónicos, filtrado web y concientizar a los empleados sobre hábitos seguros de navegación son defensas esenciales contra esta fase.

![Figura 4](3.jpg)
*Correos Maliciosos.
Fuente: Google*

## Etapa 4: Explotación

Una vez que el *payload* llega al sistema objetivo, comienza la fase de Explotación. El **malware ejecuta su código**, aprovechando la vulnerabilidad para la que fue diseñado. La aplicación oportuna de parches de seguridad, evaluaciones de vulnerabilidad regulares y la segmentación de redes son medidas clave para frustrar intentos de explotación.

![Figura 5](4.jpg)
*Código Arbitrario.
Fuente: Google*

## Etapa 5: Instalación

En la fase de Instalación, el atacante **establece una presencia persistente** dentro del sistema comprometido. Esto puede implicar la instalación de puertas traseras, rootkits u otras técnicas sigilosas. Emplear mecanismos de autenticación sólidos, monitorear la actividad anómala y llevar a cabo auditorías de seguridad regulares puede ayudar a detectar y mitigar instalaciones no autorizadas.

![Figura 6](5.jpg)
*Puertas Traseras.
Fuente: Google*

## Etapa 6: Comando y Control

Habiendo obtenido persistencia en el entorno objetivo, el atacante busca **establecer un canal de comunicación de regreso a su infraestructura**. Esta fase, conocida como Comando y Control, permite al atacante **administrar el sistema comprometido de forma remota** y extraer datos sensibles. Emplear monitoreo del tráfico de red, sistemas de detección de intrusos (IDS) y firewalls con capacidades avanzadas de detección de amenazas son cruciales para detectar y prevenir actividades de Comando y Control.

![Figura 7](6.jpg)
*Control Remoto.
Fuente: Google*

## Etapa 7: Acciones sobre Objetivos

La fase final, Acciones sobre Objetivos, es donde **el atacante logra su objetivo final**. Esto podría implicar robo de datos, interrupción de operaciones u otras actividades maliciosas. Implementar cifrado de datos sólido, controles de acceso y sistemas de detección de amenazas avanzadas puede mitigar significativamente los riesgos asociados con esta fase.

![Figura 8](7.png)
*Brecha de Datos.
Fuente: Google*

## Conclusión

Comprender la ***Cyber Kill Chain*** proporciona a las organizaciones un marco para comprender el ciclo de vida de un ciber-ataque. Al descomponer el proceso de ataque en fases distintas, las organizaciones pueden implementar **medidas de seguridad específicas** en cada etapa. Este enfoque proactivo es esencial, ayudando a las organizaciones a mantenerse un paso adelante de los adversarios y proteger sus activos valiosos.
