---
ID: 91
post_title: 'Dataset: Todas las votaciones del Congreso 2001-2013'
author: ciadmin
post_date: 2014-04-11 04:25:12
post_excerpt: ""
layout: post
permalink: >
  http://blog.congresointeractivo.org/dataset-todas-las-votaciones-del-congreso-2001-2013/
published: true
---
El año pasado lanzamos nuestra aplicación de visualización de datos <a href="http://www.decadavotada.com.ar">Década Votada</a>, la cual incluye todas las votaciones del Congreso Nacional, ocurridas en el período de 2001 a 2013 en la Cámara de Diputados y de 2003 a 2012 en la Cámara de Senadores. Esta aplicación fué creada junto a un gran grupo de colaboradores en un hackatón organizado por Hacks/Hackers y ganadora de un <a href="https://source.opennews.org/en-US/articles/decada-votada-news-app-track-voting-records/">premio de Kinght-Mozilla OpenNews</a>.

Estamos muy contentos por este primer paso que hemos dado hacia liberar estos datos, después de la frustrante experiencia de desarrollar nuestro <a href="https://github.com/congresointeractivo/votaciones-parser">scrapper en python</a>, haber conseguido el dataset liberado por <a href="http://www.andytow.com">Andy Tow</a> nos permitió avanzar muchísimo sobre información confiable.

Este dataset se encuentra disponible en Google Fusion Tables, de donde lo descargamos para crear este archivo. Esta es una base de datos pública alojada gratuitamente en los servidores de Google, links para ver cada una de las tablas: <a href="https://www.google.com/fusiontables/DataSource?docid=1OAvsKOSuQE3NzXNKGLwQpBDj9iK3mLweHb8Lcfg">Diputados</a>, <a href="https://www.google.com/fusiontables/DataSource?docid=1GNJAVHF_7xPZFhTc_w4RLxcyiD_lAiYTgVlA0D8">Votaciones diputados</a>, <a href="https://www.google.com/fusiontables/DataSource?docid=1gUTqf8A-nuvBGygRnVDcSftngYZ-z9OvxBs59M0">Bloques diputados,</a> <a href="https://www.google.com/fusiontables/DataSource?docid=1ELTXADIfpiUWfQfL9D8ia8p4VTw17UOoKXxsci4#rows:id=3">Asuntos dipuados</a>, <a href="https://www.google.com/fusiontables/DataSource?docid=1rhy-SIM34RqWGLRnRoA7UeBavBc9GUf6EvnlXZg#rows:id=1">Senadores</a>, <a href="https://www.google.com/fusiontables/DataSource?docid=1vKsuSvTBS_pwgJl7dcbtiMWrOrilaroritbDOOI#rows:id=1">Bloques senado</a>, <a href="https://www.google.com/fusiontables/DataSource?docid=1ihmsVlVwX1sTp4JQ8HK4k07vS8e8_orVY_NvJ9E#rows:id=1">Votaciones senado</a>, <a href="https://www.google.com/fusiontables/DataSource?docid=1M046BCqwBNjxe9CXbcvUUi0JT6HohC8Gq4S7gRM#rows:id=1">Asuntos senado</a>.

Pero hay personas que creen que Google no es el mejor lugar para alojar datos tan sensibles, es por eso que h<span style="line-height: 1.714285714; font-size: 1rem;">oy liberamos este conjunto de datos completo, en formato CSV, comprimido en ZIP, y alojado en nuestro propio servidor (ubicado en nueva york).</span>

DecadaVotadaCSV.zip es un dataset que contiene en 8 tablas:
<ul>
	<li>
<pre><strong>diputados</strong>.csv -  955 filas
Columnas: diputadoID, nombre, distrito

<strong style="font-size: 0.857142857rem; line-height: 1.714285714;">bloques-diputados</strong><span style="font-size: 0.857142857rem; line-height: 1.714285714;">.csv - </span><span style="font-size: 0.857142857rem; line-height: 1.714285714;">170 filas
</span><span style="font-size: 0.857142857rem; line-height: 1.714285714;">Columnas: id_bloque, bloque, color

