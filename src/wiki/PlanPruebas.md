<p align="center">
  <img src="../assets/Logos/humanIT.005.png" width="300" title="hover text">
</p>
<hr/>

<h1 align="center"> Plan de Pruebas  
<h2 align="center"> Versión 0.2

| Date       | Version | Description  |  
|------------|:-------:| :----------- |
| 12/03/2023 | 0.1     | Creación del Doc SRS|                          
| 13/03/2023 | 0.2     | Doc en Markdown|      

# Índice
1. Introducción<br>
    1.1. Propósito<br>
    1.2. Audiencia<br>	
2. Estrategia de pruebas<br>	
    2.1. Descripción de pruebas<br>	
    2.2. Objetivo de las pruebas<br>	
    2.3. Suposiciones de las pruebas<br>	
    2.4. Objetivos de las pruebas<br>	
    2.5. Alcance<br>	
    2.6. Niveles de pruebas<br>	
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Prueba de Caja Blanca (Prueba Funcional)<br>	
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Prueba de Integración (Prueba Funcional)<br>	
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Prueba de Aceptación (Prueba Funcional)<br>	
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Prueba de Recorrido Estático (Validación)<br>	
    2.7. Criterios de aceptación de pruebas<br>	
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Pruebas Informales<br>	
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Pruebas Unitarias<br>	
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Prueba de Integración<br>	
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Prueba de Validación/Aceptación<br>	
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Pruebas Estáticas de Recorrido<br>	
    2.8. Entregables de pruebas<br>	
    2.9. Lista de hitos<br>	
    2.10. Estimación de esfuerzo de las pruebas<br>
3. Proceso de gestión de pruebas<br>
    3.1. Proceso de ejecución de pruebas<br>	
    3.2. Riesgos de prueba y factores de mitigación<br>
    3.3. Plan de comunicaciones y lista de equipos<br>	
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Expectativas del Rol<br>	
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Project Manager<br>	
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Líder de Pruebas<br>	
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Líder de Back-End<br>	
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Cronograma de Actividades<br>	
4. Ambiente de pruebas<br>	
5. Pruebas<br>	
6. Conclusiones<br>


## 1. Introducción

### 1.1 Propósito
<p align="justify"> El documento presente tiene el objetivo de describir el programa de pruebas que se realizará durante el desarrollo del proyecto con NDS; una plataforma para la venta de automóviles en línea. En particular, este documento contendrá:<br>

* La estrategia y objetivos de las pruebas a realizarse en cada uno de los componentes de la aplicación.
* Una justificación acerca de las pruebas seleccionadas.
* Los criterios de validación para los componentes de la aplicación y los criterios de aceptación de cada una de las pruebas.
* El plan de ejecución de las pruebas a realizarse, al igual que el plan de remediación  en caso de que una de estas pruebas termine con un resultado negativo.
* Las responsabilidades de los integrantes del equipo en relación a las pruebas.
* Una descripción del ambiente, al igual que las herramientas  herramientas que serán utilizadas para las pruebas.

## 1.2 Audiencia 
<p align="justify"> En esta sección se encuentra la descripción detallada de la audiencia a la que se dirige el presente escrito:<br>  

* El siguiente documento está diseñado para ser consultado principalmente por los miembros del equipo de desarrollo del proyecto, profesores responsables del mismo, el cliente (NDS) y sus representantes.
    * Las pruebas funcionales o dinámicas están orientadas a la compresión de los desarrolladores y del Project Manager.
    * Las pruebas estáticas están diseñadas para ser entendidas no solo por el equipo de desarrollo, sino también por cualquier persona fuera del área de tecnología. 
* El director del proyecto es responsable de utilizar el documento para garantizar que se sigue el calendario de pruebas acordado y que se supervisa el progreso de acuerdo con las instrucciones del documento. Asimismo, esta figura es responsable de los resultados y el rendimiento de cada prueba.
* El cliente (NDS), las partes interesadas o sus representantes tienen la opción de revisar el documento para verificar que el desarrollo se ajusta a sus requisitos e intereses.
* El equipo de desarrollo se encarga de garantizar que el plan de pruebas y los resultados especificados en el documento son coherentes con lo acordado durante la fase de diseño.
* El equipo de desarrollo es responsable de resolver cualquier prueba fallida señalada en el documento.
* Otros miembros del equipo y las partes interesadas también pueden utilizar el documento como punto de referencia en todo momento para diversos asuntos relacionados con el proyecto.

## 2. Estrategia de Pruebas 
### 2.1 Descripción de Pruebas
En el presente apartado se describe a profundidad la estrategia de pruebas que se seguirá durante el proceso de desarrollo de la plataforma web para el cliente NDS.

<p align="justify"><b>Etapa 1 – Comprensión de los Requerimientos, Especificaciones del Proyecto y Pruebas Estáticas:</b><br> Antes de crear una estrategia de pruebas, primero se comprenden y establecen de manera detallada los requerimientos del proyecto. Para ello se tiene una serie de interacciones semanales con el cliente NDS en el cual se documentan de forma clara las características de la solución que cumplen con sus necesidades y objetivos. Al finalizar esta etapa se espera que haya pocos o nulos cambios, ya que el resto del proyecto se desarrollará en base a lo establecido en esta etapa, por lo cuál queda fuera de las etapas de iteración. 

