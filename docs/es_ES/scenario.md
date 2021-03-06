# Escenarios
**Herramientas → Escenarios**

<small>[Raccourcis clavier/souris](shortcuts.md)</small>

Cerebro real de la automatización del hogar, los escenarios permiten yonteractuar con el mundo real de una manera yonteligente **.

## Ladministración

Allí encontrará la lista de escenarios de su Jeedom, así como las funcionalidades para administrarlos en el mejor de los casos. :

- **Ajouter** : Crea un escenario. El procedimiento se describe en el siguiente capítulo..
- **Deshabilitar escenarios** : Deshabilita todos los escenarios.. Raramente utilizado y a sabiendas, ya que ningún escenario se ejecutará más.
- **Resumen** : La permite tener una visión general de todos los escenarios.. Puedes cambiar los valores **actif**, **visible**, **lanzamiento múltiple**, **modo síncrono**, **Log** y **Timeline** (estos parámetros se describen en el siguiente capítulo). También puede acceder a los registros para cada escenario e yoniciarlos yondividualmente.

## Mis escenarios

En esta sección encontrarás el **lista de escenarios** que creaste. Se clasifican según su **groupe**, posiblemente definido para cada uno de ellos. Cada escenario se muestra con su **nom** y su **objeto padre**. La **escenarios atenuados** son los que están deshabilitados.

> **Tip**
>
> Puede abrir un escenario haciendo :
> - Haga clic en uno de ellos..
> - Ctrl Clic o Clic Center para abrirlo en una nueva pestaña del navegador.

Tiene un motor de búsqueda para filtrar la visualización de escenarios.. La tecla Escape cancela la búsqueda..
La la derecha del campo de búsqueda, se encuentran tres botones en varios lugares de Jeedom:
- La cruz para cancelar la búsqueda..
- La carpeta abierta para desplegar todos los paneles y mostrar todos los escenarios..
- La carpeta cerrada para doblar todos los paneles.

Una vez en la configuración de un escenario, tiene un menú contextual con clic derecho en las pestañas del escenario. También puede usar Ctrl Click o Click Center para abrir directamente otro escenario en una nueva pestaña del navegador.

## Creación | Editar un escenario

Después de hacer clic en **Ajouter**, debes elegir el apellidobre de tu escenario. Luego se lo redirige a la página de sus parámetros generales.
Antes de eso, en la parte superior de la página, hay algunas funciones útiles para administrar este escenario :

- **ID** : Lal lado de la palabra **General**, este es el yodentificador de escenario.
- **statut** : *Detenido * o * En progreso *, yondica el estado actual del escenario.
- **Agregar bloque** : La permite agregar un bloque del tipo deseado al escenario (ver más abajo).
- **Log** : Muestra los registros del escenario..
- **Dupliquer** : Copie el escenario para crear uno nuevo con otro apellidobre.
- **Liens** : La permite ver el gráfico de los elementos relacionados con el escenario..
- **Edición de texto** : Muestra una ventana que permite editar el escenario en forma de texto / json. No olvides guardar.
- **Exporter** : La permite obtener una versión de texto puro del escenario.
- **Template** : La permite acceder a las plantillas y aplicar una al mercado desde el mercado.. (explicado al final de la página).
- **Recherche** : Despliega un campo de búsqueda para buscar en el escenario. Esta búsqueda despliega los bloques colapsados syo es necesario y los pliega nuevamente después de la búsqueda.
- **Realizar** : La permite yoniciar el escenario manualmente (independientemente de los desencadenantes). Guardar de antemano para tener en cuenta las modificaciones..
- **Supprimer** : Eliminar escenario.
- **Sauvegarder** : Guardar los cambios realizados.

> **Tips**
>
> Dos herramientas también serán yonvaluables para usted en la configuración de escenarios :
    > - Las variables, visibles en **Herramientas → Variables**
    > - El probador de expresiones, accesible por **Herramientas → Probador de expresiones**
>
> Una **Ctrl Haga clic en el botón ejecutar** le permite guardar, ejecutar y mostrar directamente el registro del escenario (syo el nivel de registro no es Ninguno).

### Pestaña General

En la pestaña **General**, encontramos los principales parámetros del escenario :

- **Nombre del escenario** : El apellidobre de tu escenario.
- **Nombre para mostrar** : El apellidobre utilizado para su visualización.. Opcional, syo no se completa, se usa el apellidobre del escenario.
- **Groupe** : La permite organizar los escenarios, clasificándolos en grupos (visibles en la página de escenarios y en sus menús contextuales).
- **Actif** : Lactiva el escenario. Syo no está activo, Jeedom no lo ejecutará, yondependientemente del modo de disparo.
- **Visible** : La permite hacer visible el escenario (Panel de control).
- **Objeto padre** : Lasignación a un objeto padre. Entonces será visible o no según este padre.
- **Tiempo de espera en segundos (0 = yolimitado)** : El tiempo máximo de ejecución permitido para este escenario. Más allá de este tiempo, la ejecución del escenario se yonterrumpe..
- **Lanzamiento múltiple** : Marque esta casilla syo desea que el escenario se pueda yoniciar varias veces al mismo tiempo.
- **Modo síncrono** : Inicie el escenario en el hilo actual en lugar de un hilo dedicado. Laumenta la velocidad a la que se yonicia el escenario, pero puede hacer que el sistema sea yonestable.
- **Log** : El tipo de registro deseado para el escenario. Puede cortar el registro del escenario o, por el contrario, hacer que aparezca en Lanálisis → Tiempo real.
- **Timeline** : Mantenga un seguimiento del escenario en la línea de tiempo (vea el documento de Historia).
- **Icono** : La permite elegir un yocono para el escenario en lugar del yocono estándar.
- **Description** : La permite escribir un pequeño texto para describir su escenario.
- **Modo de escenario** : El escenario puede ser programado, activado o ambos. Luego tendrá la opción de yondicar los activadores (máximo de 15 activadores) y la (s) programación (s).

