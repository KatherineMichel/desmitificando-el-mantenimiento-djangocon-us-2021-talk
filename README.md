# Desmitificando el Mantenimiento- DjangoCon US 2021 Talk

## Table of Contents

- [About](#about)
- [Slides and Script Table of Contents](#slides-and-script-table-of-contents)
- [Slides and Script](#slides-and-script) 
- [Attribution](#attribution)
- [Contact Kati](#contact-kati)
- [Copyright](#copyright)

<hr>

## About

Slides and script for a talk Katherine "Kati" Michel ([Twitter](https://twitter.com/KatiMichel), [GitHub](https://github.com/KatherineMichel)) gave at DjangoCon US Saturday, October 23, 2021.
 
Conference Page
* [DjangoCon US 2021](https://2021.djangocon.us/)

Slide Deck and Video Recording
* [Original slide deck]()
* ["Desmitificando el Mantenimiento"]()
* [Video recording]()

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Slides and Script Table of Contents

- [Desmitificando el Mantenimiento](#desmitificando-el-mantenimiento)
- [Mis Afiliaciones](#mis-afiliaciones)
- [Objetivos de la Charla](#objetivos-de-la-charla)
- [Supuestos](#supuestos)
- [Iniciandonos en la Colaboración y la Revisión de Código en GitHub](#iniciandonos-en-la-colaboración-y-la-revisión-de-código-en-github)
- [Vocabulario: GitHub Documentación en Español](#vocabulario-github-documentación-en-español)
- [Terminología de GitHub](#terminología-de-github)
- [El mantenimiento no es sólo acerca de código](#el-mantenimiento-no-es-sólo-acerca-de-código)
- [Intenta ponerte en Los Zapatos del Colaborador](#intenta-ponerte-en-los-zapatos-del-colaborador)
- [GitHub Guías de Código Abierto: “Una Lista de Verificación Antes de Contribuir”](#github-guías-de-código-abierto-una-lista-de-verificación-antes-de-contribuir)
- [Algunos Signos de un Proyecto Saludable](#algunos-signos-de-un-proyecto-saludable)
- [Proceso Ideal](#proceso-ideal)
- [Community Health Files](#community-health-files)
- [Documentación](#documentación)
- [Cómo Los Colaboradores Contribuyen](#cómo-los-colaboradores-contribuyen)
- [Modelo de Repo Comparido](#modelo-de-repo-comparido)
- [Modelo Fork y Pull](#modelo-fork-y-pull)
- [Crear un Pull Request](#crear-un-pull-request)
- [Revisando un Pull Request](#revisando-en-pull-request)
- [Revisando un Pull Request](#revisando-en-pull-request-1)
- [Pull Request: Línea Comando](#pull-request-línea-comando)
- [Pull Request: Opciones Si No Ejecutas el Código Localmente](#pull-request-opciones-si-no-ejecutas-el-código-localmente)
- [Pull Request: Opciones Si Ejecutas el Código Localmente](#pull-request-opciones-si-ejecutas-el-código-localmente)
- [Pull Request: Comandos](#pull-request-comandos)
- [Flujo de Trabajo: GitHub Flow](#flujo-de-trabajo-github-flow)
- [Flujo de Trabajo: Variación](#flujo-de-trabajo-variación)
- [Algunas Recomendaciones](#algunas-recomendaciones)
- [Licenses](#licenses)
- [Seguridad](#seguridad)
- [CHAOSS: Métricas de Código Abierto para Evaluar la Salud de Tu Proyecto](#chaoss-métricas-de-código-abierto-para-evaluar-la-salud-de-tu-proyecto)
- [Más Funciones Útiles de GitHub](#más-funciones-útiles-de-github)
- [Un Caso de Estudio: Sitio Web de DjangoCon US](#un-caso-de-estudio-sitio-web-de-djangocon-us)
- [Puntos Clave](#puntos-clave)
- [DjangoCon US: La Conferencia Con Un Corazón](#djangocon-us-la-conferencia-con-un-corazón)
- [Los Sitios que He Supervisado](#los-sitios-que-he-supervisado)
- [Los Pull Requests Más Fácil (sesenta y siete commits, veinte ocho pull requests)](#los-pull-requests-más-fácil-sesenta-y-siete-commits-veinte-ocho-pull-requests)
- [Yo aprendí como…](#yo-aprendí-como)
- [Aumento en el Número de Colaboradores](#aumento-en-el-número-de-colaboradores)
- [Me Convertí en Mentor](#me-convertí-en-mentor)
- [Algunas Lecciones Aprendidas del Sitio Web de DjangoCon US](#algunas-lecciones-aprendidas-del-sitio-web-de-djangocon-us)
- [Seguridad Psicológica](#seguridad-psicológica)
- [Los Errores Desaparecen en el Historial de Git](#los-errors-desaparecen-en-el-historial-de-git)
- [La Perspectiva del Principiante es Valiosa](#la-perspective-del-principiante-es-valiosa)
- [Logrando Resultados 10x (diez veces)](#logrando-resultados-10x-diez-veces)
- [Mi Primera Charla Tech](#mi-primera-charla-tech)
- [Un Caso de Estudio: Pinax](#un-caso-de-estudio-pinax)
- [Vocabulario de Pinax](#vocabulario-de-pinax)
- [Vocabulario de Testing](#vocabulario-de-testing)
- [Vocabulario de Packaging](#vocabulario-de-packaging)
- [Puntos Clave](#puntos-clave)
- [Fui Contratado por Eldarion para Mantener Pinax](#fui-contratado-por-eldarion-para-mantener-pinax)
- [Nació Pinax: 2008 (Dos Mil Ocho)](#nació-pinax-2008-dos-mil-ocho)
- [Cómo Comenzó](#cómo-comenzó)
- [Cómo Comenzó](#cómo-comenzó-1)
- [Cómo Iba, 80 Proyectos y Apps](#cómo-iba-80-ochenta-proyectos-y-apps)
- [Cómo Iba, Faltaba la Sostenibilidad](#cómo-iba-faltaba-la-sostenibilidad)
- [Cómo Iba, GitHub Organización, Global Docs, y Slack](#cómo-iba-github-organización-global-docs-y-slack)
- [Tradicional Proyecto Django](#tradicional-proyecto-django)
- [Tradicional Django Apps](#tradicional-django-apps)
- [Pinax CLI](#pinax-cli)
- [Pinax CLI](#pinax-cli-1)
- [Pinax CLI](#pinax-cli-2)
- [Archivo `projects.json`](#archivo-projectsjson)
- [Pinax Starter Projects](#pinax-starter-projects)
- [Pinax Apps en Starter Projects](#pinax-apps-en-starter-projects)
- [Pinax Apps Independiente](#pinax-apps-independiente)
- [Un Release Típico](#un-release-típico)
- [Manteniendo Pinax Apps](#manteniendo-pinax-apps)
- [Pinax App Código](#pinax-app-código)
- [Profesional Nivel Configs](#profesional-nivel-configs)
- [Actualizar la Test Matrix](actualizar-la-test-matrix)
- [pyenv y tox](#pyenv-y-tox)
- [Python/Django Release Notes](#pythondjango-release-notes)
- [Actualizar SemVer Versión y Change Log](#actualizar-semver-versión-y-change-log)
- [Tag y Publish](#tag-y-publish)
- [20.07 (veinte punto cero siete) Release](#2007-veinte-punto-cero-siete-release)
- [Algunas Lecciones Aprendidas de Pinax](#algunos-lecciones-apendidas-de-pinax)
- [Simplificado, Autoservicio, Autosostenible](#simplificado-autoservicio-autosostenible)
- [Mejoras Importantes que He Dirigido](#mejoras-importantes-que-he-dirigido)
- [La Importancia de Publicidad](#la-importancia-de-publicidad)
- [Agotamiento (Burnout)](agotamiento-burnout)
- [Reducir el Alcance](#reducir-el-alcance)
- [Automatización Adicional](#automatización-adicional)
- [Herramientas Específicas de Python](#herramientas-específicas-de-python)
- [Centralizar el Acceso y el Conocimiento](#centralizar-el-acceso-y-el-conocimiento)
- [Gestión de Mantenedores Voluntarios](#gestión-de-mantenedores-voluntarios)
- [Pensamientos Finales](#pensamientos-finales)
- [Cuando Necesites Ayuda](#cuando-necesites-ayuda)
- [Contrato Social de OS (código abierto)](#contrato-social-de-os-código-abierto)
- [Ventajas de Manteniendo](#ventajas-de-manteniendo)
- [Cenar Con Guido](cenar-con-guido)
- [Vale la pena? Si :)](#vale-la-pena-si-)
- [Vale la pena? Si :)](#vale-la-pena-si--1)
- [Muchas Gracias :)](#muchas-gracias)
- [Contactarme :)](#contactarme)
- [Preguntas y Respuestas](#preguntas-y-respuestas)

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Slides and Script

The script is a general outline and varies somewhat from what was said during the talk.

<table>

<tr><td width="30%">

![Slide 1](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_0.jpg)

</td><td>

### Desmitificando el Mantenimiento
 
* Hola a todos
* Mi nombre es Katherine Michel. Mi apodo es Kati
* El nombre de mi charla es “Desmitificando el Mantenimiento”
    
</td></tr>


<table>

<tr><td width="30%">

![Slide 2](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_1.jpg)

</td><td>

### Mis Afiliaciones
 
* Algunas de mis afiliaciones
* He sido Mantenedora y Release Manager de Pinax a tiempo parcial durante algunos años
* He sido consultora de Python/Django/React para la Wharton School
* He enseñado algo de programación introductoria en Python a través de Stanford
* Soy miembro de la Junta de DEFNA (Django Events Foundation North America) 
* Soy Web Chair del sitio DjangoCon US 
 
</td></tr>


<table>

<tr><td width="30%">

![Slide 3](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_2.jpg)

</td><td>

### Objetivos de la Charla
 
* Objetivos de la charla
* Voy a hablar de
* Los fundamentos del manteniendo
* Un caso de estudio de manteniendo el Sitio Web de DjangoCon US
* Un caso de estudio de manteniendo Pinax
* Y algunos lecciones aprendidas
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 4](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_3.jpg)

</td><td>

### Supuestos
 
* Yo tengo un supuesto que
* Entiendes:
* Los fundamentos de usando GitHub
* Y los fundamentos de contribución
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 5](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_4.jpg)

</td><td>

### Iniciandonos en la Colaboración y la Revisión de Código en GitHub
 
* Si necesitas más información sobre estos temas
* Tengo una charla llamada “Get a Jumpstart on Collaboration and Code Review in GitHub” 
* Hay algunos versiones en mi cuenta de GitHub 
* Por desgracia, solo está en Ingles
* Quizás en el futuro voy a traducirlas
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 6](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_5.jpg)

</td><td>

### Vocabulario: GitHub Documentación en Español
 
* GitHub tiene documentación en Español
* Yo voy a usar vocabulario similar
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 7](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_6.jpg)

</td><td>

### Terminología de GitHub
 
* Algunos ejemplos de la terminología de GitHub que voy a usar
* Repo, branch
* Fork, clone, commit, submit
* Issue, pull request (PR)
* Fetch, push, update, merge, delete
* Community health files, templates
* Change log
* Si necesitas ayuda con este vocabulario, yo recomiendo que mires la Github documentación en Español

https://docs.github.com/es
https://github.blog/2019-09-16-product-documentation-now-available-in-spanish/
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 8](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_7.jpg)

</td><td>

### El mantenimiento no es sólo acerca de código
 
* Primero
* Es importante darse cuenta que el mantenimiento no es solo sobre código
* Es también sobre
* Personas
* Comunidad
* Proceso
* Comunicación
* Amabilidad
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 9](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_8.jpg)

</td><td>

### Intenta ponerte en Los Zapatos del Colaborador
 
* Intenta poner mismo en los zapatos del colaborador
* Hace contribución el más fácil posible
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 10](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_9.jpg)

</td><td>

### GitHub Guías de Código Abierto: “Una Lista de Verificación Antes de Contribuir”
 
* Una manera que saber si quieres contribuir a un proyecto
* Es usar las Guías de Código Abierto
* Hay una lista de verificación antes de que contribuir
* Los mantenedores pueden usarlo para mejorar sus proyectos

https://opensource.guide/es/how-to-contribute/#una-lista-de-verificaci%C3%B3n-antes-de-que-contribuyas
https://opensource.guide/es/
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 11](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_10.jpg)

</td><td>

### Algunos Signos de un Proyecto Saludable
 
* Algunos Signos de un Proyecto Saludable
* Hay un ambiente de bienvenida
* Hay actividad reciente
* Los mantenedores responden rápidamente
* Los mantenedores reducen los issues y pull requests
 
</td></tr>


<table>

<tr><td width="30%">

![Slide 12](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_11.jpg)

</td><td>

### Proceso Ideal
 
* Un proceso ideal
* El futuro colaborador
* Encontra proyecto
* Está de acuerdo con el Code of Conduct
* Lea CONTRIBUTING.md
* Usa docs, issue y pull request templates
* Submit issue o pull request
* El mantenedor responde rápidamente
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 13](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_12.jpg)

</td><td>

### Community Health Files
 
* El primero paso es que el mantenedor cree los community health files
* README.md- da información general del proyecto
* LICENSE- habla de los términos legales bajo los cuales puedes contribuir y usar el código
* CODE_OF_CONDUCT.md- un conjunto de reglas que describen las expectativas y responsabilidades de los colaboradores
* CONTRIBUTING.md- da información sobre cómo contribuir
 
</td></tr>


<table>

<tr><td width="30%">

![Slide 14](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_13.jpg)

</td><td>

### Documentación
 
* La documentación es muy importante para el futuro éxito de un proyecto
* GitHub hizo una encuesta sobre el código abierto en 2017 (dos mil diecisiete) y descubrieron que la documentación es...
* Muy valorado
* A menudo se pasa por alto
* Y un medio para establecer comunidades inclusivas y accesibles

-De la encuesta sobre código abierto de GitHub de 2017

http://opensourcesurvey.org/2017/#insights
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 15](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_14.jpg)

</td><td>

### Cómo Los Colaboradores Contribuyen
 
* He hecho un par de diagramas que yo espero les den una idea del proceso ques es trabajar localmente para un colaborador frente un mantenedor
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 16](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_15.jpg)

</td><td>

### Modelo de Repo Comparido
 
* El Modelo de “Shared Repository” (o repo compartido en Español) es normalmente usado en una organización GitHub 
* Un mantenedor no necesita usar un fork, porque tiene “write permission” (o permiso de escritura en Español) al repo
* El mantenedor puede clonar el repo (usando el shared repo URL)
* El mantenedor puede realizar sus cambios, probablemente en una branch, y hacer ​​push a los cambios en el repo
* El mantenedor puede crear un pull request (directamente en el GitHub Organization)
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 17](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_16.jpg)

</td><td>

### Modelo Fork y Pull
 
* El Modelo Fork y Pull es normalmente usado en las cuentas del colaborador. Puesto que el colaborador no tiene “write permission”, necesita hacer un fork del repo en su cuenta de usuario, donde el colaborador tiene estos permisos. 
* El colaborador hace un fork al repo
* El colaborador clona el fork (usando el fork URL)
* El colaborador puede hacer su cambio, luego submit los cambios al fork (probablemente en una branch)
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 18](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_17.jpg)

</td><td>

### Crear un Pull Request
 
* Cuando este listo, el colaborador crea el pull request (a la GitHub Organization)
* La compare branch debe ser la branch del colaborador.
* La base branch debe ser la branch en la que se deben hacer merge a los cambios
* El colaborador crea un pull request y luego tal vez una descripción
* El colaborador hace clic en “Create Pull Request” (o "Crear Pull Request" en Español) 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 19](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_18.jpg)

</td><td>

### Revisando un Pull Request
 
* Ahora vamos a cambiar a la perspectiva del mantenedor
* Cuando un colaborador crea un pull request, los mantenedores del repo van a recibir una notificación del navegador o correo electrónico para informarles que hay un pull request.
* Siga el enlace a la página del pull request en el navegador
* Revise la información sobre el pull request. Puedes ver el título y la descripción y hacer clic en el enlace "Files changed" (o “Archivos cambiados” en Español) para ver todos los cambios realizados.
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 20](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_19.jpg)

</td><td>

### Revisando un Pull Request
 
* Ahora vamos a cambiar a la perspectiva del mantenedor
* Cuando un colaborador crea un pull request, los mantenedores del repo van a recibir una notificación del navegador o correo electrónico para informarles que hay un pull request.
* Siga el enlace a la página del pull request en el navegador
* Revise la información sobre el pull request. Puedes ver el título y la descripción y hacer clic en el enlace "Files changed" (o “Archivos cambiados” en Español) para ver todos los cambios realizados.
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 21](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_20.jpg)

</td><td>

### Pull Request: Línea Comando
 
* Hay algunos situaciones cuando necesitas hacer fetch una pull request branch en tu entorno de desarrollo local para poder ejecutar el código o ejecutar una test o trabajar en el código para poder hacer merge.
* Cuando haces clic en el enlace “command line instructions”, se abrirá un conjunto de instrucciones sobre cómo revisar y (posiblemente) hacer merge al pull request en tu entorno de desarrollo local.
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 22](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_21.jpg)

</td><td>

### Pull Request: Opciones Si No Ejecutas el Código Localmente
 
* Si no se necesita ningún cambio o el cambio se puede hacer en el navegador
* Realice el cambio en el navegador
* Haga clic en merge
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 23](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_22.jpg)

</td><td>

### Pull Request: Pull Request: Opciones Si Ejecutas el Código Localmente
 
* Si no se necesita ningún cambio, vuelve al navegador y haz clic en merge
* Si se necesita un cambio, pídale al colaborador que lo haga, o submit mismo la actualización, y luego haga clic en merge
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 24](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_23.jpg)

</td><td>

### Pull Request: Comandos
 
* Si necesitas ejecutar el código localmente y sigues el conjunto de instrucciones, harás merge manualmente a la pull request branch localmente a la que se pretende merge y push a esa branch en GitHub
* Yo no hago eso. 
* Sólo sigo la parte de las instrucciones en negro para obtener la branch
* Yo ignoro las instrucciones en rojo
* Si verifico que el cambio puede ser merged, vuelvo a la página de GitHub pull request en el navegador y hago clic en merge
* Por un lado, la `main` branch a menudo puede estar protegida
* Además, en el navegador, puedes simplemente pulsar un botón para revertir el pull request
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 25](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_24.jpg)

</td><td>

### Flujo de Trabajo: GitHub Flow
 
* El flujo de trabajo que hemos estado usando es básicamente GitHub Flow. Consiste en merging pull requests en un `main` branch.
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 26](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_25.jpg)

</td><td>

### Flujo de Trabajo: Variación
 
* Algunos proyectos usan ambos `main` y `develop` branches. 
* En esta situación, los desarrolladores hacen un merge de sus trabajo en el `dev` branch. Eventualmente, el `dev` branch es merged en el `main` branch. Si el `main` branch se despliega, los cambios están activos 

</td></tr>


<table>

<tr><td width="30%">

![Slide 27](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_26.jpg)

</td><td>

### Algunas Recomendaciones
 
* Algunas recomendaciones
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 28](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_27.jpg)

</td><td>

### Licenses
 
* Licencias no copyleft
* Licencias Copyleft 
* Licencias éticas
* GitHub “Choose a License” (Elija una Licencia)
* Una license muy comun es la MIT license
* La MIT License es non-copyleft y da al usuario mucha libertad en el uso del código, incluyendo el hacer el código privado
* Una Copyleft License suele exigir que el código siga siendo de código abierto
* Por esta razón, los copyleft licenses pueden crear un riesgo del negocio
* Las “ethical licenses” (o licencias éticas) son un tema muy interesante en mi opinión
* Pero a veces los términos de las “ethical licenses” son difíciles de hacer cumplir
* GitHub tiene un excelente recurso llamado “Choose a License” (o Elija una Licencia)
* En el appendix esta tabla con una comparación de licenses: https://choosealicense.com/appendix/
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 29](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_28.jpg)

</td><td>

### Seguridad
 
 * Un aspecto difícil de la seguridad del software es que
* El supply chain del software es todo lo que compone su código,
* Incluidas el GitHub organization, el proyecto, y las personas que tienen acceso
* E incluidas las dependencias y el alojamiento externo
* Por ello, un proyecto necesita un plan de seguridad con varias partes
* Algunos ejemplos
* Para el nivel individual… autenticación de 2 (dos) factores, acceso limitado 
* Para el nivel de organización… scanning de secretos y dependencias para las vulnerabilidades
* Para el nivel de proyecto… nuevas releases que incorporan los últimos parches de seguridad y un plan de seguridad del proyecto con información sobre cómo informar de las vulnerabilidades
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 30](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_29.jpg)

</td><td>

### CHAOSS: Métricas de Código Abierto para Evaluar la Salud de Tu Proyecto
 
* Si quieres empezar a medir la salud de tu proyecto
* Hay métricas especiales
* CHAOSS, por ejemplo, es una colección de métricas que puedes utilizar para crear un plan de salud para tu proyecto
https://chaoss.community/metrics/
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 31](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_30.jpg)

</td><td>

### Más Funciones Útiles de GitHub
 
* Una lista para futuras referencias de más funciones útiles de GitHub
* Issue y pull request templates y Global Community Health File Repo
* Project Management: Project Boards, milestones, issues, labels
* Métodos de Comunicación: Wiki, GitHub Pages/Jekyll
* Descubribilidad: labels/triaging, topics, publicaciones de blog
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 32](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_31.jpg)

</td><td>

### Un Caso de Estudio: Sitio Web de DjangoCon US
 
* Un caso de estudio: Sitio Web de DjangoCon US
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 33](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_32.jpg)

</td><td>

### Puntos Clave
 
* DjangoCon US Sitio de Web ha estado
* Una oportunidad para:
* Aprender los fundamentos de manteniendo
* Crecer en una comunidad de colaboradores

</td></tr>


<table>

<tr><td width="30%">

![Slide 34](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_33.jpg)

</td><td>

### DjangoCon US: La Conferencia Con Un Corazón
 
* Pasé mucho tiempo mirando a través de GitHub
* Me di cuenta que muchas conferencias están buscando voluntarios quien pueden mantener sus sitios web
* Entonces, me involucré con DjangoCon US
* Esta es una foto de mi con algunos de los otros organizadores
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 35](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_34.jpg)

</td><td>

### Los Sitios que He Supervisado
 
* Quería llevar mi conocimiento de GitHub a un nivel superior al aprender cómo ser un mantenedor
* Entonces yo pregunté la DjangoCon US Chair si podía ser un mantenedor del sitio web
* Ella dijo "seguro" y me invitó a ser el web Chair del sitio y yo acepté
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 36](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_35.jpg)

</td><td>

### Los Pull Requests Más Fácil (sesenta y siete commits, veinte ocho pull requests)
 
* Una de las estrategias que me ayudó a aprender el proceso de mantener el software
* El otro mantener me dejó los pull requests más fáciles
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 37](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_36.jpg)

</td><td>

### Yo aprendí como…
 
* Yo aprendí como…
* Hacer fetch a un pull request localmente
* Ejecutar el código
* Hacer push a una actualización desde un fork a un pull request
* Hacer merge a un pull request localmente
* Hacer push a un pull request a una `main` branch
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 38](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_37.jpg)

</td><td>

### Aumento en el Número de Colaboradores
 
* Porque un sitio web Jekyll es muy fácil de usar
* Pude aprender los fundamentos de ser un mantenedor
* Y también pudimos aumentar drásticamente el número de colaboradores
* De 23 (veinte trés) en 2016 (dos mil dieciséis)
* A la 65 (sesenta y cinco) en 2020 (dos mil veinte)
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 39](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_38.jpg)

</td><td>

### Me Convertí en Mentor
 
* Creé los nuevos documentos colaboradores
* Yo ayudé a algunos principiantes a hacer sus primeras contribuciones
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 40](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_39.jpg)

</td><td>

### Algunas Lecciones Aprendidas del Sitio Web de DjangoCon US
 
* Algunas lecciones aprendidas del Sitio Web de DjangoCon US
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 41](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_40.jpg)

</td><td>

### Seguridad Psicológica
 
* Es ideal aprender en un ambiente que ofrece seguridad psicológica
* Afortunadamente para mí, no podría haberme topado con una comunidad más agradable
 
</td></tr>


<table>

<tr><td width="30%">

![Slide 42](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_41.jpg)

</td><td>

### Los Errores Desaparecen en el Historial de Git
 
* Está bien tener una mentalidad de principiante; cometer errores, seguir mejorando 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 43](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_42.jpg)

</td><td>

### La Perspectiva del Principiante es Valiosa
 
* La perspectiva del principiante es valiosa
* Es posible que los veteranos del proyecto no pueden verlo con los ojos de un principiante
* Un principiante puede mejorar el proyecto para la próxima persona
* Por ejemplo: crear docs de instalación
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 44](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_43.jpg)

</td><td>

### Logrando Resultados 10x (diez veces)
 
* Personas con frecuencia hablan sobre el concepto del 10x (diez veces) resultados
* Es importante recordar que algunas de los habilidades que crean el 10x (diez veces), no involucran escribir código
* Un pocos ejemplos:
* Mantener los docs
* Hacerle publicidad al proyecto
* Ser mentor de los colaboradores
 
</td></tr>


<table>

<tr><td width="30%">

![Slide 45](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_44.jpg)

</td><td>

### Mi Primera Charla Tech
 
* Cuando aprendes una nueva habilidad, tienes la oportunidad de enseñar otras personas y impactar al mundo
* Después yo aprendí cómo mantener el DjangoCon US sitio web yo cree una charla sobre cómo hacerlo
* Es uno de mis objetivos que ayudar otras mujeres ser mantenedores
* Yo di la charla llamada “Get a Jumpstart on Collaboration and Code Review in GitHub” por primera vez en DjangoCon US 2017 (dos mil diecisiete)
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 46](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_45.jpg)

</td><td>

### Un Caso de Estudio: Pinax
 
* Un caso de estudio: Pinax
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 47](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_46.jpg)

</td><td>

### Vocabulario de Pinax
 
* Yo voy a usar alguno vocabulario especial por el caso de estudio de Pinax
* Un Pinax Starter Project es un Proyecto de Inicio de Pinax
* Una Pinax app es una aplicación Pinax
* El Pinax CLI (Command line interface) es una interfaz de línea de comandos
* Los Pinax Themes son Temas Pinax
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 48](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_47.jpg)

</td><td>

### Vocabulario de Testing
 
* Yo voy a usar alguno vocabulario especial de testing
* Test es prueba
* Test matrix es matriz de pruebas
* Continuous integration es integración continua
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 49](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_48.jpg)

</td><td>

### Vocabulario de Packaging
 
* Yo voy a usar alguno vocabulario especial de packaging
* Package es paquete
* Release notes son notas de versión
* Tag es etiqueta
* Publish es publicar
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 50](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_49.jpg)

</td><td>

### Puntos Clave
 
* Pinax ha estado
* Una oportunidad para:
* Mantener una librería compleja de Django
* Convertirte en un Python package release manager
* Aprenda a lidiar con el síndrome de lavadero
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 51](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_50.jpg)

</td><td>

### Fui Contratado por Eldarion para Mantener Pinax
 
* En el otoño de 2017 (dos mil diecisiete), según mi experiencia como mantenedor de DjangoCon US 2017 (dos mil diecisiete)
* Me contrataron para trabajar en Pinax
* Pinax es una librería de código abierto de Starter Projects, apps y temas reutilizables de Django para crear sitios web  
 
</td></tr>

<table>

<tr><td width="30%">

![Slide 52](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_51.jpg)

</td><td>

### Nació Pinax: 2008 (Dos Mil Ocho)
 
* Un poco de historia sobre Pinax
* Cuando me contrataron, habían pasado alrededor de 10 (diez) años desde que nació la idea de Pinax
* Django había sido de código abierto en 2005 (dos mil cinco)
* En marzo de 2008 (dos mil ocho), en PyCon US en Chicago, algunos entusiastas de Django comenzaron trabajando en Pinax
* Estaban creando Pinax para resolver su propio problema

</td></tr>


<table>

<tr><td width="30%">

![Slide 53](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_52.jpg)

</td><td>

### Cómo Comenzó
 
* Se encontraron reutilizando algunos de los mismos patrones de código mientras creaban sitios web con Django
* Así que comenzaron a abstraer estos patrones en Starter Projects, aplicaciones y temas reutilizables de Django
* Ellos querían crear una libreria de desarrollo web reutilizable que hiciera elecciones y compromisos
* Esta libreria les permitiría centrarse en las features en la parte superior de la pila
* De esa manera, podrían pasar de la idea del sitio web a la realización rápidamente, en lugar de reinventar la rueda
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 54](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_53.jpg)

</td><td>

### Cómo Comenzó
 
* Entonces, ¿cuál era el estado de Pinax cuando me contrataron?
* Es bastante común, desde el principio hasta ahora, que las personas descubran Pinax y digan "es todo lo que siempre soñaron"
* En esta diapositiva hay uno de los primeros tweets sobre Pinax ... alguien dice "Pinax es todas las ideas que he tenido"
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 55](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_54.jpg)

</td><td>

### Cómo Iba, 80 (Ochenta) Proyectos y Apps
 
* En 2017 (dos mil diecisiete), Pinax había crecido hasta convertirse en un gran grupo de proyectos y apps Django de calidad profesional y interdependientes
* Incluyendo starter projects con Pinax apps preinstalado y una Pinax CLI para instalarlos
* Y tests sofisticadas, packaging y configuraciones de continuous integration
* El Pinax GitHub Organización tiene aproximente 80 (ochenta) repos
* Esta diapositiva incluye muchas de los más populares

</td></tr>


<table>

<tr><td width="30%">

![Slide 56](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_55.jpg)

</td><td>

### Cómo Iba, Faltaba la Sostenibilidad
 
* Pero ... faltaba la sostenibilidad
* Muchos de los autores originales habían seguido adelante
* Sin una estrategia para hacer Pinax más facil de mantener, los mantenedores comenzaron a sufrir agotamiento (o burnout en English)
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 57](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_56.jpg)

</td><td>

### Cómo Iba, GitHub Organización, Global Docs, y Slack
 
* Además de la GitHub Organización Pinax ahora tenía un sitio de global docs y un Pinax Slack canal para comunidad y apoyar
* También había docs específicos de la aplicación en repos individuales
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 58](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_57.jpg)

</td><td>

### Tradicional Proyecto Django
 
* Ahora, yo voy a hablar sobre GitHub y el entorno de desarrollo local y cómo funciona Pinax
* En tu entorno de desarrollo local, si estás iniciando un proyecto tradicional de Django...
* Necesitarás tener Django instalado y normalmente estarías usando un virtual environment
* Ejecutas el comando `` `django-admin startproject``` en la terminal para iniciar un proyecto
* El proyecto contiene la configuración global y otras configuraciones para tu sitio web
* Los proyecto template archivos creados en el directorio están desde el Django package
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 59](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_58.jpg)

</td><td>

### Tradicional Django Apps
 
* Luego, ejecutas un comando adicional para agregar una o más aplicaciones a tu proyecto
* Cada aplicación contiene una funcionalidad especial (por ejemplo, una aplicación de "blog" para una parte de blog de tu sitio web)
* Los aplicación template archivos creados también están desde el Django package
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 60](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_59.jpg)

</td><td>

### Pinax CLI
 
* Con Pinax, puedes instalar Pinax CLI
* Puedes usar comandos para obtener información sobre Pinax (como una lista de starter projects o apps)
* Pinax Starter Projects son básicamente proyectos personalizados de Django
* Estos ya tienen alguna funcionalidad integrada y cuando usando los no es necesario que empieces de cero con un proyecto tradicional de Django
* Lo mismo con Pinax Apps
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 61](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_60.jpg)

</td><td>

### Pinax CLI
 
* También puedes usar Pinax CLI para instalar un Pinax Starter Project en lugar del proyecto tradicional de Django
* Hay un comando especial de Pinax CLI para hacer esto `pinax start <pinax-starter-project> <tu-proyecto>
* Cuando Pinax CLI ejecuta este comando
* El Pinax CLI usa el mismo ```startproject``` comando usado para instalar un proyecto tradicional de Django
* Pero Django llama lo desde el base de código de Pinax CLI
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 62](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_61.jpg)

</td><td>

### Pinax CLI
 
* El URL del starter project se pasa como un parámetro
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 63](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_62.jpg)

</td><td>

### Archivo `projects.json`
 
* La URL conduce a un archivo (projects punto json) `projects.json` que proporciona la dirección del archivo tar en el repo de los Pinax Starter Projects
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 64](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_63.jpg)

</td><td>

### Pinax Starter Projects
 
* Los starter projects están en uno repo
* Cada starter project está en una branch individual
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 65](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_64.jpg)

</td><td>

### Pinax Apps en Starter Projects
 
* Cada starter project contiene las Pinax apps relevantes, para ser instaladas desde PyPI (el Python Package Index)
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 66](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_65.jpg)

</td><td>

### Pinax Apps Independiente
 
* Alternativamente, puedes usar Pinax apps independiente de cualquier Pinax Starter Project
* Puedes encontrar las buscando “pinax” en PyPI
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 67](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_66.jpg)

</td><td>

### Un Release Típico
 
* Un release típico
* Actualizar la test matrix
* Agregar nuevas funciones
* Implementar nuevas mejores prácticas
* Arreglar las depreciaciones
* Mejorar la documentación
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 68](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_67.jpg)

</td><td>

### Manteniendo Pinax Apps
 
* Algunos detalles importantes sobre manteniendo las Pinax apps
* Usamos GitHub Flow flujo de trabajo
* Para el versionado semántico
* Usamos CalVer en el release-nivel (año punto mes)
* Usamos SemVer en el aplicación-nivel (major punto minor punto patch)

</td></tr>


<table>

<tr><td width="30%">

![Slide 69](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_68.jpg)

</td><td>

### Pinax App Código
 
* Cada Pinax app base de código vive en un GitHub repo
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 70](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_69.jpg)

</td><td>

### Profesional Nivel Configs
 
* Cada aplicación repo tiene configuraciones del nivel profesional usado por mantener el código actualizado
* CircleCI es para continuous integration
* (setup punto py) `setup.py` contiene packaging configs
* `tox` es para testing la Python/Django versiones matrix
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 71](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_70.jpg)

</td><td>

### Actualizar la Test Matrix
 
* Cuando hacemos un release, actualizamos la test matrix para apoyar las últimas versiones de Python y Django
* En mi release plan, yo documentó un fragmento de la test matrix para copiar y pegar en los archivos de la aplicación
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 72](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_71.jpg)

</td><td>

### pyenv y tox
 
* El proceso es que... 
* Yo clone el Pinax app repo localmente, y creo una branch nueva
* Yo actualizo la test matrix en la branch
* Hay una herramienta llamada pyenv que puedes usar para instalar múltiples versiones globales de Python localmente
* Cuando se ejecuta tox, tox puede usar estas versiones globales para comprobar la compatibilidad del código de la Pinax app con las nuevas versiones de Python y Django
* Cuando hay una incompatibilidad, tox le mostrará el error en rojo
* Cuando todas las tests pasen… se mostrará en verde al final
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 73](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_72.jpg)

</td><td>

### Python/Django Release Notes
 
* Mientras se solucionan estas incompatibilidades
* Las Python y Django release notes explican todos los cambios realizados en el base de código de Python/Django en el release
* Puedes usar las release notes para entender qué actualizaciones debes hacer para cumplir
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 74](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_73.jpg)

</td><td>

### Actualizar SemVer Versión y Change Log
 
* Cuando todas las test matrix y otras actualizaciones están completos
* Querrá actualizar la versión de SemVer en el (setup punto py) `setup.py`
* Y también las versiones en el (setup punto py) `setup.py` metadatos y README
* Actualizar el Change Log en el README
* Estas son algunas de las piezas varios de metadatos
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 75](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_74.jpg)

</td><td>

### Tag y Publish
 
* Entonces, vaya a la "tags" área del repo
* Draft una release nueva
* Incluye un enlace al Change Log
* Ejecutas un proceso localmente para package la aplicación
* He documentado este proceso en el repo punto github en el archivo RELEASE.md
* Y publish el package en PyPI
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 76](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_75.jpg)

</td><td>

### 20.07 (veinte punto cero siete) Release
 
* En Julio 2020 (dos mil veinte), supervisé la finalización de una Pinax release importante
* Incluía aproximadamente 28 (veinte ocho) aplicaciones y notablemente discontinuamos el soporte para Python 2.7 (dos punto siete)
* Fue un hito importante para mí, personal y profesionalmente
* Inicié el release, gestioné el proceso de principio a fin, creé el plan del release, supervisé el trabajo de otros, actualicé 10 (diez) aplicaciones yo mismo, merged todos los pull requests, y tagged y published los packages

</td></tr>


<table>

<tr><td width="30%">

![Slide 77](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_76.jpg)

</td><td>

### Algunas Lecciones Aprendidas de Pinax
 
* Algunas Lecciones Aprendidas de Pinax
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 78](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_77.jpg)

</td><td>

### Simplificado, Autoservicio, Autosostenible
 
* He intentado para solucionar algunos de los problemas críticos de Pinax
* El objetivo en general ha sido implementar cambios para hacerlo más sencillo y autoservicio
* Como resultado, los principiantes, colaboradores y mantenedores podrían ayudarse a sí mismos
* Y por lo tanto, crear una cultura que pueda sostenerse a sí misma
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 79](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_78.jpg)

</td><td>

### Mejoras Importantes que He Dirigido
 
* Mejoras importantes que he dirigido
* Documentación del conocimiento tribal
* Consolidation de docs, en un lugar fácil de encontrar
* Estandarización de las configuraciones entre proyectos
* Creación de docs detallados de release y mantenimiento
* Creación de Community Health Files, incluidas Issue y Pull Request Templates
* Reducción significativa del número de issues y pull requests para estar al día con los nuevos issues y pull requests
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 80](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_79.jpg)

</td><td>

### La Importancia de Publicidad
 
* Una de las lecciones más importantes que he aprendido de Pinax
* A veces es contrario a la intuición
* A veces es importante parar y comunicar tus progresos y planes a la comunidad
* Y pedir ayuda
* Por ejemplo, porque de mis publicaciones de blog, recibí ayuda que fue crucial para completar la última release de Pinax
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 81](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_80.jpg)

</td><td>

### Agotamiento (Burnout)
 
* Hay un peligro real de agotamiento en código abierto
* Es un sujeto triste
* Los autores del código y los mantenedores están generoso 
* A veces trabajan demasiado
* Y, por desgracia, a veces ellos tienen que lidiar con las actitudes negativas de los usuarios del código
* No estoy seguro Pinax va estar saludable y prospere de nuevo
* Pero he aprendido mucho de Pinax
* Yo quiero hablar de algunas maneras de hacer una comunidad autosuficiente
* Para los mantenedores, colaboradores y usuarios
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 82](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_81.jpg)

</td><td>

### Reducir el Alcance
 
* Maneras de reducir el alcance
* Marcar repos como obsoletos
* Archivar repos
* Desactivar issues
* Comunicar que los mantenedores mantienen el código esporádicamente
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 83](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_82.jpg)

</td><td>

### Automatización Adicional
 
* Puedes implementar automatización adicional para reducir la carga de trabajo
* Estos son algunos lugares donde puedes encontrar herramientas de automatización
* GitHub Actions
* GitHub Apps
* Probot: https://probot.github.io/
* Probot es un lugar para encontrar ideas noveles sobre lo que podría ser automatizado
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 84](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_83.jpg)

</td><td>

### Herramientas Específicas de Python
 
* Algunas herramientas de automatización específicas de Python
* Además de pyenv y tox hay
* Coverage.py (coverage punto py)
* isort
* Black
* Restructured Text
* Y muchos otros
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 85](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_84.jpg)

</td><td>

### Centralizar el Acceso y el Conocimiento
 
* Es un problema cuando sólo una persona tiene acceso o conocimiento de un proyecto (por ejemplo, acceso al repo o a PyPI)
* Si la persona deja el proyecto y no entrega el acceso y el conocimiento, es difícil continuar
* En mi opinión es mejor tener una política de centralizar el acceso y estar dispuesto a dar acceso a otras personas
* Una otra forma de este problema es cuando un mantenedor crea una solución única a un problema y es la sóla persona con acceso y conocimiento
* Si la persona pierde el interés, es difícil que otros continúen
* En mi opinión, es mejor evitar las soluciones únicas.
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 86](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_85.jpg)

</td><td>

### Gestión de Mantenedores Voluntarios
 
* Cuando hay riesgo de agotamiento (burnout), es posible dar acceso adicional y limitado a los colaboradores
* Es importante que recordar que es el responsabilidad del mantener de asegurar el código
* Puedes dar permisos selectivos (por ejemplo, sólo dar acceso a un repo individual)
* Proteger branches (por ejemplo, nadie puede delete una branch importante)
* Requerir revisiones de pull requests (por ejemplo, más de una persona contribuye a la revisión antes merging) 
* Usar status checks
* En el peor de los casos, puedes revert un pull request, si es necesario
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 87](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_86.jpg)

</td><td>

### Pensamientos Finales
 
* Algunos pensamientos finales
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 88](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_87.jpg)

</td><td>

### Cuando Necesites Ayuda
 
Es inevitable que vas a tener momentos de frustración y vas a necesitar ayuda... aquí están algunos lugares donde puedes encontrar ayuda
* Google
* Stack Overflow
* GitHub docs
* Git docs
* Atlassian y GitLab docs
  
</td></tr>

  
<table>

<tr><td width="30%">

![Slide 89](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_88.jpg)

</td><td>

### Contrato Social de OS (código abierto)
 
* Brett Cannon (un Python Core Dev) ha hablado del “contrato social” del código abierto
* Los mantenedores de código abierto deben la comunidad literalmente nada
* Los autores de Pinax no tenían hacer sus código abierto y mantenerlo
* Ellos no tenían que responder a las innumerables preguntas que respondieron
* Es importante recordar la generosidad de los mantenedores de código abierto
  
</td></tr>
  
  
<table>

<tr><td width="30%">

![Slide 90](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_89.jpg)

</td><td>

### Ventajas de Manteniendo
 
* Hay muchas ventajas del mantenimiento
* Es una oportunidad para… 
* Aprender habilidades técnicas
* Encontrar nuevas oportunidades profesionales
* Asistir a conferencias
* Conocer personas inteligentes e interesantes que construye aplicaciones increíbles
* Viajar a lugares increíbles
  
</td></tr>
      
  
<table>

<tr><td width="30%">

![Slide 91](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_90.jpg)

</td><td>

### Cenar Con Guido
* En PyCascades 2020 (dos mil veinte), yo tuve la oportunidad de cenar con Guido, el creador del lenguaje de programación Python
* El nos contó algunas historias sobre los primeros días de Python
* Fue una noche mágica
* Atribuyo directamente este tipo de experiencia al código abierto

</td></tr>
  
  
<table>

<tr><td width="30%">

![Slide 92](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_91.jpg)

</td><td>

### Vale la pena? Si :)
 
* Durante Maintainer Week de GitHub (o Semana del Mantenedor)
* Yo vi este tweet de Mfon... sus contribuciones fueron críticas para ayudarme a completar el 20.07 (veinte punto cero siete) release
  
</td></tr>
  
  
<table>

<tr><td width="30%">

![Slide 93](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_92.jpg)

</td><td>

### Vale la pena? Si :)
 
* Veyendo la differencia mi trabaja hizo para él y descubriendo que él considera me una amiga muy buena es muy especial para mí
* Las palabras él dijo inmediatamente hicieron que valiera la pena
* Suddenamente yo realizado...
* En el corazón del código abierto están las relaciones yo he formado con las personas
* Voy a tenerlas por el resto de mi vida
  
</td></tr>
  
  
<table>

<tr><td width="30%">

![Slide 94](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_93.jpg)

</td><td>

### Muchas Gracias :)
 
* Gracias a Ricardo Diaz Rincon por revisar mi charla
* Si hay algún error, es el mío
  
</td></tr>
  
  
<table>

<tr><td width="30%">

![Slide 95](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_94.jpg)

</td><td>
 
### Contactarme :)
 
* Por supuesto, puedes contactarme por más información
  
</td></tr>
  
  
<table>

<tr><td width="30%">

![Slide 96](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_95.jpg)

</td><td>

### Preguntas y Respuestas
 
* Ahora, estoy lista para las Preguntas y Respuestas
* Muchas gracias a todos

</td></tr>
  
</table>

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Attribution

The style of this transcript is heavily inspired by:

* Ana Balica's ([Twitter](https://twitter.com/anabalica), [GitHub](https://github.com/ana-balica)) transcript of her [Humanizing among coders](https://ana-balica.github.io/2017/05/28/humanizing-among-coders/) keynote for [PyCon CZ 2016](https://cz.pycon.org/2016). 
* Honza Javorek's ([Twitter](https://twitter.com/honzajavorek), [GitHub](https://github.com/honzajavorek)) transcript of Anna Ossowski's ([Twitter](https://twitter.com/OssAnna16), [GitHub](https://github.com/OssAnna16)) keynote [Be(Come) A Mentor! Help Others Succeed!](https://github.com/honzajavorek/become-mentor) for [PyCon CZ 2017](https://cz.pycon.org/2017/). 

Thank you!

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Contact Kati

* Email: kthrnmichel@gmail.com
* GitHub: https://github.com/KatherineMichel
* Twitter: https://twitter.com/KatiMichel

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Copyright

© 2021 to Present Katherine Michel. All Rights Reserved.