<p align="justify"><b>Etapa 2 - Pruebas Informales:</b><br> En un principio, se comenzará realizando pruebas informales durante el desarrollo del software. Esto incluiría pruebas realizadas individualmente por cada uno de los desarrolladores sin supervisión, teniendo un enfoque en comprobar la funcionalidad de componentes creados. En esta etapa comienza el proceso iterativo de las pruebas y va dentro de las pruebas dinámicas. 

<p align="justify"><b>Etapa 3 – Realización de Pruebas Unitarias:</b><br> Esta etapa también va dentro de las pruebas dinámicas y se pretende comenzar realizando las pruebas unitarias para cada componente de software de la plataforma. Esto concentrándose en pruebas de caja negra (black box tests) tomando especial atención en la entrada y salida esperadas en su correcto funcionamiento. Simultáneamente a esto, se acordará de manera iterativa con NDS las pruebas de historias de usuario van de acuerdo a sus criterios de aceptación. Esto ayudará a garantizar que la página web satisfaga correctamente las necesidades de NDS y de sus clientes.

<p align="justify"><b>Etapa 4 - Pruebas de Caja Blanca de cobertura (White Box Testing):</b><br> En esta etapa, que también va dentro de las dinámicas, se realizan las pruebas de caja blanca a los componentes definidos en este documento, especialmente dando prioridad a aquellos componentes que generaron errores en las Pruebas de Caja Negra. De esta manera, se podrá analizar el código de dichos componentes, así permitiendo arreglar errores persistentes en pruebas anteriores o eliminar redundancias. 
Para hacer más eficaz nuestro proceso de pruebas de caja blanca, usaremos la técnica de cobertura en donde se probaran los caminos más utilizados para hacer uso de cada función de cada tipo de usuario. 

<p align="justify"><b>Etapa 5 - Pruebas de Integración:</b><br> En esta etapa, que es la última dentro de las etapas dinámicas, después de que todas las pruebas unitarias hayan pasado con éxito se pasan a las pruebas de integración donde de manera ascendente se van uniendo los diferentes componentes para validar su correcto funcionamiento en conjunto. Las pruebas de integración se llevarán a cabo mediante pruebas de caja negra de casos de uso aleatorias, las cuales serán elegidas y supervisadas por el Project Manager responsable del equipo de desarrollo.

<p align="justify"><b>Etapa 6 – Pruebas de Validación/Aceptación:</b><br> En esta etapa, se requiere que haya pocos o ningún cambio, ya qué, después de que las pruebas de integración hayan sido exitosas se realizan las pruebas de validación en las que se revisará con el cliente NDS que los criterios de validación definidos en etapas anteriores se cumplen hasta el momento del proceso de pruebas.

<p align="justify"><b>Etapa 7 – Pruebas de Estática de Recorridos:</b><br> Una vez que se haya tenido la aprobación de NDS se realizará la prueba del funcionamiento del sistema como un todo, verificando el comportamiento y correcto funcionamiento de toda la plataforma en el nivel más alto posible.

<p align="justify"><b>Etapa 8 - Manual de Usuario:</b><br> En esta etapa final, una vez que se haya completado las etapas anteriores y son pocos o nulos los cambios se crea el manual de usuario en el que se le proveerá información e instrucciones al usuario de cómo usar el software desarrollado. En el manual de usuario se incluirán los caminos previamente establecidos en las pruebas de caja blanca de cobertura. El manual toma en cuenta la versión más actualizada y funcional de la aplicación.

<p align="justify">Es relevante mencionar, que en esta estrategia se mantiene un flujo iterativo, donde de ser necesario se actualizará el documento de pruebas o se podrá regresar a etapas de pruebas anteriores para así solucionar cualquier fallo o error en cualquier nivel de la plataforma.

### 2.2 Objetivo de las Pruebas
<p align="justify"> El objetivo de las pruebas que se realizarán durante el transcurso del proyecto es la validación de las funcionalidades fundamentales de la aplicación, al igual que comprobar la correcta implementación de los requerimientos establecidos en el documento SRS. En consideración de este objetivo, las pruebas a realizarse comprenderán:<br>

* Pruebas que aseguren la correcta autorización de usuarios, al igual que la asignación de los premios asociados.
* Pruebas que comprueben el correcto funcionamiento en la búsqueda y filtrado del catálogo de autos.
* Pruebas que comprueben el correcto funcionamiento del guardado de automóviles en la base de datos.
* Pruebas que garanticen el funcionamiento de la recopilación, análisis, y generación de estadística relacionada con usuarios agentes de la aplicación.
* Pruebas relacionadas al servicio de chat implementado en la aplicación.
Pruebas con el objetivo de comprobar el correcto funcionamiento del proceso de compra de un automóvil.
* Pruebas asociadas a la creación de usuarios con diferentes permisos. 
* Pruebas asociadas al funcionamiento de un software estable y listo para producción.

