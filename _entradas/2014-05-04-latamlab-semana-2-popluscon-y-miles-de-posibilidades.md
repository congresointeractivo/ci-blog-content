---
ID: 121
post_title: 'LatamLab Semana 2: #PoplusCon y miles de posibilidades'
author: ciadmin
post_date: 2014-05-04 21:24:21
post_excerpt: ""
layout: post
permalink: >
  http://blog.congresointeractivo.org/latamlab-semana-2-popluscon-y-miles-de-posibilidades/
published: true
---
Esta segunda semana de la pasantía LatamLab fué corta en términos de trabajo, pero infinita en términos de proyectos para el futuro. La conferencia del proyecto Poplus nos permitió conocer a 80 personas de 30 países que están trabajando en los mismos temas y son desarrolladores y potenciales usuarios de los componentes Poplus.

La semana empezó el lunes (dijo el capitán obvio) programando el scrapper de proyectos de ley del Congreso Nacional Argentino. Por suerte la información está bastante accesible, sólo se trata de hace 4 pedidos por proyecto para poder saber el estado actual de tramitación, los firmantes, las comisiones a las que fue girado, y el texto completo. Y digo que esto es simple porque en Paraguay, por ejemplo, es necesario tener configuradas algunas cookies en el pedido y no hay forma de obtener un listado completo, sino que hay que buscar con diferentes keywords y no hay forma de verificar si se están trayendo todos los proyectos. Por suerte en argentina es más sencillo, se pueden recuperar de a 1000 proyectos por ves y de una forma ordenada cronológicamente que no trae complicaciones. Aunque, para ser sinceros, el sitio del senado funciona de forma intermitente y aún no hemos podido relevar los proyectos almacenados allí.

La idea es almacenar esta información en la instancia de BillIt que administra la Fundación Ciudadano Inteligente. BillIt es un componente de Poplus que sirve para almacenar textos, tales como los proyectos de ley.

También hubo avances en el scrapper de diputados, ahora tenemos la información sobre a qué comisión pertenece cada legislador, gracias Alfredo.

Si todo esto no suena maravilloso, es porque no lo es, es sólo la base para poder hacer luego análisis profundos de forma rápida. Durante la conferencia Poplus quedó muy claro que antes de avanzar, desperdiciando el esfuerzo en tareas potencialmente innecesarias, es importante acercarse a los grupos que están necesitando este tipo de herramientas, para poder asegurarnos de que sean realmente útiles para los grupos que queremos apoyar.

Por ejemplo, algo que nuestra investigación ha validado de forma tentativa como necesario sería facilitar que un activista o comunicador de un grupo de interés seleccione rápidamente a quién acercarse y descarte aquellos que serían una pérdida de tiempo (ver <a href="https://docs.google.com/document/d/1MY1-FTbT1301rgH3cjOBbWZU0P1VfqNsB3WAD7_2hPc/edit">escenario 3 en este documento</a>). Por ejemplo, poder saber si un legislador está a favor de los proyectos que promueven la educación pública o más bien a favor de la privatización de la educación.

Para poder hacer eso, necesitamos saber:
<ol>
	<li>Sobre qué tema es un proyecto (ej: educación pública). Esto es sencillo porque podemos saberlo a partir de los giros a comisión y los temas que trata cada comisión. Más o menos.</li>
	<li>Si el proyecto está a favor o en contra de ese tema (ej: a favor de la educación pública). Esto es más difícil. Requiere de un análisis especializado, un gran trabajo de inteligencia artificial o humana, dedicado a comprender cada proyecto.</li>
	<li>Si un legislador determinado votó a favor o en contra del proyecto (ej: si votó en contra, está en contra de la educación pública). Esa información ya la tenemos.</li>
	<li>Hacer un promedio de las diversas posturas de un legislador, de un bloque, de una provincia, etc, para poder tener información fácil de procesar.</li>
</ol>
Fin del ejemplo. Ahora voy a contar sobre la conferencia más en detalle.

Durante la conferencia de Poplus, que se llevó a cabo el martes y miércoles en el campus de la universidad católica de chile.

Conocí gente de todo el mundo: Kenya, Guatemala, Inglaterra, Marruecos, Estados Unidos, Taiwan, Hungría, Alemania, Jamaica, Paraguay, Chile, Argentina, Uruguay, Sudáfrica, Nueva Zelanda, Japón, Estonia y más. La relación entre toda esta gente fué de absoluta cordialidad e incluso creo que algunos prejuicios pudieron ser diluidos.
Conocí proyectos de datos abiertos, lucha contra la corrupción y nuevas formas de colaboración cívica en línea de todos estos países.

Pueden ver el <a href="https://docs.google.com/spreadsheets/d/1oUxV85Kcmv1KfGr8GY4FypjIP2FIBOpMXsJwX67xHSQ/edit#gid=0">listado de asistentes aquí</a> y el <a href="https://popluscon.hackpad.com/">resumen escrito de cada una de las sesiones</a> (un poco desordenado, pero MUY completo)

Uno de los temas más repetidos fué la necesidad de trabajar codo a codo con las poblaciones más vulnerables para descubrir sus necesidades, capacitarlos en el uso de tecnología y asegurarnos así que nuestras aplicaciones sirven a sus objetivos. Creo que la metodología de investigación en experiencia de usuario puede resultar muy útil en esa tarea y por eso fuí anfitrión en <a href="https://popluscon.hackpad.com/User-Experience-UX-research-Session-3-Grey-Room-Wednesday-7aHLWZW2Ak9">una sesión al respecto</a>.

Un comentario interesante al respecto es el de <span data-sheets-value="[null,2,&quot;Tom Steinberg&quot;]" data-sheets-userformat="[null,null,641,[null,0],null,null,null,null,null,null,0,null,0]">Tom Steinberg, director de MySociety en Inglaterra. Él interpreta las revoluciones burguesas del siglo 18 como una reacción de los propietarios y mercaderes para proteger sus bienes de los reyes, esto establece el sistema que tenemos ahora, en el que los grandes comerciantes tienen más poder (generalmente) que los cortesanos y familias reales. Sin embargo aún no se ha logrado la plena participación política de todos los actores sociales, es por eso que debemos trabajar para quienes no forman parte de la elite empoderada. Más detalles en <a href="https://popluscon.hackpad.com/Who-are-we-helping-Impact-Research-w7rPPNto0sk">el documento de la sesión sobre investigación de impacto</a>.</span>

Finalmente, creo que se llegó a algunos consensos sobre los <a href="https://popluscon.hackpad.com/What-Poplus-Components-should-exist-KlZwvmR5ycO">objetivos del proyecto poplus</a> y sobre <a href="https://popluscon.hackpad.com/What-are-Poplus-components-yVemaWdWcmI">qué es un componente</a>. Si bien será necesario seguir trabajando para que esta visión se complete ya que hay varios componentes, por ejemplo VotIt, que serían necesarios para el sitio que estamos construyendo, pero aún no están completos, entonces nosotros trabajaremos como se pueda y luego cuando los estándares estén disponibles veremos de implementarlos.