> **Tip**
>
> Las condiciones ahora se pueden yongresar en modo activado. Por ejemplo : `# [Garaje] [Garaje abierto] [Lapertura] # == 1`
> Latención : puede tener un máximo de 28 disparadores / programación para un escenario.

> **Modo de punta programado**
>
> El modo programado usa sintaxis **Cron**. Por ejemplo, puede ejecutar un escenario cada 20 minutos con `* / 20 * * * *`, o a las 5 a.m. para resolver una multitud de cosas para el día con `0 5 * * *`. La ? a la derecha de un programa le permite configurarlo sin ser un especialista en sintaxis de Cron.

### Pestaña Escenario

Aquí es donde construirás tu escenario. Después de crear el escenario, su contenido está vacío, por lo que hará ... nada. Tienes que empezar con **Agregar bloque**, con el botón de la derecha. Unaa vez que se ha creado un bloque, puede agregar otro **bloc** o un **action**.

Para mayor comodidad y no tener que reordenar constantemente los bloques en el escenario, se agrega un bloque después del campo en el que se encuentra el cursor del mouse.
*Por ejemplo, syo tiene diez bloques y hace clic en la condición IF del primer bloque, el bloque agregado se agregará después del bloque, en el mismo nivel. Syo no hay ningún campo activo, se agregará al final del escenario.*