### 2.3 Suposiciones de las Pruebas
<b>Suposiciones Clave</b><br>
1. Se dará prioridad a las pruebas funcionales debido a limitantes de tiempo y presupuesto. 
Todas las pruebas se harán en el mismo ambiente.
2. Todas las pruebas se harán inicialmente con pruebas Informales y posteriormente en Caja Negra.

<b>Suposiciones Generales</b><br>
1. Las pruebas funcionales serán las más relevantes del plan de pruebas.
2. Realizar las mismas pruebas conlleva a los mismos resultados.
3. Las pruebas con variedad en el rol de acceso no son equivalentes, y debe definirse una prueba por cada rol.
4. Si el ambiente de pruebas deja de estar disponible; el equipo de pruebas creará uno lo más similar lo antes posible.
5. Todas las funciones han sido probadas meticulosamente.
6. Las pruebas de caja blanca y pruebas paso a paso solo se ejecutarán si los resultados son distintos a lo esperado.
7. El equipo de pruebas documentará sus resultados de acuerdo a lo evaluado.
8. El equipo de pruebas asume que todas las entradas o inputs requeridos durante el diseño y la ejecución de las pruebas estarán apoyados por el desarrollador/analista respectivamente. 
9. Todos los documentos personales del usuario serán guardados con el mismo formato y nomenclatura.
10. El PM verificará los resultados de todas las pruebas efectuadas.
11. El PM aprueba todos los casos de prueba propuestos previo a la ejecución de los mismos
12. El equipo de pruebas manejará todo el esfuerzo de ejecución de prueba de forma coordinada con el PM.
13. El recorrido y manual de usuario se realizará en los últimos sprints.

### 2.4 Objetivos de las Pruebas
<i>Flujo del Cliente:</i><br>
* Probar la funcionalidad de Login.
* Probar la funcionalidad de búsqueda de catálogo.
* Probar la funcionalidad de filtrado de catálogo.
* Probar la funcionalidad del agendado  de la prueba de manejo.
* Probar la funcionalidad de la subida de documentos para la solicitud de prueba de manejo.
* Probar la funcionalidad de la subida de documentos para la compra de un auto.
* Probar la funcionalidad de la transacción del pago para la prueba de manejo.
* Probar la funcionalidad de la transacción de la compra de auto.
* Probar la funcionalidad del seguimiento de acciones del usuario (prueba de manejo o compras).
* Probar la funcionalidad del sistema de Chat.
* Probar la funcionalidad del sistema de favoritos (wishlist).
* Probar la funcionalidad de la edición de datos en el perfil.

<i>Flujo del Super Administrador:</i><br>
* Probar la funcionalidad de Login.
* Probar la funcionalidad de búsqueda de usuarios.
* Probar las funcionalidad de filtrado de usuarios.
* Probar la funcionalidad de la modificación de datos de un grupo automotriz.
* Probar la funcionalidad de la búsqueda de solicitudes.
* Probar la funcionalidad del filtrado de solicitudes.
* Probar funcionalidad de la aprobación/negación de una solicitud.
* Probar la funcionalidad del registro de un grupo automotriz.
* Probar la funcionalidad del dashboard estadístico. 

<i>Flujo del Grupo Automotriz:</i><br>

<i>Etapa 1:</i><br>
* Probar funcionalidad del Login.
* Probar funcionalidad para realizar una aplicación.
* Probar funcionalidad del panel de seguimiento a una aplicación.
* Probar funcionalidad de la modificación de los datos del perfil.
* Probar funcionalidad de la eliminación de una cuenta.

<i>Etapa 2:</i><br>
* Probar funcionalidad de Login.
* Probar funcionalidad del registro de una agencia.
* Probar funcionalidad de la búsqueda de usuarios.
* Probar funcionalidad del filtrado de usuarios.
* Probar funcionalidad para la modificación de datos de una agencia.
* Probar funcionalidad del dashboard estadístico.

<i>Flujo de la Agencia:</i><br>
* Probar funcionalidad de Login.
* Probar funcionalidad de la búsqueda de usuarios.
* Probar funcionalidad del filtrado de usuarios.
* Probar funcionalidad del registro de un gerente.
* Probar funcionalidad para la modificación de datos de un gerente.
* Probar funcionalidad para la actualización/modificación del catálogo de autos.
* Probar funcionalidad del dashboard estadístico.

<i>Flujo del Gerente:</i><br>
* Probar funcionalidad de Login.
* Probar funcionalidad de la búsqueda de usuarios.
* Probar funcionalidad del filtrado de usuarios.
* Probar funcionalidad del registro de un vendedor.
* Probar funcionalidad para la modificación de datos de un vendedor.
* Probar funcionalidad para la actualización/modificación del catálogo de autos.
* Probar funcionalidad del dashboard estadístico.


