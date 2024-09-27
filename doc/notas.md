# Notas

* Buenos dias a todos!
* En principio, agradecerles por participar de esta charla
* Agradecer a las autoridades de la Escuela de Informática (Alfredo y Celia) y a toda la UNO en su conjunto

* Paso a presentar la Agenda de la charla. El tiempo de la misma es de 1h. y la planifiqué de la siguiente forma:
  * Presentación (me presento)
  * Programación Web
  * Accesibilidad Web

---

## Presentación

* **Lenguajes Formales**: modelos matemáticos formales para solucionar problemas computacionales. Modelos como: AF, AP, GIC, MT

* **Programación con Objetos**: desarrollo de SW usando objeto-mensaje, encapsulamiento, polimorfismo, herencia. Hacer programas donde los objetos se comunican enviandose mensajes para solucionar un problema

* **Programación Web**: presentar y trabajar con tecnologías que complementan el desarrollo de aplicaciones o sitios web. Las APP Web son herramientas que los usuarios pueden usar accediendo a un servidor a traves de Internet o de una Intranet mediante un navegador (browser). Ej: Chrome, Firefox, Edge, ...
  * ***Servidor Web***: programa que procesa una aplicación del lado del servidor. Ej: NGINX, Apache. Escuchan peticiones de los clientes (navegadores).  Cliente --> request --> Server  y server devuelve response

* **Lenguajes de Programación**: Evolución de los LP, clasificación de los LP (ej. compilado vs interpretado). aspectos sintácticos, semánticos, y pragmáticos. Decidir que LP es el más adecuado para cada tipo de problema a resolver.

* **INVAP**: Es una empresa referente en proyectos tecnologicos a nivel mundial y protagonista del desarrollo en Argentina. Dedicada al diseño y construcción de sistemas tecnologicos complejos (de avanzada). Compuesta por 4 gerencias: defensa, medicina, nuclear y espacial. Dentro de espacial: construcción de satélites de aplicaciones científicas y de comunicaciones (ARSAT-1, ARSAT-2).
  * ***Mis tareas en INVAP*** fueron evaluar las respuestas (telemetria) de ejecución de los telecomandos desde tierra tomados de la base de datos SATDB. También desarrollaba programas en Java que probaba los subsistemas del software de vuelo (flight software) de ARSAT-1

* **AFIP**: Administración Federal de Ingresos Públicos. Organismo que tiene a su cargo la ejecución de la política tributaria , aduanera y de recaudación de los recursos de la seguridad social de la Nación.
  * ***Mis tareas en AFIP*** son desarrollar tests automáticos en Java o Python para probar los servicios que utilizaran los contribuyentes. Evaluo tecnologías. Construyo herramientas que faciltan el trabajo de desarrolladores y homologadores. Ej. FETA y WA11Y. Capacitaciones a los equipos de la dirección

---

## Sistema de Información

* Es un conjunto de componentes interrelacionados (datos, procedimientos, SW, HW, RRHH) que trabajan juntos para recopilar, procesar, almacenar y difundir información para apoyar la toma de decisiones. **MEJORAR**

## Etapas

1. **Planificación**: documentar los requerimientos del proyecto y las tecnologías a usar
1. **UX/UI**: definir los flujos e interacción del usuario y diseño de pantallas
1. **Desarrollo**: de la UI, BD, lógica de la APP
1. **Despliegue**: subirlo a un entorno productivo
1. **Soporte**: corregir errores no detectados, etc.

Se arman equipos de trabajo (todos somos responsables de todo). Se elige metodología:  cascada / agil (SCRUM)

## Desarrollo Web

* **FRONTEND**: es la parte encargada del lado del cliente. Lo que se observa en pantalla. Lo que el browser "renderiza"
  * HTML5: estructura, maquetado, contenido (encabezados, tablas, listas, links, imágenes)
  * CSS3: estilos (colores, fonts, fondos, bordes, animaciones)
  * JS: comportamiento (validaciones, lógia, efectos)
  * Frameworks: (bootstrap, vue, react, angular, jquery)

* **BACKEND**: es la parte encargada del lado del servidor. No es visible. Es el núcleo del negocio de la empresa. Se crea con código mediante un lenguaje de programación web
  * Python (Flask, Django). Adm lib: pip
  * Java (Spring). Adm lib: maven, gradle
  * JS (nodejs, express, nestjs). Adm lib: npm
  * PHP (laravel). Adm lib: composer
  * Otros lenguajes: GO, Rust, Ruby, C#
  * Storage: MySQL, Oracle, PostgreSQL, SQLite, MongoDb, Redis

* Tanto Front como Back se comunican mediante APIs (request/response) bajo el protocolo HTTP/HTTPS

## QA automation

* **Quality assurance**: asegurar el correcto funcionamiento de una solución tecnológica
  * ***Finalidad***. pulir al máximo el control de errores, para entregar un producto lo mas cercano a la perfección

* **Heramientas de QA automatión**:
  * Python (unittest, pytest). Selenium. Locus
  * Java (JUnit5, TestNG). Selenium. JMeter
  * JS (Mocha). Cypress. Artillery/K6
  * PHP (PhpUnit)
  * Appium para celulares

## Deploy

* Se nesecita:

* **Un dominio**: nombre asociado a una dirección IP de Internet. Ej www.uno.edu.ar

* **Un servidor**: una computadora conectada a Internet donde publicas todos los recursos de tu APP Web

* Servidor para hacer deploy gratis:
  * Heroku
  * Firebase
  * GitHub Pages
  * **Render**

## Otras herramientas

* Terminal (LDC)
* Git (GitHub/GitLab): control de versiones, repo de código, trabajo colaborativo
* Docker: permite crear contenedores (entorno aislado e independiente)
* Kubernetes: orquestador de contenedores. Adm de carga de servicios. Ej:  ARGO CD, OpenShif de ReadHat
* Jenkins. Servidor de integración continua

---

## AW

* Es una práctica que tiene como objetivo lograr que las páginas web sean utilizadas por el máximo número de personas, independientemente de sus conocimientos o capacidades personales, independientemente de las características técnicas del equipo para acceder a la Web

* AW nos benficia a TODOS, ya que se trata de que todos puedan acceder a la Web
  * ambiente ruidoso, no permite oir el audio de un video
  * ambiente con poco iluminación: dificulta la lectura
  * intener limitada: no permite acceder a contenido con imagenes, etc

* Sitio accesible. Tiene que ser:
  * **comprensible**: contendios claros y simples
  * **navegable**: mecanismos sencillos de navegación
  * **perceptible**: alternativas textuales, constrastes

## Técnicas

* CAPTCHA: confirmar si al contenido está accediendo un humano y no una computadora. Proporcionar maneras alternaticas de CAPTCHA con emisiones dirigidas a diferentes sentidos que se ajusten a diferentes capacidades
* Subtítulos para todo contenido de audio
* Imágenes con alternativa textual
* Control de audio con mecanismo para pausarlo y controlar volumen
* Contraste
* Toda la funcionalidad accesible a través de teclado
* Foco: orden y resaltado (visible)
* Tiempo suficiente para leer y usar el contenido.  Desactivar el límite de tiempo o ajustarlo hasta un rango de al menos 10 veces la duración por defecto (exc. subastas)
* Las páginas web no contienen nada que destelle más de 3 veces en cualquier período de un segundo, ya que puede causar ataques

---

**OBJETIVO**: ayudarlos a organizar y usar las tecnologías web, brindando innovaciones, buenas prácticas y experiencia laboral para que udes el día de mañana puedan entender y reconocer necesidades que las diferentes instituciones pueden tener