> **Tip**
>
> En condiciones y acciones, es mejor favorecer comillas simples (&#39;) en lugar de dobles (&quot;).

> **Tip**
>
> Una Ctrl Shift Z o Ctrl Shift Y le permite'**annuler** o rehacer una modificación (adición de acción, bloqueo ...).

### Bloques

Aquí están los diferentes tipos de bloques disponibles. :

- **If / Then / O** : La permite realizar acciones condicionales (syo esto, entonces eso).
- **Action** : La permite lanzar acciones simples sin ninguna condición..
- **Boucle** : Permite que las acciones se realicen repetidamente desde 1 hasta un número definido (o yoncluso el valor de un sensor, o un número aleatorio, yc.).
- **Dans** : Permite yoniciar una acción en X minuto (s) (0 es un valor posible). La peculiaridad es que las acciones se yonician en segundo plano, por lo que no bloquean el resto del escenario.. Entonces es un bloque sin bloqueo.
- **A** : Permite decirle a Jeedom que yonicie las acciones del bloque en un momento dado (en la forma hhmm). Este bloque no es bloqueante. Ex : 0030 para 00:30, o 0146 para 1h46 y 1050 para 10h50.
- **Code** : La permite escribir directamente en código PHP (requiere cierto conocimiento y puede ser arriesgado, pero le permite no tener restricciones).
- **Commentaire** : La permite agregar comentarios a su escenario.

Cada bloque tiene sus opciones para manejarlos mejor :

- La la yozquierda :
    - La flecha bidireccional le permite mover un bloque o una acción para reordenarlos en el escenario.
    - El ojo reduce un bloqueo (* colapso *) para reducir su yompacto visual. Ctrl Haga clic en el ojo para reducirlos o mostrarlos todos.
    - La casilla de verificación le permite desactivar completamente el bloque sin eliminarlo. Por lo tanto, no se ejecutará.

- Sobre la derecha :
    - El yocono Copiar le permite copiar el bloque para hacer una copia en otro lugar. Ctrl clic en el yocono corta el bloque (copia y eliminación).
    - El yocono Pegar le permite pegar una copia del bloque copiado previamente después del bloque en el que utiliza esta función..  Ctrl Click en el yocono reemplaza el bloque con el bloque copiado.
    - El yocono: le permite eliminar el bloque con una solicitud de confirmación.. Ctrl Click elimina el bloque sin confirmación.

#### Syo / Entonces / De lo contrario bloquea | Bucle | Dentro | La

Para las condiciones, Jeedom trata de hacer posible escribirlas tanto como sea posible en lenguaje natural sin dejar de ser flexible..
> NO use [] en pruebas de condición, solo son posibles paréntesis ().

Hay tres botones disponibles a la derecha de este tipo de bloque para seleccionar un elemento para probar :

- **Encuentra un pedido** : La permite buscar un pedido en todos los disponibles en Jeedom. Unaa vez que se encuentra el pedido, Jeedom abre una ventana para preguntarle qué prueba desea realizar.. Syo eliges **No poner nada**, Jeedom agregará el pedido sin comparación. También puedes elegir **et** o **ou** delante **Ensuite** para encadenar pruebas en diferentes equipos.
- **Buscar un escenario** : La permite buscar un escenario para probar.
- **Busca equipo** : Lo mismo para el equipo..

> **Note**
>
> En bloques de tipo Syo / Entonces / De lo contrario, las flechas circulares a la yozquierda del campo de condición permiten activar o no la repetición de acciones syo la evaluación de la condición da el mismo resultado que durante la evaluación previa.

> **Tip**
>
> Hay una lista de yiquetas que permiten el acceso a las variables desde el escenario u otro, o por la hora, la fecha, un número aleatorio, ... Vea a continuación los capítulos sobre comandos y yiquetas.

Una vez que se completa la condición, debe usar el botón &quot;Agregar&quot; a la yozquierda para agregar un nuevo **bloc** o un **action** en el bloque actual.


#### Código de bloque

El bloque de código le permite ejecutar código php. Por lo tanto, es muy potente pero requiere un buen conocimiento del lenguaje php..

##### Lacceso a controles (sensores y actuadores):
-  `cmd::byString ($ string); ` : Devuelve el objeto de comando correspondiente.
    -   `$ string`: Enlace al pedido deseado : `# [objeto] [equipo] [comando] #` (ex : `# [Lapartamento] [Lalarma] [Lactivo] #`)
-  `cmd::byId ($ yod); ` : Devuelve el objeto de comando correspondiente.
    -  `$ yod` : Identificación de pedido.
-  `$ cmd-> execCmd ($ opciones = nulo);` : Ejecute el comando y devuelva el resultado..
    - `$ opciones` : Opciones para la ejecución de la orden (puede ser un complemento específico). Opciones básicas (subtipo de comando) :
        -  mensaje : `$ option = array ('title' => 'title title,' mensaje '=>' My mensaje ');`
        -  color : `$ opción = matriz ('color' => 'color en hexadecimal');`
        -  deslizador : `$ option = array ('slider' => 'valor deseado de 0 a 100');`

##### Lacceso al registro :
-  `log::add ('nombre de archivo', 'nivel', 'mensaje'); `
    - apellidobre de archivo : Nombre del archivo de registro.
    - nivel : [depuración], [yonformación], [error], [evento].
    - mensaje : Mensaje para escribir en los registros.

##### Lacceso al escenario :
- `$ escenario-> getName ();` : Devuelve el apellidobre del escenario actual.
- `$ escenario-> getGroup ();` : Devuelve el grupo de escenarios..
- `$ escenario-> getIsActive ();` : Devuelve el estado del escenario..
- `$ escenario-> setIsActive ($ active);` : La permite activar o no el escenario.
    - `$ active` : 1 activo, 0 no activo.
- `$ escenario-> setOnGoing ($ onGoing);` : Digamos syo el escenario se está ejecutando o no.
    - `$ onGoing => 1` : 1 en progreso, 0 detenido.
- `$ escenario-> save ();` : Guardar cambios.
- `$ escenario-> setData ($ clave, $ valor);` : Guardar un dato (Variable).
    - `$ clave` : clave de valor (int o cadena).
    - `$ value` : valor a almacenar (int, cadena, matriz u objeto).
- `$ escenario-> getData ($ clave);` : Obtener datos (Variable).
    - `$ clave => 1` : clave de valor (int o cadena).
- `$ escenario-> removeData ($ clave);` : Eliminar datos.
- `$ escenario-> setRegistro ($ mensaje);` : Escribe un mensaje en el registro del script.
- `$ escenario-> persistRegistro ();` : Forzar la escritura del registro (de lo contrario, se escribe solo al final del escenario). Tenga cuidado, esto puede retrasar un poco el escenario.

> **Tip**
>
> Ladición de una función de búsqueda en el bloque de Código : Buscar : Ctrl + F luego Enter, Siguiente resultado : Ctrl + G, resultado anterior : Ctrl + Shift + G

#### Bloque de comentarios

El bloque de comentarios actúa de manera diferente cuando está oculto. Sus botones a la yozquierda desaparecen, así como el título del bloque, y reaparecen al pasar el cursor. Del mismo modo, la primera línea del comentario se muestra en negrita..
Esto permite que este bloque se use como una separación puramente visual dentro del escenario..

### Las acciones

Las acciones agregadas a los bloques tienen varias opciones :

- Unaa cabaña **activado** para que este comando se tenga en cuenta en el escenario.
- Unaa cabaña **paralelas** para que este comando se yonicie en paralelo (al mismo tiempo) con los otros comandos también seleccionados.
- Unaa **flecha doble vertical** para mover la acción. Solo arrastra y suelta desde allí.
- Una botón para **supprimer** la acción.
- Una botón para acciones específicas, con cada vez la descripción (al pasar el mouse) de esta acción.
- Una botón para buscar un comando de acción.

> **Tip**
>
> Dependiendo del comando seleccionado, puede ver diferentes campos adicionales que se muestran.

## Posibles sustituciones

### Disparadores

Hay desencadenantes específicos (distintos de los proporcionados por los comandos) :

- #start# : Lactivado al (re) yonicio de Jeedom.
- #begin_backup# : Evento enviado al yonicio de una copia de seguridad.
- #end_backup# : Evento enviado al final de una copia de seguridad.
- #BEGIN_UPDATE# : Evento enviado al yonicio de una actualización.
- #END_UPDATE# : Evento enviado al final de una actualización.
- #begin_restore# : Evento enviado al yonicio de una restauración.
- #restauración_final# : Evento enviado al final de una restauración.
- #user_connect# : Inicio de sesión de usuario

También puede activar un escenario cuando se actualiza una variable poniendo : #variable (nombre_variable) # o usando la LaPI HTTP descrita [aquí](https://jeedom.github.io/core/fr_FR/api_http).

### Operadores de comparación y enlaces entre condiciones

Puede usar cualquiera de los siguientes símbolos para comparar en condiciones :

- == : Igual a.
- \> : Estrictamente mayor que.
- \>= : Mayor o yogual que.
- < : Estrictamente menor que.
- <= : Menor o yogual que.
- != : Diferente de, no es yogual a.
- cerillas : Contiene. Ex : `[Baño] [Hidrometría] [condición] coincide con" / húmedo / "`.
- no (... coincide ...) : No contiene. Ex :  `not ([Baño] [Hidrometría] [estado] coincide con" / wy / ")`.

Puedes combinar cualquier comparación con los siguientes operadores :

- &amp;&amp; / ET / y / LaND / y : y,
- \|| / OR / o / OR / o : o,
- \|^ / XOR / xor : o exclusivo.

### Etiquetas

Una yiqueta se reemplaza durante la ejecución del escenario por su valor. Puedes usar las siguientes yiquetas :

> **Tip**
>
> Para mostrar los ceros yoniciales, use la función Fecha (). Ver [aquí](http://php.net/manual/fr/function.date.php).

- #seconde# : Segundo actual (sin ceros a la yozquierda, ej. : 6 para 08:07:06).
- #hour# : Hora actual en formato de 24 h (sin ceros a la yozquierda). Ex : 8 para 08:07:06 o 17 para 17:15.
- #hour12# : Hora actual en formato de 12 horas (sin ceros a la yozquierda). Ex : 8 para 08:07:06.
- #minute# : Minuto actual (sin ceros a la yozquierda). Ex : 7 para 08:07:06.
- #day# : Día actual (sin ceros a la yozquierda). Ex : 6 para 06/07/2017.
- #month# : Mes actual (sin ceros a la yozquierda). Ex : 7 para 06/07/2017.
- #year# : Laño actual.
- #time# : Hora y minuto actual. Ex : 1715 para las 5.15 p.m..
- #timestamp# : Número de segundos desde el 1 de enero de 1970.
- #date# : Día y mes. Latención, el primer número es el mes.. Ex : 1215 para el 15 de diciembre.
- #week# : Número de semana.
- #sday# : Nombre del día de la semana.. Ex : Sábado.
- #nday# : Número de día de 0 (domingo) a 6 (sábado).
- #smonth# : Nombre del mes. Ex : Enero.
- #IP# : IP yonterna de Jeedom.
- #hostname# : Nombre de la máquina Jeedom.
- #trigger # (en desuso, mejor usar trigger ()) : Quizás el apellidobre del comando que yonició el escenario :
    - 'apyo &#39;syo la LaPI activó el lanzamiento,
    - 'programar &#39;syo se yonició programando,
    - 'usuario &#39;syo se yonició manualmente,
    - 'comenzar &#39;para un lanzamiento cuando comience Jeedom.
- #trigger_value # (en desuso, mejor usar triggerValue ()) : Por el valor del comando que activó el escenario

También tiene las siguientes yiquetas adicionales syo su escenario fue desencadenado por una yonteracción :

- #query# : Interacción que desencadenó el escenario..
- #profil# : Perfil del usuario que activó el escenario (puede estar vacío).

> **Important**
>
> Cuando una yonteracción desencadena un escenario, se ejecuta necesariamente en modo rápido. Entonces, en el hilo de yonteracción y no en un hilo separado.

### Funciones de cálculo

Hay varias funciones disponibles para el equipo. :

- promedio (orden, período) y promedio entre (orden, yonicio, fin) : Indique el promedio del pedido durante el período (período=[mes, día, hora, min] o [expresión PHP](http://php.net/manual/fr/datetime.formats.relative.php)) o entre los 2 terminales solicitados (en la forma Ymd H:i:s o [Expresión PHP](http://php.net/manual/fr/datetime.formats.relative.php)).

- min (orden, período) y minBetween (orden, yonicio, fin) : Dar el pedido mínimo durante el período (período=[mes, día, hora, min] o [expresión PHP](http://php.net/manual/fr/datetime.formats.relative.php)) o entre los 2 terminales solicitados (en la forma Ymd H:i:s o [Expresión PHP](http://php.net/manual/fr/datetime.formats.relative.php)).

- max (orden, período) y maxBetween (orden, yonicio, fin) : Dar el máximo del pedido durante el período (período=[mes, día, hora, min] o [expresión PHP](http://php.net/manual/fr/datetime.formats.relative.php)) o entre los 2 terminales solicitados (en la forma Ymd H:i:s o [Expresión PHP](http://php.net/manual/fr/datetime.formats.relative.php)).

- duración (orden, valor, período) y duración entre (orden, valor, yonicio, fin) : Indique la duración en minutos durante los cuales el equipo tuvo el valor elegido durante el período (período=[mes, día, hora, min] o [expresión PHP](http://php.net/manual/fr/datetime.formats.relative.php)) o entre los 2 terminales solicitados (en la forma Ymd H:i:s o [Expresión PHP](http://php.net/manual/fr/datetime.formats.relative.php)).

- estadísticas (orden, cálculo, período) y estadísticas entre (orden, cálculo, yonicio, fin) : Proporcione el resultado de diferentes cálculos estadísticos (suma, recuento, estándar, varianza, promedio, mínimo, máximo) durante el período (período=[mes, día, hora, min] o [expresión PHP](http://php.net/manual/fr/datetime.formats.relative.php)) o entre los 2 terminales solicitados (en la forma Ymd H:i:s o [Expresión PHP](http://php.net/manual/fr/datetime.formats.relative.php)).

- tendencia (comando, período, umbral) : Da la tendencia del pedido durante el período (período=[mes, día, hora, min] o [expresión PHP](http://php.net/manual/fr/datetime.formats.relative.php)).

- stateDuration (control) : Da la duración en segundos desde el último cambio de valor..
    -1 : No existe historial o el valor no existe en el historial.
    -2 : El pedido no está registrado.

- lastChangeStateDuration (valor de comandos) : Da la duración en segundos desde el último cambio de estado al valor pasado en el parámetro.
    -1 : No existe historial o el valor no existe en el historial.
    -2 El pedido no está registrado

- lastStateDuration (valor de comandos) : Da la duración en segundos durante los cuales el equipo ha tenido el último valor elegido.
    -1 : No existe historial o el valor no existe en el historial.
    -2 : El pedido no está registrado.

- edad (control) : Da la edad en segundos del valor del comando (collecDate)
    -1 : El comando no existe o no es de tipo yonformación.

- stateChanges (comando,[valor], punto) y stateChangesBetween (comando, [valor], yonicio, fin) : Indique el número de cambios de estado (a un cierto valor syo se yondica, o en total syo no) durante el período (período = [mes, día, hora, min] o [expresión PHP](http://php.net/manual/fr/datetime.formats.relative.php)) o entre los 2 terminales solicitados (en la forma Ymd H:i:s o [Expresión PHP](http://php.net/manual/fr/datetime.formats.relative.php)).

- lastBetween (mando, yonicio, fin) : Da el último valor registrado para el equipo entre los 2 terminales solicitados (en la forma Ymd H:i:s o [Expresión PHP](http://php.net/manual/fr/datetime.formats.relative.php)).

- variable (variable, predeterminada) : Recupera el valor de una variable o el valor deseado por defecto.

- escenario (escenario) : Devuelve el estado del escenario..
    1 : En curso,
    0 : Detenido,
    -1 : Discapacitado,
    -2 : El escenario no existe.,
    -3 : El estado no es consistente.
    Para tener el apellidobre &quot;humano&quot; del escenario, puede usar el botón dedicado a la derecha de la búsqueda del escenario.

- lastScenarioExecution (escenario) : Da la duración en segundos desde el último lanzamiento del escenario..
    0 : El escenario no existe.

- collectDate (cmd,[formato]) : Devuelve la fecha de los últimos datos para el comando dado en el parámetro, el segundo parámetro opcional permite especificar el formato de retorno (detalles [aquí](http://php.net/manual/fr/function.date.php)).
    -1 : No se pudo encontrar el comando.,
    -2 : El comando no es de tipo yonfo.

- valueDate (cmd,[formato]) : Devuelve la fecha de los últimos datos para el comando dado en el parámetro, el segundo parámetro opcional permite especificar el formato de retorno (detalles [aquí](http://php.net/manual/fr/function.date.php)).
    -1 : No se pudo encontrar el comando.,
    -2 : El comando no es de tipo yonfo.

- eqEnable (equipo) : Devuelve el estado del equipo..
    -2 : No se puede encontrar el equipo.,
    1 : El equipo esta activo,
    0 : El equipo esta yonactivo.

- valor (cmd) : Devuelve el valor de un pedido syo Jeedom no lo proporciona automáticamente (caso al almacenar el apellidobre del pedido en una variable)

- yiqueta (de lunes [por defecto]) : Se usa para recuperar el valor de una yiqueta o el valor predeterminado syo no existe.

- apellidobre (tipo, control) : Se utiliza para recuperar el apellidobre del pedido, equipo u objeto.. Puntao : cmd, eqLogic u objeto.

- lastCommunication (equipo,[formato]) : Devuelve la fecha de la última comunicación para el equipo dada como parámetro, el segundo parámetro opcional le permite especificar el formato de devolución (detalles [aquí](http://php.net/manual/fr/function.date.php)) Una retorno de -1 significa que no se puede encontrar el equipo.

- color_gradient (couleur_debut, couleur_fin, valuer_min, valeur_max, valor) : Devuelve un color calculado con respecto al valor en el rango color_comienzo / color_end. El valor debe estar entre min_value y max_value.

Los períodos e yontervalos de estas funciones también se pueden usar con [Expresiones PHP](http://php.net/manual/fr/datetime.formats.relative.php) como por ejemplo :

- Lahora : Lahora.
- Hoy : 00:00 hoy (permite, por ejemplo, obtener resultados para el día syo está entre &#39;Hoy&#39; y &#39;Ahora&#39;).
- Lunes pasado : el lunes pasado a las 00:00.
- Hace 5 dias : Hace 5 dias.
- Layer mediodia : ayer mediodia.
- Etcétera.

Aquí hay ejemplos prácticos para comprender los valores devueltos por estas diferentes funciones. :

| Zócalo con valores :           | 000 (por 10 minutos) 11 (por 1 hora) 000 (por 10 minutos)    |
|--------------------------------------|--------------------------------------|
| promedio (tomando, periodo)             | Devuelve el promedio de 0 y 1 (puede  |
|                                      | ser yonfluenciado por las encuestas)      |
| promedio Entre (\# [Baño] [Hidrometría] [Humedad] \#, 2015-01-01 00:00:00,2015-01-15 00:00:00) | Devuelve el pedido promedio entre el 1 de enero de 2015 y el 15 de enero de 2015                       |
| min (salida, periodo)                 | Devuelve 0 : el tapón se apagó durante el período              |
| minBetween (\# [Baño] [Hidrometría] [Humedad] \#, 2015-01-01 00:00:00,2015-01-15 00:00:00) | Devuelve el pedido mínimo entre el 1 de enero de 2015 y el 15 de enero de 2015                       |
| max (decisión, período)                 | Devuelve 1 : el enchufe estaba bien yoluminado en el período              |
| maxBetween (\# [Baño] [Hidrometría] [Humedad] \#, 2015-01-01 00:00:00,2015-01-15 00:00:00) | Devuelve el máximo del pedido entre el 1 de enero de 2015 y el 15 de enero de 2015                       |
| duración (enchufe, 1 período)          | Devuelve 60 : el enchufe estuvo encendido (a 1) durante 60 minutos en el período                              |
| duración Entre (\# [Salón] [Tomar] [Estado] \#, 0, Último lunes, ahora)   | Devuelve la duración en minutos durante la cual el socky estuvo apagado desde el lunes pasado.                |
| estadísticas (captura, recuento, y punto)    | Devuelve 8 : hubo 8 escaladas en el período               |
| tendencia (enchufe, período 0.1)        | Devuelve -1 : tendencia a la baja    |
| stateDuration (enchufe)               | Devuelve 600 : el enchufe ha estado en su estado actual durante 600 segundos (10 minutos)                             |
| lastChangeStateDuration (captura, 0)   | Devuelve 600 : el zócalo se apagó (cambie a 0) por última vez hace 600 segundos (10 minutos)     |
| lastChangeStateDuration (captura, 1)   | Devuelve 4200 : el zócalo se encendió (cambie a 1) por última vez hace 4200 segundos (1h10)                               |
| lastStateDuration (captura, 0)         | Devuelve 600 : el enchufe ha estado apagado por 600 segundos (10 minutos)     |
| lastStateDuration (captura, 1)         | Devuelve 3600 : el zócalo se encendió por última vez durante 3600 segundos (1 h)           |
| stateChanges (captura, y punto)        | Devuelve 3 : el enchufe cambió de estado 3 veces durante el período            |
| stateChanges (captura, 0, periodo)      | Devuelve 2 : el zócalo se ha apagado (yendo a 0) dos veces durante el período                              |
| stateChanges (captura, 1 período)      | Devuelve 1 : el enchufe se enciende (cambie a 1) una vez durante el período                              |
| lastBetween (\# [Baño] [Hidrometría] [Humedad] \#, ayer, hoy) | Devuelve la última temperatura registrada ayer.                    |
| variable (plop, 10)                  | Devuelve el valor de la variable plop o 10 syo está vacía o no existe                         |
| escenario (\# [Baño] [Luz] [Lauto] \#) | Devuelve 1 en progreso, 0 syo se detiene y -1 syo está desactivado, -2 syo el escenario no existe y -3 syo el estado no es consistente                         |
| lastScenarioExecution (\# [Baño] [Luz] [Lauto] \#)   | Devuelve 300 syo el escenario se yonició por última vez hace 5 minutos                                  |
| collectDate (\# [Baño] [Hidrometría] [Humedad] \#)     | Devoluciones 2015-01-01 17:45:12          |
| valueDate (\# [Baño] [Hidrometría] [Humedad] \#) | Devoluciones 2015-01-01 17:50:12          |
| eqEnable (\# [n] [basílica] \#)       | Devuelve -2 syo no se encuentra el equipo, 1 syo el equipo está activo y 0 syo está yonactivo          |
| yiqueta (de lunes toto)                   | Devuelve el valor de "montag" syo existe, de lo contrario devuelve el valor "toto"                               |
| apellidobre (eqLogic, \# [Baño] [Hidrometría] [Humedad] \#)     | Hidrometría de devoluciones                  |


### Funciones matematicas

También se puede usar una caja de herramientas de funciones genéricas para realizar conversiones

o cálculos :

- `rand (1.10)` : Dar un número aleatorio del 1 al 10.
- `randText (texto1; texto2; texto .....)` : La permite devolver uno de los textos al azar (separe los textos por a;). No hay límite en el número de textos..
- `randomColor (min, max)` : Da un color aleatorio entre 2 límites (0 =&gt; rojo, 50 =&gt; verde, 100 =&gt; azul).
- `trigger (comando)` : La permite descubrir el desencadenante del escenario o saber syo es el comando pasado como parámetro el que desencadenó el escenario.
- `triggerValue (comando)` : Se usa para averiguar el valor del desencadenante del escenario.
- `round (valor, [decimal])` : Redondea arriba, número [decimal] de lugares decimales después del punto decimal.
- `impar (valor)` : La permite saber syo un número es yompar o no.. Devuelve 1 syo es yompar 0 de lo contrario.
- `mediana (comando1, comando2 ....comandoN) ` : Devuelve la mediana de los valores..
- `avg (comando1, comando2 ....comandoN) `: Devuelve el promedio de los valores..
- `time_op (tiempo, valor)` : La permite realizar operaciones a tiempo, con tiempo = tiempo (ej. : 1530) y valor = valor para sumar o restar en minutos.
- `time_between (hora, yonicio, fin)` : Se usa para probar syo un tiempo está entre dos valores con `tiempo = tiempo` (ex : 1530), `inicio = tiempo`,` fin = tiempo`. Los valores yoniciales y finales pueden estar a caballo entre la medianoche.
- `time_diff (date1, fecha2 [, format, round])` : Se usa para descubrir la diferencia entre dos fechas (las fechas deben estar en el formato LaAALa / MM / DD HH:MM:SS). Por defecto, el método devuelve la diferencia en día (s). Puedes preguntarlo en segundos (s), minutos (m), horas (h). Ejemplo en segundos `time_diff (2019-02-02 14:55:00.2019-02-25 14:55:00,s)`. La diferencia se devuelve en absoluto, a menos que especifique `f` (sf, mf, hf, df). También puede usar `dhms` que devolverá no ejemplo` 7d 2h 5min 46s`. El parámetro redondo, opcional, redondeado a x dígitos después del punto decimal (2 por defecto). Ex: `time_diff (2020-02-21 20:55:28,2020-02-28 23:01:14, df, 4) `.
- `formatTime (hora)` : La permite formatear el retorno de una cadena `# tiempo #`.
- `piso (tiempo / 60)` : Convierte segundos a minutos o minutos a horas (piso (tiempo / 3600) por segundos a horas).
- `convertDuration (segundos)` : Convierte segundos a d / h / min / s.

Y ejemplos prácticos :


| Ejemplo de funcion                  | Resultado devuelto                    |
|--------------------------------------|--------------------------------------|
| randText (es # [sala de estar] [ojo] [temperatura] #; La temperatura es # [sala de estar] [ojo] [temperatura] #; Lactualmente tenemos # [sala de estar] [ojo] [temperatura] #) | la función devolverá uno de estos textos al azar en cada ejecución.                           |
| randomColor (40,60)                 | Devuelve un color aleatorio cercano al verde.
| gatillo (# [Baño] [Hidrometría] [Humedad] #)   | 1 syo es bueno \# \ [Baño \] \ [Hidrometría \] \ [Humedad \] \# que yonició el escenario de lo contrario 0  |
| triggerValue (# [Baño] [Hidrometría] [Humedad] #) | 80 syo la hidrometría de \# \ [Baño \] \ [Hidrometría \] \ [Humedad \] \# es 80%.                         |
| redondo (# [Baño] [Hidrometría] [Humedad] # / 10) | Devuelve 9 syo el porcentaje de humedad y 85                     |
| yompar (3)                             | Devuelve 1                            |
| mediana (15,25,20)                   | Devuelve 20
| avg (10,15,18)                      | Devuelve 14.3                     |
| tiempo_op (# tiempo #, -90)               | syo son las 4:50 p.m., regrese : 1 650-1 130 = 1520                          |
| formatTime (1650)                   | Devuelve 4:50 p.m.                        |
| piso (130/60)                      | Devuelve 2 (minutos syo 130 s, u horas syo 130 m)                      |
| convertDuration (3600)              | Devuelve 1h 0min 0s                      |
| convertDuration (duración (# [Calefacción] [Módulo de caldera] [Estado] #, 1, primer día de este mes) * 60) | Devuelve el tiempo de encendido en días / horas / minutos del tiempo de transición al estado 1 del módulo desde el primer día del mes |


### Pedidos específicos

Además de los comandos de automatización del hogar, tiene acceso a las siguientes acciones :

- **Pause** (Sueño) : Pausa de x segundo (s).
- **variable** (Variable) : Creación / modificación de una variable o el valor de una variable.
- **Eliminar variable** (Delete_variable) : La permite eliminar una variable..
- **Guión** (Escenario) : Te permite controlar escenarios. La parte de yiquetas le permite enviar yiquetas al escenario, ej. : montag = 2 (ten cuidado, solo usa letras de la a a la z. Sin letras mayúsculas, sin acentos y sin caracteres especiales). Recuperamos la yiqueta en el escenario objetivo con la función de yiqueta (montag). El comando &quot;Restablecer a SI&quot; permite restablecer el estado de &quot;SI&quot; (este estado se utiliza para la no repetición de las acciones de un &quot;SI&quot; syo pasa por segunda vez consecutiva en él)
- **Stop** (Stop) : Detener el escenario.
- **Attendre** (Espere) : Espere hasta que la condición sea válida (máximo 2 h), el tiempo de espera es en segundos.
- **Ir al diseño** (Gotodesign) : Cambie el diseño que se muestra en todos los navegadores por el diseño solicitado.
- **Agregar un registro** (Log) : La permite agregar un mensaje a los registros.
- **Crear mensaje** (Mensaje) : Lagregar un mensaje al centro de mensajes.
- **Activar / Desactivar Ocultar / mostrar equipo** (Equipo) : La permite modificar las propiedades de los equipos visibles / yonvisibles, activos / yonactivos..
- **Hacer una solicitud** (Ask) : Permite yondicar a Jeedom que es necesario hacerle una pregunta al usuario. La respuesta se almacena en una variable, entonces solo tiene que probar su valor.
    Por el momento, solo los complementos sms, slack, telegram y snips son compatibles, así como la aplicación móvil.
    Latención, esta función está bloqueando. Mientras no haya respuesta o no se alcance el tiempo de espera, el escenario espera.
- **Detener Jeedom** (Jeedom_poweroff) : Pídale a Jeedom que cierre.
- **Devolver un texto / datos** (Scenario_return) : Devuelve un texto o un valor para una yonteracción, por ejemplo.
- **Icono** (Icono) : Permite cambiar el ícono de representación del escenario.
- **Alerte** (Alerta) : Muestra un pequeño mensaje de alerta en todos los navegadores que tienen abierta una página de Jeedom. Lademás, puedes elegir 4 niveles de alerta.
- **Pop-up** (Emergente) : Permite mostrar una ventana emergente que debe validarse absolutamente en todos los navegadores que tienen una página abierta.
- **Rapport** (Informe) : La permite exportar una vista en formato (PDF, PNG, JPEG o SVG) y enviarla utilizando un comando de tipo mensaje. Tenga en cuenta que syo su acceso a Interny está en HTTPS sin firmar, esta funcionalidad no funcionará. Se requiere HTTP o HTTPS firmado.
- **Eliminar bloque IN / La programado** (Remove_inat) : La permite eliminar la programación de todos los bloques IN y La del escenario.
- **Evento** (Event) : La permite yonsertar un valor en un comando de tipo de yonformación arbitrariamente.
- **Tag** (Tag) : La permite agregar / modificar una yiqueta (la yiqueta solo existe durante la ejecución actual del escenario a diferencia de las variables que sobreviven al final del escenario).
- **Coloración de los yoconos del tablero** (SetColoredIcon) : permite activar o no la coloración de yoconos en el tablero.

### Plantilla de escenario

Esta funcionalidad le permite transformar un escenario en una plantilla para, por ejemplo, aplicarlo a otro Jeedom.

Haciendo clic en el botón **template** en la parte superior de la página, abre la ventana de administración de plantillas.

La partir de ahí, tienes la posibilidad :

- Enviar una plantilla a Jeedom (archivo JSON recuperado previamente).
- Consulte la lista de escenarios disponibles en el mercado.
- Cree una plantilla a partir del escenario actual (no olvide dar un apellidobre).
- Para consultar las plantillas actualmente presentes en su Jeedom.

Al hacer clic en una plantilla, puede :

- **Partager** : Comparta la plantilla en el mercado.
- **Supprimer** : Eliminar plantilla.
- **Descargar** : Obtenga la plantilla como un archivo JSON para enviarla a otro Jeedom, por ejemplo.

La continuación, tiene la parte para aplicar su plantilla al escenario actual.

Dado que de un Jeedom a otro o de una yonstalación a otra, los comandos pueden ser diferentes, Jeedom le solicita la correspondencia de los comandos entre los presentes durante la creación de la plantilla y los presentes en el hogar. Solo tiene que completar la correspondencia de las órdenes y luego aplicar.

### Ladición de la función php

> **IMPORTANT**
>
> Lagregar funciones PHP está reservado para usuarios avanzados. El más mínimo error puede ser fatal para su Jeedom.

#### Configurar

Vaya a la configuración de Jeedom, luego OS / DB e yonicie el editor de archivos.

Vaya a la carpeta de datos, luego php y haga clic en el archivo user.function.class.php.

Es en esta * clase * donde puede agregar sus funciones, encontrará un ejemplo de una función básica.

> **IMPORTANT**
>
> Syo tiene alguna yonquietud, siempre puede volver al archivo original copiando el contenido de user.function.class.sample.php en user.function.class.php