<i>Flujo del Vendedor:</i><br>
* Probar funcionalidad del Login.
* Probar la funcionalidad de búsqueda de catálogo.
* Probar la funcionalidad de filtrado de catálogo.
* Probar la funcionalidad de la búsqueda de solicitudes.
* Probar la funcionalidad del filtrado de solicitudes.
* Probar funcionalidad del manejo de una solicitud.
* Probar funcionalidad del sistema de chat.
* Probar funcionalidad del dashboard estadístico.

### 2.5 Alcance
<b>Flujo del Cliente:</b><br>
<i>1. Probar la funcionalidad de Login.</i><br>
* Acceso válido con Credenciales correctas de super-administrador.
* Acceso no autorizado con correo invalido/cuenta inexistente.
* Acceso no autorizado con contraseña incorrecta.

<i> 2. Probar la funcionalidad de búsqueda de catálogo.</i><br>
* Se hace una búsqueda de un auto dentro del catálogo
* El sistema muestra los resultados de los autos segun la búsqueda

<i>3. Probar la funcionalidad de filtrado de catálogo.</i><br>
* Dentro de la búsqueda de un auto del catálogo se muestran los filtros disponibles para la búsqueda
* Se seleccionan los filtros deseados
* El sistema muestra los resultados de los autos según los filtros aplicados

<i>4. Probar la funcionalidad del agendado de la prueba de manejo.</i><br>
* El usuario cliente selecciona el auto de su preferencia para solicitar una prueba de manejo
* Para poder solicitar la prueba es necesario que llene un formulario y suba los documentos necesarios
* Una vez completado lo anterior su solicitud se confirma y automáticamente se le asigna un usuario vendedor que le dará seguimiento a su solicitud
* El usuario vendedor se pone en contacto con el cliente a través del chat de la plataforma, en caso de que tenga dudas, además puede ver el estatus de su solicitud en un apartado donde se listaran las solicitudes del cliente
* El vendedor revisa los documentos de la solicitud, si están correctos se aprueban, de lo contrario el vendedor le tiene que notificar al cliente para que pueda volver a subir sus documentos correctamente
* Una vez que los documentos son aprobados por el vendedor, en caso de que el auto seleccionado se requiera pagar una cuota para la prueba de manejo, se hace la transacción necesaria 
* Una vez completada la transacción el cliente agenda su prueba de manejo

<i>5. Probar la funcionalidad de la subida de documentos para la solicitud de prueba de manejo.</i><br>
* El usuario cliente selecciona el auto de su preferencia para solicitar una prueba de manejo
* El cliente llena el formulario con los datos necesarios y sube los documentos que se le piden
* El vendedor revisa los documentos de la solicitud, si están correctos se aprueban, de lo contrario el vendedor le tiene que notificar al cliente para que pueda volver a subir sus documentos correctamente

<i>6. Probar la funcionalidad de la subida de documentos para la compra de un auto.</i><br>
* El usuario cliente selecciona un vehículo y solicita comprarlo
* Para poder solicitar la comprar es necesario que llene un formulario y suba los documentos necesarios
* Después de subirlos se le asignará un vendedor quien revisará sus documentos y le dará seguimiento a su compra
* Una vez que complete esto el cliente puede ver el estatus de su solicitud en un apartado donde se listaran sus solicitudes
* El vendedor al revisar los documentos si están correctos los aprueba y puede continuar con el proceso de compra, de lo contrario le tiene que notificar al usuario para que los vuelva a subir

<i>7. Probar la funcionalidad de la transacción del pago para la prueba de manejo.</i><br>
* Una vez que los documentos de la prueba de manejo fueron aprobados, si el vehículo necesita una cuota para realizar la prueba se le notifica al cliente
* El cliente revisa el seguimiento de su solicitud y hace el pago
* Una vez que termina el pago el sistema le confirma de recibido el pago y se actualiza el seguimiento

<i>8. Probar la funcionalidad de la transacción de la compra de auto</i><br>
* Una vez que los documentos de la compra fueron aprobados, se le notifica al cliente para pueda realizar el pago del vehículo
* El cliente revisa el seguimiento de su solicitud y hace el pago
* Una vez que termina el pago el sistema le confirma de recibido el pago y se actualiza el seguimiento

<i>9. Probar la funcionalidad del seguimiento de acciones del usuario (prueba de manejo o compras).</i><br>
* Una vez que el cliente sube los documentos necesarios ya sea para la prueba de manejo o para la compra de un auto puede realizar el seguimiento de su solicitud
* En el apartado indicado de seguimiento, puede ver en qué fase va su solicitud
* Mientras el vendedor asignado a su solicitud la revisa y mientras va avanzando el proceso el vendedor va actualizando la etapa en la que se encuentra el cliente

<i>10. Probar la funcionalidad del sistema de Chat.</i><br>
* Entrada a la vista de chats y contactos con acceso de cliente
* El cliente revisa si tiene algún mensaje
* Selecciona una conversación iniciada
* El vendedor y el cliente pueden tener un medio de contacto directo

<i>11. Probar la funcionalidad del sistema de favoritos (wishlist).</i><br>
* Se muestra el catálogo de autos
* Si al cliente le interesa algún auto lo marca como favorito
* En el apartado indicado el cliente puede revisar su lista de favoritos con los autos que marcó previamente 

