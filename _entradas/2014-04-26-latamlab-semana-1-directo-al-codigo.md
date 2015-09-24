---
ID: 100
post_title: 'LatamLab Semana 1: Directo al código'
author: ciadmin
post_date: 2014-04-26 16:37:07
post_excerpt: ""
layout: post
permalink: >
  http://blog.congresointeractivo.org/latamlab-semana-1-directo-al-codigo/
published: true
---
Estamos transitando los primeros días de trabajo en la Pasantía LatamLab de Fundación Ciudadano Inteligente y Congreso Interactivo. Intentaré no extenderme demasiado, pero estoy tan contento que no puedo. Les contaré algunos avances simbólicos y otros más técnicos, espero que se entusiasmen tanto como nosotros.

Primero algunas fotos:

[gallery ids="107,102,114,106,112,111,113,104,103"]

La Fundación Ciudadano Inteligente es un gran motor de intervención política por la transparencia en Chile, pero además tiene un laboratorio de desarrollo de software con proyección regional y alianzas internacionales.

Algunas cosas fascinantes sobre la Fundación:
<ul>
	<li>Generaron una alianza con un diputado chileno representante del movimiento estudiantil que explotó hace un par de años para proveerle software.</li>
	<li>Llegó un taiwanés, de <a href="http://www.g0v.tw">www.g0v.tw</a>, que tiene un sistema de versionado para proyectos de ley en el que piensa integrar un sistema de anotaciones colaborativas para que pueda verse y comentarse el progreso de los procesos de redacción de proyectos de ley.</li>
	<li>La próxima semana hacen la <a href="http://poplus.org/poplus_event.html">PoplusConf</a> con 80 personas de todo el mundo sobre desarrollo de software cívico.</li>
</ul>
Congreso Interactivo está creando un sitio de monitoreo parlamentario para Argentina, con la ayuda de FCI y los <a href="http://poplus.org/catalogue.html">componentes Poplus</a>, que se desarrollan conjuntamente con <a href="http://mysociety.org">MySociety</a> en Inglaterra y <a href="http://opennorth.ca/">OpenNorth</a> en Canadá.
Nuestro sistema estará basado en el mismo código que <a href="http://www.congresoabierto.cl">www.congresoabierto.cl</a>

Hasta ahora tuvimos cinco días de trabajo conjunto y ya conseguimos conectarnos con la API de <a href="popit.mysociety.org">PopIt</a>, una base de datos de personas y organizaciones que forma parte del proyecto Poplus y está alojado en Inglaterra. Enviamos datos sobre los legisladores nacionales argentinos y bloques.
Está aún un poco precario pero pueden verlo aquí: <a href="http://legisladores-ar.popit.mysociety.org/">http://legisladores-ar.popit.mysociety.org/</a>

Si bien nos preguntamos si alojar los datos en otro país lleva al riesgo de dejar registros en routers intermedios, con la posibilidad de que queden expuestos nuestros usuarios a la supervisión de sus acciones con respecto a datos que pueden ser sensibles, la ventaja de no tener que gestionar la instalación del software es fantástica en esta etapa temprana del desarrollo. Esperamos más adelante poder alojar todos los datos en nuestros servidores locales.

El nivel actual del <a href="https://github.com/congresointeractivo/parser-diputados">scrapper de legisladores</a>  (software para obtener información de páginas web) tiene información de contacto, foto, mandatos, bloques, partidos y provincias. En el futuro nos gustaría agregar la información de declaraciones juradas usando la <a href="http://interactivos.lanacion.com.ar/declaraciones-juradas/">información publicada por LaNación</a>, cargos anteriores gracias a <a href="http://cargografias.org">Cargografías</a> y todo lo que podamos encontrar.

También comenzamos con el scrapper de proyectos de ley, en el momento actual puede obtener un listado de las direcciones de cada proyecto y el texto completo de la página, pero aún no logramos obtener por separado los datos de firmantes, comisiones y texto completo. Esto irá alojado en una instancia de BillIt, otro proyecto de Poplus que sirve para almacenar proyectos de ley.

La estructura es muy extensible, todo es software libre y APIs públicas. De hecho ambos scrappers estuvieron basados en código antiguo desarrollado en el DataFest de 2012 en Buenos Aires en un caso y en las elecciones municipales de 2012 en Santiago.

Aunque los componentes están bastante inmaduros, están mejorando constantemente.
Una parte importante del trabajo es determinar si es necesario hacer mejoras en el software que estamos utilizando, y si corresponde, levantar issues en los githubs de cada proyecto para conseguir los desarrolladores (ingleses, canadienses, etc) actualizaran los proyectos y las documentaciones de sus proyectos.

Creemos que estamos avanzando en un muy bien camino y que esto es el comienzo de una plataforma muy sólida de monitoreo parlamentario.
Gracias a todos por acompañarnos.