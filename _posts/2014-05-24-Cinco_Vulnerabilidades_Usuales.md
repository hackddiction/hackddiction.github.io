---
title: "Cinco Vulnerabilidades Usuales Dentro de una Organización"
date: 2014-05-24
categories: [Cybersecurity, Vulnerabilities]
tags: [vulnerabilities]
author: <MH>
comments: false
img_path: /assets/img/postimg/brechas
image: SecurityBreach.jpg

---

Como ya han de saber, las vulnerabilidades siempre están presentes dentro de las organizaciones y si no son analizadas o controladas de alguna forma antes de ser explotadas, podrían representar un grave peligro para los activos de información propios de la organización comprometida.

Existen niveles de criticidad en las vulnerabilidades asociadas a sistemas de información. En el siguiente post hablaremos sobre 5 vulnerabilidades usualmente catalogadas como riesgo bajo pero que son importantes de analizar, ya que podrían representar el primer paso para un ataque mucho más grande.

# Vulnerabilidad 1: Contraseñas poco robustas

Siempre un atacante buscara entrar por el lado más desprotegido o poco controlado dentro de una organización, por ejemplo el factor humano. Entonces, en términos de credenciales, los usuarios siempre van a preferir utilizar contraseñas fáciles de recordar, simples o asociadas a algún evento o vivencia importante como un cumpleaños o el nombre de sus hijos. En otros casos utilizan contraseñas secuenciales como “Abril 2014++”, “Mayo2014++” y así sucesivamente.

**CRASO ERROR!** Ese tipo de contraseñas son fáciles de romper mediante algoritmos de fuerza bruta, utilización de diccionarios o mecanismos híbridos. Utilizar este tipo de contraseñas compromete en un nivel muy alto la información manejada por el usuario. Hay que tener presente que si se trata de un usuario clave en la organización, la información que maneja puede ser muy sensible. Contraseñas de servidores, accesos a base de datos y estrategias comerciales son algunos ejemplos.

> Mientras tu contraseña sea lo más compleja posible y no guarde relación con asuntos personales, el riesgo de romperla disminuirá.
{: .prompt-tip }

![Figura 1](figura1.png)
*Utilizando John The Ripper para obtener la contraseña del usuario root*

# Vulnerabilidad 2: Divulgación de Información

Hablando sobre los productos de Microsoft, ¿Cuantos no han visto alguna vez  la típica pantalla amarilla de error que representa una excepción no controlada en aplicaciones web? ¿Cuántos no se han visto frente a la ostentosa pantalla del IIS7 al tratar de entrar a una página web de forma errada?

![Figura 2](figura2.png)
*Banner de Microsoft IIS7*

Para un usuario común, ese par de pantallas podrían ser insignificantes y hasta inentendibles, pero **para un atacante podrían ser de mucha utilidad** dentro de un proceso de Footprinting o cosecha de datos para luego desplegar ataques elaborados.

Al ver la pantalla de IIS7 un atacante pensaría automaticamente lo siguiente:

- IIS versión 7
- Sistema operativo utilizado por el servidor: Windows Server 2008 (como mínimo)
- Posiblemente utilicen ASP.Net en Visual o C# ya que es lo más comercial.

Realmente a un atacante no le pesaría la mano para buscar en google que tipo de vulnerabilidades existen para IIS7 o levantar en una máquina virtual un servidor con esas características y pasarle un escáner de vulnerabilidades. 

**Sucede lo mismo para las excepciones no controladas**, si alguna emite un mensaje de error ORA, inmediatamente sabríamos que se utiliza un DBMS Oracle y de ser una aplicación poco robusta podríamos comenzar con pruebas simples de inyecciones SQL.

> Hay que tener mucho cuidado con la información que se difunde de cara a Internet, nunca se sabe quién está del otro lado.
{: .prompt-tip }

# Vulnerabilidad 3: Sistemas no parchados

Es un hecho que **los sistemas que no cuentan con las últimas actualizaciones de software son los más propensos a convertirse en blanco de un ataque.** Es cierto que mantener un sistema actualizado es considerado como una buena práctica, pero a veces se convierte en una tarea complicada más aun cuando se trabaja en ambientes de producción donde se requiere alta disponibilidad de las aplicaciones.

Por ejemplo, si una organización cuenta con una aplicación web basada en Net Framework 1.1 sobre WS2000 y actualiza la versión del SO a WS2008 sin haber realizado pruebas, puede que se presenten problemas que afecten la disponibilidad del servicio, ya que sin la instalación de ciertos hotfix el Framework 1.1 no trabaja bien con WS2008. Muchas veces los administradores de servidores optan por desactivar las actualizaciones automáticas debido a que no se puede predecir el comportamiento de una aplicación frente a las actualizaciones de software para un servidor. En este sentido, se deberá de optar por otras alternativas para garantizar la disponibilidad de servicios y la seguridad de los servidores en simultáneo.

![Figura 3](figura3.png)
*Windows Update*

# Vulnerabilidad 4: Configuraciones por Defecto

Cuando una organización adquiere una nueva tecnología o un hardware especializado (firewalls, preventores etc) casi siempre dejan la instalación y configuración del producto en las manos del proveedor. En teoría, hacer eso es lo más lógico ya que nadie dentro de la organización es especialista o  conocedor del nuevo producto.

**En la práctica, hacer eso es un tanto riesgoso.** Los proveedores en algunos casos optan por enviar personal poco capacitado para la instalación de sus productos dado que les genera un menor costo o incluso tercerizan la instalación. En otros casos, los proveedores optan por las instalaciones por defecto, ya que no quieren arriesgarse a que la instalación provoque problemas en la operativa del cliente. Esto genera configuraciones y credenciales que todo el mundo conoce. ¿Quién no sabe que las credenciales por defecto de un Tomcat son admin/admin?  

> Exijan siempre instalaciones personalizadas o designen siempre alguien que supervise la instalación.
{: .prompt-tip }

# Vulnerabilidad 5: Controles sin seguimiento

Dentro de las organizaciones siempre se crean procedimientos o controles que buscan alinear la operativa diaria de los colaboradores internos. En muchos casos, **las organizaciones creen que solo basta con definir procedimientos y no realizan un seguimiento para validar si el procedimiento está siendo cumplido** a cabalidad. Por ejemplo: Una organización que realiza sus propios desarrollos debe de garantizar que sean confiables y que no generen brechas de seguridad. Para esto se debe de definir un procedimiento o políticas de desarrollo seguro. Estas permitirán asegurar los desarrollos pero ¿Qué pasa si los desarrolladores no cumplen con estas políticas por un tema de practicidad o para darle mayor agilidad al proceso de desarrollo?

Esto podría ser una situación real para cualquier organización si es que no se hacen controles periódicos donde se valide que los desarrollos cumplan con los lineamientos establecidos.