<i>12. Probar la funcionalidad de la edición de datos en el perfil.</i><br>
* El cliente puede acceder a los ajustes de su cuenta en el apartado indicado
* Dentro de los ajustes puede seleccionar la opción de modificar sus datos
* Al entrar a la opción modifica los datos necesarios y al final selecciona el botón de guardar cambios
* Los datos se actualizan tanto en la vista del cliente, como en la base de datos


<b>Flujo del Super Administrador:</b><br>
<i>1. Probar la funcionalidad de Login.</i><br>
* Acceso válido con Credenciales correctas de super-administrador
* Acceso no autorizado con correo invalido/cuenta inexistente
* Acceso no autorizado con contraseña incorrecta

<i>2. Probar la funcionalidad de búsqueda de usuarios.</i><br>
* Se hace una búsqueda de un usuario dentro del catálogo
* El sistema muestra los resultados de los usuarios según la búsqueda

<i>3. Probar las funcionalidad de filtrado de usuarios.</i><br>
* Dentro de la búsqueda de usuarios se muestran los filtros disponibles para la búsqueda
* Se seleccionan los filtros deseados
* El sistema muestra los resultados de lo usuarios según los filtros aplicados

<i>4. Probar la funcionalidad de la modificación de datos de un grupo automotriz.</i><br>
* Se accede a la página de la cuenta del grupo automotriz con acceso de super-administrador
* Se efectúa un cambio de la información del grupo automotriz desde la página de la cuenta.
* Se guardan los cambios de la cuenta del grupo automotriz.

<i>5. Probar la funcionalidad de la búsqueda de solicitudes.</i><br>
* Se hace una búsqueda de una solicitud dentro del catálogo
* El sistema muestra los resultados de las solicitudes y sus estados

<i>6. Probar la funcionalidad del filtrado de solicitudes.</i><br>
* Dentro de la búsqueda de solicitudes se muestran los filtros disponibles para la búsqueda
* Se seleccionan los filtros deseados
* El sistema muestra los resultados de las solicitudes según los filtros aplicados (aprobada/pendiente/denegada)

<i>7. Probar funcionalidad de la aprobación/negación de una solicitud.</i><br>
* Se elige una solicitud pendiente con acceso de super-administrador
* Se efectúa la aprobación de una solicitud en espera
* Se efectúa la negación de una solicitud en espera

<i>8. Probar la funcionalidad del registro de un grupo automotriz.</i><br>
* Se accede al landing-page de creación de grupo automotriz.
* Creación exitosa de un grupo automotriz
* Acceso exitoso a la cuenta del grupo automotriz

<i>9. Probar la funcionalidad del dashboard estadístico.</i><br>
* Acceso al dashboard con una cuenta de nivel valido muestra las estadísticas y métricas de la plataforma
* Las estadísticas son válidas y representativas de los datos dentro del sistema
* Las opciones y parámetros presentes dentro de la vista permiten ver estadísticas particulares de acuerdo a la selección de las mismas.

<b>Flujo del Vendedor:</b><br>
<i>1. Probar funcionalidad del Login.</i><br>
* Acceso válido con Credenciales correctas de vendedor
* Acceso no autorizado con correo invalido/cuenta inexistente
* Acceso no autorizado con contraseña incorrecta

<i>2. Probar la funcionalidad de búsqueda de catálogo.</i><br>
* Se hace una búsqueda de un auto dentro del catálogo
* El sistema muestra los resultados de los autos segun la búsqueda
* Probar la funcionalidad de filtrado de catálogo.
* Dentro de la búsqueda de un auto del catálogo se muestran los filtros disponibles para la búsqueda
* Se seleccionan los filtros deseados
* El sistema muestra los resultados de los autos según los filtros aplicados

<i>3. Probar la funcionalidad de la búsqueda de solicitudes.</i><br>
* Se hace una búsqueda de una solicitud dentro del catálogo
* El sistema muestra los resultados de las solicitudes y sus estados

<i>4. Probar la funcionalidad del filtrado de solicitudes.</i><br>
* Dentro de la búsqueda de solicitudes se muestran los filtros disponibles para la búsqueda
* Se seleccionan los filtros deseados
* El sistema muestra los resultados de las solicitudes según los filtros aplicados (aprobada/pendiente/denegada)

<i>5. Probar funcionalidad del manejo de una solicitud.</i><br>
* Se elige una solicitud
* Dentro de la vista de solicitud se modifica la etapa de proceso.

<i>6. Probar funcionalidad del sistema de chat.</i><br>
* Entrada a la vista de chats y contactos con acceso de vendedor
* Selección de una conversación iniciada
* Creación de una conversación desde vista de contacto
* Enviar mensaje al cliente

<i>7. Probar funcionalidad del dashboard estadístico.</i><br>
* Acceso al dashboard con una cuenta de nivel valido muestra las estadísticas y métricas de la plataforma
* Las estadísticas son válidas y representativas de los datos dentro del sistema* Las opciones y parámetros presentes dentro de la vista permiten ver estadísticas particulares de acuerdo a la selección de las mismas.
			

