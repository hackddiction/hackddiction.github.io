---
title: "Threat Intelligence 101"
date: 2024-05-18
categories: [Cybersecurity, Threat Intelligence]
tags: [Threat Intelligence, cyberSec101, cybersecurity]
author: <MH>
comments: false
img_path: /assets/img/postimg/threatintell
image: banner2.jpg
lang: es
lang-ref: threatintell
---

## ¿Qué es Threat Intelligence?

Threat Intelligence, Threat Intel o Cyber Threat Intelligence (CTI) se refiere al proceso de **recolectar, analizar y actuar sobre información relevante acerca de potenciales amenazas y riesgos para la seguridad de una organización**. Esta información puede incluir indicadores de compromiso (IOCs); tácticas, técnicas y procedimientos (TTPs) de ataques cibernéticos; así como perfiles de actores maliciosos. El objetivo principal de la Inteligencia de Amenazas es **permitir que las organizaciones anticipen, mitiguen y respondan proactivamente a las amenazas cibernéticas**, fortaleciendo así sus defensas y reduciendo el riesgo de impactos negativos en sus activos, datos y operaciones.

## Tipos de Threat Intelligence

De acuerdo a IBM, hay tres tipos principales de Threat Intelligence. Puedes encontrar el artículo completo de [Threat Intelligence de IBM aquí!](https://www.ibm.com/topics/threat-intelligence#Types+of+threat+intelligence)

### Tactical Threat Intelligence
**Tactical Threat Intelligence** o Inteligencia de Amenazas Táctica se enfoca en la **detección y respuesta inmediata a las amenazas cibernéticas**. Involucra indicadores específicos de compromiso (IoCs) como direcciones IP maliciosas, hashes de archivos y líneas de asunto de correos electrónicos de phishing. Este tipo de inteligencia ayuda a los centros de operaciones de seguridad (SOCs) y a los equipos de respuesta a incidentes a filtrar falsos positivos e identificar amenazas reales.

La **Inteligencia de Amenazas Táctica** desempeñó un papel crucial en el caso del **ataque a la cadena de suministro de SolarWinds en 2020**. Los investigadores de seguridad analizaron el tráfico de la red, muestras de malware y la infraestructura de comando y control para descubrir el alcance de la vulneración y desarrollar estrategias de remediación.

![Figura 1](1.png)
*Tactical Threat Intelligence.
Fuente: https://www.crowdstrike.com/cybersecurity-101/threat-intelligence/*

### Operational Threat Intelligence
**Operational Threat Intelligence** o Inteligencia de Amenazas Operativa proporciona información detallada sobre ataques cibernéticos específicos. Incluye información sobre las **tácticas, técnicas y procedimientos (TTPs)** utilizados por los actores de amenazas. Este tipo de inteligencia respalda **medidas de defensa proactivas**, ayudando a las organizaciones a comprender la naturaleza de las amenazas que enfrentan y cómo defenderse de ellas de manera efectiva. Es particularmente útil para los centros de operaciones de seguridad y los equipos de respuesta a incidentes en la **planificación y ejecución de acciones defensivas**.

El caso de **Emotet** puede ser utilizado como un **ejemplo practico de Inteligencia de Amenazas Operativa**. Emotet es una cepa de malware sofisticada conocida por su capacidad para entregar otras cargas de malware, como TrickBot y el ransomware Ryuk. La Inteligencia de Amenazas Operativa ha sido crucial en **monitorizar la infraestructura de Emotet, rastrear campañas de distribución e identificar sistemas recién comprometidos**. Los equipos de seguridad **aprovechan esta inteligencia** para bloquear archivos adjuntos maliciosos en correos electrónicos, detectar infecciones de Emotet e interrumpir las comunicaciones de comando y control para **prevenir la propagación futura de malware**.

![Figura 2](2.png)
*Operational Threat Intelligence.
Fuente: https://www.crowdstrike.com/cybersecurity-101/threat-intelligence/*

### Strategic Threat Intelligence
**Strategic Threat Intelligence** o Inteligencia de Amenazas Estratégica involucra la recolección, análisis e interpretación de información para comprender **tendencias a largo plazo, patrones y riesgos potenciales** que podrían afectar la postura general de seguridad de una organización. Se enfoca en proporcionar **información y orientación a alto nivel** para informar la toma de decisiones estratégicas, como la asignación de recursos, el desarrollo de políticas y las estrategias de mitigación de riesgos. La Inteligencia de Amenazas Estratégica tiene como objetivo anticipar amenazas emergentes, identificar vulnerabilidades y evaluar el panorama más amplio de amenazas y riesgos cibernéticos para ayudar a las organizaciones a **anticiparse a posibles desafíos de seguridad**.

Las organizaciones a menudo dependen de la **Inteligencia de Amenazas Estratégica proporcionada por informes, estudios y evaluaciones de la industria** para comprender tendencias más amplias y amenazas emergentes relevantes para su sector. Por ejemplo, los informes anuales de los proveedores de seguridad ofrecen conocimientos estratégicos sobre amenazas prevalentes, vectores de ataque y vulnerabilidades específicas de la industria. Las empresas utilizan esta inteligencia para **soportar sus estrategias de seguridad, priorizar inversiones y asignar recursos de manera efectiva**.

![Figura 3](3.png)
*Strategic Threat Intelligence.
Fuente: https://www.crowdstrike.com/cybersecurity-101/threat-intelligence/*