</span><strong style="font-size: 0.857142857rem; line-height: 1.714285714;">asuntos-diputados</strong><span style="font-size: 0.857142857rem; line-height: 1.714285714;">.csv</span><span style="font-size: 0.857142857rem; line-height: 1.714285714;"> - 1.406 filas
</span><span style="font-size: 0.857142857rem; line-height: 1.714285714;">Columnas: </span><span style="font-size: 0.857142857rem; line-height: 1.714285714;">asuntoId, sesion, asunto, ano, fecha, hora, base, mayoria, resultado, presidente, presentes, ausentes, abstenciones, afirmativos, negativos, votopresidente, titulo, permalink
<strong style="font-size: 0.857142857rem; line-height: 1.714285714;">
votaciones-diputados</strong><span style="font-size: 0.857142857rem; line-height: 1.714285714;">.csv - </span><span style="font-size: 0.857142857rem; line-height: 1.714285714;">359.936 filas
<span style="font-size: 0.857142857rem; line-height: 1.714285714;">Columnas: </span><span style="font-size: 0.857142857rem; line-height: 1.714285714;">asuntoId, diputadoId, bloqueId, voto
<strong style="font-size: 0.857142857rem; line-height: 1.714285714;">
senadores</strong><span style="font-size: 0.857142857rem; line-height: 1.714285714;">.csv - 155 filas
<span style="font-size: 0.857142857rem; line-height: 1.714285714;">Columnas: </span><span style="font-size: 0.857142857rem; line-height: 1.714285714;">diputadoID, nombre, distrito
<strong style="font-size: 0.857142857rem; line-height: 1.714285714;">
bloques-senadores</strong><span style="font-size: 0.857142857rem; line-height: 1.714285714;">.csv</span><span style="font-size: 0.857142857rem; line-height: 1.714285714;"> - 46 filas
</span></span></span></span></span></span><span style="font-size: 0.857142857rem; line-height: 1.714285714;">Columnas: </span><span style="font-size: 0.857142857rem; line-height: 1.714285714;">id_bloque, bloque, color

<strong style="font-size: 0.857142857rem; line-height: 1.714285714;">asuntos-senado</strong><span style="font-size: 0.857142857rem; line-height: 1.714285714;">.csv</span><span style="font-size: 0.857142857rem; line-height: 1.714285714;"> - 1811 filas
<span style="font-size: 0.857142857rem; line-height: 1.714285714;">Columnas: </span><span style="font-size: 0.857142857rem; line-height: 1.714285714;">asuntoId, sesion, asunto, ano, fecha, hora, base, mayoria, resultado, presidente, presentes, ausentes, abstenciones, afirmativos, negativos, votopresidente, titulo, auditoria, permalink

<strong style="font-size: 0.857142857rem; line-height: 1.714285714;">votaciones-senado</strong><span style="font-size: 0.857142857rem; line-height: 1.714285714;">.csv - </span><span style="font-size: 0.857142857rem; line-height: 1.714285714;">130.392
<span style="font-size: 0.857142857rem; line-height: 1.714285714;">Columnas: </span><span style="font-size: 0.857142857rem; line-height: 1.714285714;">asuntoId, diputadoId, bloqueId, voto</span></span></span></span></span></pre>
</li>
</ul>
Para más información, recomendamos leer la <a href="http://decadavotada.com.ar/doc.html">documentación de Decada Votada</a>.

&nbsp;
<h2>Descargar el archivo: <a href="http://www.congresointeractivo.org/data/DecadaVotadaCSV-v2.zip">DecadaVotadaCSV-2.zip</a> (1.554.615 bytes)</h2>
Actualizado, licencia:
<p style="padding-left: 30px;">
<span>Dataset: Todas las votaciones del Congreso 2001-2013</span> por <a href="http://www.congresointeractivo.org/dataset-todas-las-votaciones-del-congreso-2001-2013/" rel="cc:attributionURL">Honorable Congreso de la Nación Argentina, Andy Tow y CongresoInteractivo.org</a> se distribuye bajo una <a href="http://creativecommons.org/licenses/by/4.0/" rel="license">Licencia Creative Commons Atribución 4.0 Internacional</a>.
Basada en una obra en <a href="http://www.hcdn.gov.ar" rel="dct:source">http://www.hcdn.gov.ar</a>.
Permisos que vayan más allá de lo cubierto por esta licencia pueden encontrarse en <a href="http://www.hcdn.gov.ar" rel="cc:morePermissions">http://www.hcdn.gov.ar</a>.</p>
&nbsp;

Pueden <a title="Sobre nosotros" href="http://www.congresointeractivo.org/sobre-nosotros/">contactarnos</a> para informarnos sus intenciones al descargar este dataset, y también para hacernos sugerencias y correcciones sobre el contenido. Esperamos que les resulte de utilidad.