### 2.6 Niveles de Pruebas
<p align="justify">A continuación se muestran el nivel de las pruebas que se realizarán durante el desarrollo del proyecto, además de detallar algunas de los métodos que se utilizaran al igual que los responsables de dichas pruebas.

#### <b>Pruebas Informales (Prueba Funcional)</b>
El propósito de este tipo de pruebas es verificar rápidamente el funcionamiento de los componentes del software. Las pruebas de este estilo no tienen ningún tipo de entrega.
- <i>Alcance:</i> Todas las secciones desarrolladas serán probadas mediante pruebas unitarias informales.
- <i>Responsables:</i> Los desarrolladores de software.
- <i>Metodología:</i> Los desarrolladores responsables del componentes se encargaran de realizar pruebas de Input-Output para comprobar su correcto funcionamiento.
- <i>Cada cuando:</i> En cuanto se finalice, o se modifique algún componente.

#### <b>Prueba de Caja Negra (Prueba Funcional)</b>
El propósito de las pruebas unitarias es probar cada uno de los componentes y funcionalidades  que comprenden la aplicación que se desarrollará.

- <i>Alcance:</i> Todas las secciones desarrolladas serán probadas mediante pruebas de caja negra.
- <i>Responsables:</i> Los desarrolladores de software y los testers.
- <i>Metodología:</i> Los desarrolladores probarán componentes de la aplicación sin tener conocimiento del código detrás de los mismos componentes, reportando errores en caso de encontrarlos. Específicamente, el tipo de pruebas de caja negra que se realizarán serán pruebas de tipo de casos de uso. Dentro de estas pruebas se realizarán tres baterías negativas y tres baterías positivas que se deberán cumplir cuando se realicen este tipo de pruebas.
- <i>Cada cuándo:</i> Al finalizar cada componente.

#### <b>Prueba de Caja Blanca (Prueba Funcional)</b>
El propósito de este tipo de pruebas es encontrar la causa de algún tipo de falla que se haya encontrado en otro tipo de pruebas. En específico, las pruebas de caja blanca que se realizan son pruebas de cobertura, es decir, se probarán los tres caminos más utilizados por los usuarios. Más aún, se considerará que los caminos seleccionados son apropiados si estos cubren un mínimo de 80%  de los caminos posibles. Este 80% debe regresar resultados de prueba positivos para así justificar que el componente funciona de manera correcta. 
- <i>Alcance:</i> Cualquier componente de software que presente alguna falla dentro de algún otro tipo de prueba.
- <i>Responsables:</i> Los desarrolladores de software y los testers.
- <i>Metodología:</i> Los desarrolladores que se encargaron de crear los componentes en donde se encontraron los errores serán los encargados de realizar pruebas de caja blanca con el objetivo de encontrar que pedazo de código es el que está causando dicho error.
- <i>Cada cuándo:</i> Al finalizar cada sprint.

#### <b>Prueba de Integración (Prueba Funcional)</b>
El propósito de las pruebas de integración es comprobar el correcto funcionamiento de la aplicación cuando todos los componentes son utilizados en conjunto. Para efectos de este proyecto, debido a las restricciones de tiempo, este tipo de pruebas sólo serán realizadas en los componentes críticos de la aplicación. 
- <i>Alcance:</i> Componentes críticos para el funcionamiento de la aplicación
- <i>Responsables:</i> Los responsables de cada célula de trabajo.
- <i>Metodología:</i> Los desarrolladores responsables de cada célula, al terminar más de un componente relacionado, empezaran a realizar pruebas e integración. De la misma manera, al terminar el proyecto, se realizarán  nuevas pruebas de este estilo.
- <i>Cada cuándo:</i> Al terminarse pedazos de software relacionados y al acabar todos los componentes de la aplicación.

#### <b>Prueba de Aceptación (Prueba Funcional)</b>
El propósito de este tipo de pruebas es validar con el equipo de desarrollo y NDS si el sistema está a la par con sus expectativas y cumple las funcionalidades que fueron discutidas en el documento SRS.
- <i>Alcance:</i> Todos los aspectos del pedazo de software serán probados pruebas de validación. Esto con el objetivo de revisar si aspectos de diseño y funcionalidad de la aplicación están a la par de las expectativas de NDS.
- <i>Responsables:</i> Rubén Raya (NDS), los desarrolladores, los testers y el SCRUM master..
- <i>Metodología:</i> Los desarrolladores se reunirán con Rubén Raya y bajo su supervisión se encargará de validar los aspectos importantes de la aplicación desarrollada.
- <i>Cada cuándo:</i>En cuanto se cumplan las pruebas de integración.

#### <b>Prueba de Recorrido Estático (Validación)</b>
El propósito de este tipo de pruebas es asegurar que el servicio, en términos de funcionalidad y desempeño, actúe de manera satisfactoria.
- <i>Alcance:</i> Dado que se trata de una prueba de sistema, el software será probado en completud.
- <i>Responsables:</i> Desarrolladores no pertenecientes al proyecto, los testers, el SCRUM master y Rubén Raya (NDS). Un recorrido se considera aceptado una vez que sea aprobado por el equipo de desarrolladores y Rubén Raya. Los responsables del proceso de validación son los desarrolladores no pertenecientes al proyecto, Esteban Castillo y Ruben Raya.  
- <i>Metodología:</i> Crear escenarios de acuerdo a las situaciones más usuales de los usuarios.
- <i>Cada cuándo:</i> Al final del proyecto.

### 2.7 Criterios de aceptación de pruebas

#### <b>Pruebas Informales</b>
<p align="justify"> Cada desarrollador tiene como responsabilidad realizar una prueba informal a cada componente que finalice. Ya que esta prueba no sigue una metodología específica, el desarrollador sabrá que el componente pasó la prueba si realiza de manera correcta su funcionalidad y trabaja de manera adecuada con otros componentes. 
 
#### <b>Pruebas Unitarias</b>
- <i>Funcionalidad de Login:</i> Esta funcionalidad nunca debe fallar. Todas las pruebas deben proporcionar el usuario y la página de inicio correctos, o bien enviar un mensaje de error indicando que el usuario no existe. Esto para cada tipo de usuario que permite la plataforma.

- <i>Funcionalidad de Registro:</i> Todas las pruebas deben de crear las credenciales ingresadas de forma correcta en la base de datos o bien enviar un mensaje de error indicando la razón por la cual las credenciales no son permitidas. Igualmente, el registro debe agregar la cuenta con los privilegios y permisos correspondientes a cada tipo de usuario.

- <i>Funcionalidad CRUD del Catálogo:</i> Todas las pruebas deben permitir la subida, lectura, modificación y eliminación de elementos del catálogo de autos. Esto debe de permitirse acorde a los permisos respectivos a cada tipo de cuenta, respetando los privilegios que conlleva cada una de ellas. Se debe de desplegar el mensaje de error correspondiente, si la información/datos por el usuario no es permitida/correcta.

- <i>Funcionalidad de Búsqueda del Catálogo:</i> Todas las pruebas deben permitir la búsqueda  de los autos dentro del catálogo con uso de lenguaje natural. Para todos los tipos de administradores que tienen acceso al catálogo pueden hacer una búsqueda de los autos que pertenecen a su respectivo grupo automotriz o a su respectiva agencia, para los clientes pueden hacer una búsqueda de todos los autos de todas las agencia. Los resultados mostrados deben ser relacionados a las palabras ingresadas en la barra de búsqueda, si no hay autos relacionados con las palabras ingresadas en la búsqueda, no se mostrarán resultados ya que no hay autos que coincidan. 

- <i>Funcionalidad de Filtrado del Catálogo:</i> Todas las pruebas deben permitir el filtrado de los autos dentro del catálogo con los filtros previamente determinados. Para todos los tipos de administradores que tienen acceso al catálogo pueden hacer un filtrado de la búsqueda de los autos que pertenecen a su respectivo grupo automotriz o a su respectiva agencia, para los clientes pueden hacer un filtrado de la búsqueda de todos los autos de todas las agencia. Los resultados mostrados deben ser según los filtros relacionados, si no hay autos que cumplan con las restricciones de los filtros, no se mostrarán resultados ya que no hay autos que coincidan. 

- <i>Funcionalidad de Búsqueda de Usuarios:</i> Todas las pruebas deben permitir la búsqueda de otros usuarios con uso de lenguaje natural. Para todos los tipos de administradores que tienen acceso a la búsqueda de otros usuarios pueden hacer una búsqueda de los usuarios que pertenecen a su respectivo grupo automotriz o a su respectiva agencia. Los resultados mostrados deben ser relacionados a las palabras ingresadas en la barra de búsqueda, si no hay usuarios relacionados con las palabras ingresadas en la búsqueda, no se mostrarán resultados ya que no hay usuarios que coincidan. 

- <i>Funcionalidad de Filtrado de usuarios:</i> Todas las pruebas deben permitir el filtrado de los usuarios con los filtros previamente determinados. Para todos los tipos de administradores que tienen acceso a la búsqueda de otros usuarios pueden hacer un filtrado de la búsqueda de los autos que pertenecen a su respectivo grupo automotriz o a su respectiva agencia. Los resultados mostrados deben ser según los filtros relacionados, si no hay usuarios que cumplan con las restricciones de los filtros, no se mostrarán resultados ya que no hay usuarios que coincidan. 

- <i>Funcionalidad de Pago:</i> Todas las pruebas deben permitir que el usuario pueda realizar el pago de un auto mediante cada uno de los diferentes métodos de pago que ofrece la plataforma. Se deben de desplegar mensajes ya sea de éxito en la transacción o falla en la misma, indicando al usuario si hay una razón de su lado por la cual no fue posible efectuar el pago. 

- <i>Funcionalidad de Chat:</i> Todas las pruebas deben permitir que el usuario pueda seleccionar a otro usuario y comunicarse con este efectivamente mediante mensajes. Los mensajes enviados deben de ser visibles y mostrarse en la cuenta receptora, con la capacidad de mostrar un mensaje de error indicando al usuario la razón por la cual no se pudo enviar el mismo.

- <i>Funcionalidad de Favoritos (Wishlist):</i> Todas las pruebas deben permitir que el usuario pueda marcar como “favorito” a todos los autos que desea, así como visualizarlos correctamente en la sección de “wishlist”. Asimismo, el usuario siempre debe de ser capaz de eliminar a cualquier auto de dicha lista, donde los cambios deberán reflejarse correctamente.

- <i>Funcionalidad Analítica:</i> Todas las pruebas deben permitir que cada tipo de usuario pueda visualizar correctamente las estadísticas e información adecuada para los permisos que le corresponden a dicha cuenta. Esta funcionalidad siempre deberá estar activa, y de haber un error en el lado del servidor, se deberá indicar con un mensaje respectivamente.

#### <b>Pruebas de Integración</b>
- <i>Manejo de Solicitudes:</i> Todas las pruebas deberán permitir que el usuario en cuestión (Super-Admin y Vendedor) pueda modificar el estado/etapa de cualquier solicitud a su cargo. Asimismo, debe ser posible comentar acerca del estado de una solicitud así informando al aplicante las acciones que debe realizar, o razones que justifican el estado de su solicitud. Finalmente, el usuario que maneja las solicitudes debe de poder negar o aceptar cualquier solicitud. Todo lo descrito anteriormente, debe siempre verse reflejado en la cuenta del usuario aplicante.

- <i>Compra de un Auto:</i> Todas las pruebas deberán permitir que el cliente tenga la capacidad de comprar un auto exitosamente, y que este pase por las dos posibilidades principales en el proceso de compra, siendo la aceptación o negación de la solicitud. Para ello, el cliente debe ser capaz de seleccionar un auto junto con sus especificaciones, aplicar para la compra del mismo, subir la información y documentos necesarios, darle seguimiento a su solicitud, esperar la aceptación/negación de la misma, efectuar la compra por uno de los métodos de pago disponible, continuar la comunicación con el vendedor el tiempo que sea necesario para finalmente recibir su adquisición. 

- <i>Agendado de la prueba de manejo:</i> Todas las pruebas deberán permitir que el cliente tenga la capacidad de agendar una prueba de manejo exitosamente, y que este pase por las dos posibilidades principales en el proceso de agendado, siendo la aceptación o negación de la solicitud. Para ello, el cliente debe ser capaz de seleccionar un auto, solicitar una prueba de manejo para el mismo, subir la información y documentación necesaria, darle seguimiento a la solicitud, y de ser aceptada seleccionar una fecha, lugar y hora disponible en el horario del vendedor. Asimismo, la comunicación entre el cliente y el vendedor debe de ser posible en todo momento como parte del seguimiento de la prueba de manejo. 

#### <b>Pruebas de Validación/Aceptación</b>
<p align="justify">Los clientes y representantes de los mismos están satisfechos con la funcionalidad revisada así como la experiencia del usuario (UI/UX)  de la plataforma.

#### <b>Pruebas Estáticas de Recorrido</b>
<p align="justify">Es posible completar el flujo básico de la plataforma para cada uno de los tipos de usuario, desde el registro, login hasta cada una de sus acciones principales. 

### 2.8 Entregables de Pruebas

<table>
<thead>
  <tr>
    <th>No.</th>
    <th>Nombre de Entregable</th>
    <th>Autor</th>
    <th>Reviewer</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>1.</td>
    <td>Plan de Pruebas</td>
    <td>Director de Pruebas</td>
    <td>Project Manager/Analista de Negocios</td>
  </tr>
  <tr>
    <td>2.<br></td>
    <td>Revisión Técnica Formal</td>
    <td>Director de Pruebas</td>
    <td>Project Manager/Analista de Negocios</td>
  </tr>
  <tr>
    <td>3.</td>
    <td>Resultados de Pruebas Unitarias</td>
    <td>Equipo de Pruebas</td>
    <td>Project Manager</td>
  </tr>
  <tr>
    <td>4.</td>
    <td>Resultados de Pruebas Integrales</td>
    <td>Equipo de Pruebas</td>
    <td>Project Manager</td>
  </tr>
  <tr>
    <td>5.</td>
    <td>Resultados de Pruebas de Validación</td>
    <td>Equipo de Pruebas</td>
    <td>Project Manager</td>
  </tr>
  <tr>
    <td>6.</td>
    <td>Resultados de la Prueba de Sistema</td>
    <td>Equipo de Pruebas</td>
    <td>Project Manager</td>
  </tr>
  <tr>
    <td>7.</td>
    <td>Reporte Diario/Semanal del Estatus</td>
    <td>Director de Pruebas/ Equipo de Pruebas</td>
    <td>Director de Pruebas/Project Manager</td>
  </tr>
  <tr>
    <td>8.</td>
    <td>Reporte de Cierre</td>
    <td>Director de Pruebas</td>
    <td>Project Manager</td>
  </tr>
</tbody>
</table>


