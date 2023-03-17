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


# 1. Introducción

## 1.1 Propósito
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

# 2. Estrategia de Pruebas 
## 2.1 Descripción de Pruebas
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

## 2.2 Objetivo de las Pruebas
<p align="justify"> El objetivo de las pruebas que se realizarán durante el transcurso del proyecto es la validación de las funcionalidades fundamentales de la aplicación, al igual que comprobar la correcta implementación de los requerimientos establecidos en el documento SRS. En consideración de este objetivo, las pruebas a realizarse comprenderán:<br>

* Pruebas que aseguren la correcta autorización de usuarios, al igual que la asignación de los premios asociados.
* Pruebas que comprueben el correcto funcionamiento en la búsqueda y filtrado del catálogo de autos.
* Pruebas que comprueben el correcto funcionamiento del guardado de automóviles en la base de datos.
* Pruebas que garanticen el funcionamiento de la recopilación, análisis, y generación de estadística relacionada con usuarios agentes de la aplicación.
* Pruebas relacionadas al servicio de chat implementado en la aplicación.
Pruebas con el objetivo de comprobar el correcto funcionamiento del proceso de compra de un automóvil.
* Pruebas asociadas a la creación de usuarios con diferentes permisos. 
* Pruebas asociadas al funcionamiento de un software estable y listo para producción.

## 2.3 Suposiciones de las Pruebas
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

## 2.4 Objetivos de las Pruebas
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

## 2.5 Alcance
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

	
<b>Flujo del Grupo Automotriz:</b><br>

<b>Etapa 1:</b><br>
<i>Probar funcionalidad del Login.</i>
* Acceso válido con Credenciales correctas de super-administrador
* Acceso no autorizado con correo invalido/cuenta inexistente
* Acceso no autorizado con contraseña incorrecta

<i>Probar funcionalidad para realizar una aplicación.</i>
* Publicación válida de documentos.
* Publicación válida de datos.
* Subida de la creación de la aplicación en la plataforma.

<i>Probar funcionalidad del panel de seguimiento a una aplicación</i>
* Es posible eliminar los archivos subidos.
* Es posible volver a subir archivos después de haber eliminado los mismos.
* Es posible modificar la información subida.
* los cambios realizados a la aplicación se guardan correctamente.

<i>Probar funcionalidad de la modificación de los datos del perfil.</i>
* Es posible eliminar y reescribir cada rubro en la información del perfil.
* Los cambios se guardan correctamente.

<i>Probar funcionalidad de la eliminación de una cuenta.</i>
* El sistema muestra una opción para borrar la cuenta.
* El sistema verifica que el usuario desea eliminar su cuenta.

<b>Etapa 2:</b><br>
<i>Probar funcionalidad de Login.</i>
* Acceso válido con Credenciales correctas de super-administrador
* Acceso no autorizado con correo invalido/cuenta inexistente
* Acceso no autorizado con contraseña incorrecta

<i>Probar funcionalidad del registro de una agencia.</i>
* Se accede al landing-page de creación de una agencia
* Creación exitosa de una agencia
* Acceso exitoso a la cuenta de la agencia

<i>Probar funcionalidad de la búsqueda de usuarios.</i>
* Se hace una búsqueda de un usuario dentro del buscador.
* El sistema muestra los resultados de los usuarios encontrados según la búsqueda.

<i>Probar funcionalidad del filtrado de usuarios.</i>
* Dentro de la búsqueda se muestran los filtros disponibles para la búsqueda.
* Se seleccionan los filtros deseados.
* El sistema muestra los resultados de los usuarios según los filtros aplicados.

<i>Probar funcionalidad para la modificación de datos de una agencia.</i>
* Se accede a la página de la cuenta de la agencia.
* Se efectúa un cambio de la información de la agencia desde la página de la cuenta.
* Se guardan los cambios de la cuenta de la agencia.

<i>Probar funcionalidad del dashboard estadístico.</i>
* Acceso al dashboard con una cuenta de nivel valido muestra las estadísticas y métricas de la plataforma
* Las estadísticas son válidas y representativas de los datos dentro del sistema.
* Las opciones y parámetros presentes dentro de la vista permiten ver estadísticas particulares de acuerdo a la selección de las mismas.

<b>Flujo de la Agencia:</b><br>

<i>Probar funcionalidad de Login.</i>
* Acceso válido con Credenciales correctas de super-administrador.
* Acceso no autorizado con correo invalido/cuenta inexistente.
* Acceso no autorizado con contraseña incorrecta.

<i>Probar funcionalidad de la búsqueda de usuarios.</i>
* Se hace una búsqueda de un usuario dentro del buscador.
* El sistema muestra los resultados de los usuarios encontrados según la búsqueda.

<i>Probar funcionalidad del filtrado de usuarios.</i>
* Dentro de la búsqueda se muestran los filtros disponibles para la búsqueda.
* Se seleccionan los filtros deseados.
* El sistema muestra los resultados de los usuarios según los filtros aplicados.

<i>Probar funcionalidad del registro de un gerente.</i>
* Se accede al landing-page de creación de un gerente.
* Creación exitosa de un gerente
* Acceso exitoso a la cuenta del gerente.

<i>Probar funcionalidad para la modificación de datos de un gerente.</i>
* Se accede a la página de la cuenta del gerente.
* Se efectúa un cambio de la información del gerente desde la página de la cuenta.
* Se guardan los cambios de la cuenta del gerente.

<i>Probar funcionalidad para la actualización/modificación del catálogo de autos.</i>
* Se presenta la opción de agregar un auto.
* Se suben correctamente las imágenes.
* Se suben correctamente los datos ingresados.
* Se presenta la opción de editar un auto.
* Se reemplazan correctamente las imágenes previamente subidas por las nuevas.
* Es posible cambiar cada rubro de la información de un auto.
* Se guarda correctamente la publicación del auto o la modificación según sea el caso.

<i>Probar funcionalidad del dashboard estadístico.</i>
* Acceso al dashboard con una cuenta de nivel valido muestra las estadísticas y métricas de la plataforma
* Las estadísticas son válidas y representativas de los datos dentro del sistema.
* Las opciones y parámetros presentes dentro de la vista permiten ver estadísticas * particulares de acuerdo a la selección de las mismas.

<b>Flujo del Gerente:</b><br>
<i>Probar funcionalidad de Login.</i>
* Acceso válido con Credenciales correctas de super-administrador.
* Acceso no autorizado con correo invalido/cuenta inexistente.
* Acceso no autorizado con contraseña incorrecta.
<i>Probar funcionalidad de la búsqueda de usuarios.</i>
* Se hace una búsqueda de un usuario dentro del buscador.
* El sistema muestra los resultados de los usuarios encontrados según la búsqueda.

<i>Probar funcionalidad del filtrado de usuarios.</i>
* Dentro de la búsqueda se muestran los filtros disponibles para la búsqueda.
* Se seleccionan los filtros deseados.
* El sistema muestra los resultados de los usuarios según los filtros aplicados.

<i>Probar funcionalidad del registro de un vendedor.</i>
* Se accede al landing-page de creación de un vendedor.
* Creación exitosa de un vendedor.
* Acceso exitoso a la cuenta del vendedor.

<i>Probar funcionalidad para la modificación de datos de un vendedor.</i>
* Se accede a la página de la cuenta del vendedor.
* Se efectúa un cambio de la información del vendedor desde la página de la cuenta.
* Se guardan los cambios de la cuenta del vendedor.

<i>Probar funcionalidad para la actualización/modificación del catálogo de autos.</i>
* Se presenta la opción de agregar un auto.
* Se suben correctamente las imágenes.
* Se suben correctamente los datos ingresados.
* Se presenta la opción de editar un auto.
* Se reemplazan correctamente las imágenes previamente subidas por las nuevas.
* Es posible cambiar cada rubro de la información de un auto.
* Se guarda correctamente la publicación del auto o la modificación según sea el caso.

<i>Probar funcionalidad del dashboard estadístico.</i>
* Acceso al dashboard con una cuenta de nivel valido muestra las estadísticas y métricas de la plataforma
* Las estadísticas son válidas y representativas de los datos dentro del sistema.
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
			

## 2.6 Niveles de Pruebas
<p align="justify">A continuación se muestran el nivel de las pruebas que se realizarán durante el desarrollo del proyecto, además de detallar algunas de los métodos que se utilizaran al igual que los responsables de dichas pruebas.

### <b>Pruebas Informales (Prueba Funcional)</b>
El propósito de este tipo de pruebas es verificar rápidamente el funcionamiento de los componentes del software. Las pruebas de este estilo no tienen ningún tipo de entrega.
- <i>Alcance:</i> Todas las secciones desarrolladas serán probadas mediante pruebas unitarias informales.
- <i>Responsables:</i> Los desarrolladores de software.
- <i>Metodología:</i> Los desarrolladores responsables del componentes se encargaran de realizar pruebas de Input-Output para comprobar su correcto funcionamiento.
- <i>Cada cuando:</i> En cuanto se finalice, o se modifique algún componente.

### <b>Prueba de Caja Negra (Prueba Funcional)</b>
El propósito de las pruebas unitarias es probar cada uno de los componentes y funcionalidades  que comprenden la aplicación que se desarrollará.

- <i>Alcance:</i> Todas las secciones desarrolladas serán probadas mediante pruebas de caja negra.
- <i>Responsables:</i> Los desarrolladores de software y los testers.
- <i>Metodología:</i> Los desarrolladores probarán componentes de la aplicación sin tener conocimiento del código detrás de los mismos componentes, reportando errores en caso de encontrarlos. Específicamente, el tipo de pruebas de caja negra que se realizarán serán pruebas de tipo de casos de uso. Dentro de estas pruebas se realizarán tres baterías negativas y tres baterías positivas que se deberán cumplir cuando se realicen este tipo de pruebas.
- <i>Cada cuándo:</i> Al finalizar cada componente.

### <b>Prueba de Caja Blanca (Prueba Funcional)</b>
El propósito de este tipo de pruebas es encontrar la causa de algún tipo de falla que se haya encontrado en otro tipo de pruebas. En específico, las pruebas de caja blanca que se realizan son pruebas de cobertura, es decir, se probarán los tres caminos más utilizados por los usuarios. Más aún, se considerará que los caminos seleccionados son apropiados si estos cubren un mínimo de 80%  de los caminos posibles. Este 80% debe regresar resultados de prueba positivos para así justificar que el componente funciona de manera correcta. 
- <i>Alcance:</i> Cualquier componente de software que presente alguna falla dentro de algún otro tipo de prueba.
- <i>Responsables:</i> Los desarrolladores de software y los testers.
- <i>Metodología:</i> Los desarrolladores que se encargaron de crear los componentes en donde se encontraron los errores serán los encargados de realizar pruebas de caja blanca con el objetivo de encontrar que pedazo de código es el que está causando dicho error.
- <i>Cada cuándo:</i> Al finalizar cada sprint.

### <b>Prueba de Integración (Prueba Funcional)</b>
El propósito de las pruebas de integración es comprobar el correcto funcionamiento de la aplicación cuando todos los componentes son utilizados en conjunto. Para efectos de este proyecto, debido a las restricciones de tiempo, este tipo de pruebas sólo serán realizadas en los componentes críticos de la aplicación. 
- <i>Alcance:</i> Componentes críticos para el funcionamiento de la aplicación
- <i>Responsables:</i> Los responsables de cada célula de trabajo.
- <i>Metodología:</i> Los desarrolladores responsables de cada célula, al terminar más de un componente relacionado, empezaran a realizar pruebas e integración. De la misma manera, al terminar el proyecto, se realizarán  nuevas pruebas de este estilo.
- <i>Cada cuándo:</i> Al terminarse pedazos de software relacionados y al acabar todos los componentes de la aplicación.

### <b>Prueba de Aceptación (Prueba Funcional)</b>
El propósito de este tipo de pruebas es validar con el equipo de desarrollo y NDS si el sistema está a la par con sus expectativas y cumple las funcionalidades que fueron discutidas en el documento SRS.
- <i>Alcance:</i> Todos los aspectos del pedazo de software serán probados pruebas de validación. Esto con el objetivo de revisar si aspectos de diseño y funcionalidad de la aplicación están a la par de las expectativas de NDS.
- <i>Responsables:</i> Rubén Raya (NDS), los desarrolladores, los testers y el SCRUM master..
- <i>Metodología:</i> Los desarrolladores se reunirán con Rubén Raya y bajo su supervisión se encargará de validar los aspectos importantes de la aplicación desarrollada.
- <i>Cada cuándo:</i>En cuanto se cumplan las pruebas de integración.

### <b>Prueba de Recorrido Estático (Validación)</b>
El propósito de este tipo de pruebas es asegurar que el servicio, en términos de funcionalidad y desempeño, actúe de manera satisfactoria.
- <i>Alcance:</i> Dado que se trata de una prueba de sistema, el software será probado en completud.
- <i>Responsables:</i> Desarrolladores no pertenecientes al proyecto, los testers, el SCRUM master y Rubén Raya (NDS). Un recorrido se considera aceptado una vez que sea aprobado por el equipo de desarrolladores y Rubén Raya. Los responsables del proceso de validación son los desarrolladores no pertenecientes al proyecto, Esteban Castillo y Ruben Raya.  
- <i>Metodología:</i> Crear escenarios de acuerdo a las situaciones más usuales de los usuarios.
- <i>Cada cuándo:</i> Al final del proyecto.

## 2.7 Criterios de aceptación de pruebas

### <b>Pruebas Informales</b>
<p align="justify"> Cada desarrollador tiene como responsabilidad realizar una prueba informal a cada componente que finalice. Ya que esta prueba no sigue una metodología específica, el desarrollador sabrá que el componente pasó la prueba si realiza de manera correcta su funcionalidad y trabaja de manera adecuada con otros componentes. 
 
### <b>Pruebas Unitarias</b>
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

### <b>Pruebas de Integración</b>
- <i>Manejo de Solicitudes:</i> Todas las pruebas deberán permitir que el usuario en cuestión (Super-Admin y Vendedor) pueda modificar el estado/etapa de cualquier solicitud a su cargo. Asimismo, debe ser posible comentar acerca del estado de una solicitud así informando al aplicante las acciones que debe realizar, o razones que justifican el estado de su solicitud. Finalmente, el usuario que maneja las solicitudes debe de poder negar o aceptar cualquier solicitud. Todo lo descrito anteriormente, debe siempre verse reflejado en la cuenta del usuario aplicante.

- <i>Compra de un Auto:</i> Todas las pruebas deberán permitir que el cliente tenga la capacidad de comprar un auto exitosamente, y que este pase por las dos posibilidades principales en el proceso de compra, siendo la aceptación o negación de la solicitud. Para ello, el cliente debe ser capaz de seleccionar un auto junto con sus especificaciones, aplicar para la compra del mismo, subir la información y documentos necesarios, darle seguimiento a su solicitud, esperar la aceptación/negación de la misma, efectuar la compra por uno de los métodos de pago disponible, continuar la comunicación con el vendedor el tiempo que sea necesario para finalmente recibir su adquisición. 

- <i>Agendado de la prueba de manejo:</i> Todas las pruebas deberán permitir que el cliente tenga la capacidad de agendar una prueba de manejo exitosamente, y que este pase por las dos posibilidades principales en el proceso de agendado, siendo la aceptación o negación de la solicitud. Para ello, el cliente debe ser capaz de seleccionar un auto, solicitar una prueba de manejo para el mismo, subir la información y documentación necesaria, darle seguimiento a la solicitud, y de ser aceptada seleccionar una fecha, lugar y hora disponible en el horario del vendedor. Asimismo, la comunicación entre el cliente y el vendedor debe de ser posible en todo momento como parte del seguimiento de la prueba de manejo. 

### <b>Pruebas de Validación/Aceptación</b>
<p align="justify">Los clientes y representantes de los mismos están satisfechos con la funcionalidad revisada así como la experiencia del usuario (UI/UX)  de la plataforma.

### <b>Pruebas Estáticas de Recorrido</b>
<p align="justify">Es posible completar el flujo básico de la plataforma para cada uno de los tipos de usuario, desde el registro, login hasta cada una de sus acciones principales. 

## 2.8 Entregables de Pruebas

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

## 2.9 Lista de Hitos
La lista de hitos es tentativa y puede cambiar por las siguientes razones:
1. Cualquier problema con la preparación del entorno del Sistema
2. Cualquier cambio en el alcance o cosas agregadas al alcance del proyecto
3. Cualquier otra dependencia que afecte el esfuerzo y el tiempo

<table>
  <thead>
    <tr>
      <th>
        No.
      </th>
      <th>
        Tipo de prueba
      </th>
      <th>
        Ejemplo de Prueba (SUT)
      </th>
      <th>
        Dependencia (DOC)
      </th>
    </tr>
  </thead>
    <tr>
      <td>
        1
      </td>
      <td>
        Pruebas Unitarias
      </td>
      <td>
        Registro de la Plataforma: Probar que el proceso de registro funciona correctamente para cada tipo de usuario.
      </td>
      <td>
        - Base de Datos Completada y conectada. <br> 
        - API Completado y Funcional.
      </td>
    </tr>
    <tr>
      <td>
        2
      </td>
      <td>
        Pruebas Unitarias
      </td>
      <td>
        Login de la Plataforma: Probar que el proceso de Login funciona correctamente para cada tipo de usuario.
      </td>
      <td>
        - Base de Datos Completada y conectada. <br>
        - API Completado y Funcional. <br>
        - Configuraci&oacute;n de Autenticaci&oacute;n y Autorizaci&oacute;n <br>
      </td>
    </tr>
    <tr>
      <td>
        3
      </td>
      <td>
        Pruebas Unitarias
      </td>
      <td>
        Modificaci&oacute;n del Cat&aacute;logo:&nbsp;Probar que los usuarios autorizados pueden subir, modificar y eliminar elementos del cat&aacute;logo correctamente.
      </td>
      <td>
        - Base de Datos Completada y conectada. <br>
        - API Completado y Funcional. <br>
        - Configuraci&oacute;n de privilegios completada.
      </td>
    </tr>
    <tr>
      <td>
        4
      </td>
      <td>
        Pruebas Unitarias
      </td>
      <td>
        Funcionalidad de B&uacute;squeda:&nbsp;Probar que los diferentes tipos de usuarios pueden buscar correctamente la informaci&oacute;n que desean mediante la barra de navegaci&oacute;n 
      </td>
      <td>
        - Base de Datos Completada y conectada. <br>
        - API Completado y Funcional.
      </td>
    </tr>
    <tr>
      <td>
        5
      </td>
      <td>
        Pruebas Unitarias
      </td>
      <td>
        Funcionalidad de Filtrado: Probar que los diferentes tipos de usuarios pueden filtrar correctamente la informaci&oacute;n que desean.
      </td>
      <td>
        - Base de Datos Completada y conectada. <br>
        - API Completado y Funcional.
      </td>
    </tr>
    <tr>
      <td>
        6
      </td>
      <td>
        Pruebas Unitarias
      </td>
      <td>
        Funcionalidad de Pago: Probar el proceso de pagos asegurando que los usuarios pueden completar el pago de un auto de manera f&aacute;cil y segura.
      </td>
      <td>
        - Integraci&oacute;n de la herramienta externa de Pago/Transacciones (Stripe)
      </td>
    </tr>
    <tr>
      <td>
        7
      </td>
      <td>
        Pruebas Unitarias
      </td>
      <td>
        Funcionalidad de Chat: Probar que los diferentes tipos de usuario pueden comunicarse exitosamente entre s&iacute; mediante el Chat interno de la plataforma.</span>
        </p>
      </td>
      <td>
        - Base de Datos completada y conectada. <br>
        - Integraci&oacute;n de librer&iacute;a externa para desarrollo del Chat (Socket IO).
      </td>
    </tr>
    <tr>
      <td>
        8
      </td>
      <td>
        Pruebas Unitarias
      </td>
      <td>
        Funcionalidad de Favoritos: Probar que los usuarios puedan seleccionar y guardar sus autos favoritos.
      </td>
      <td>
        - Base de Datos Completada y conectada. <br>
        - API Completado y Funcional.
      </td>
    </tr>
    <tr>
      <td>
        9
      </td>
      <td>
        Pruebas Unitarias 
      </td>
      <td>
        Funcionalidad de An&aacute;lisis de Documentos: Probar que autom&aacute;ticamente se analiza correctamente la validez de un documento.
      </td>
      <td>
        - Integraci&oacute;n de servicio de AWS Textract
      </td>
    </tr>
    <tr>
      <td>
        10
      </td>
      <td>
        Pruebas Unitarias
      </td>
      <td>
        Funcionalidad Anal&iacute;tica: Probar que el dashboard muestre la informaci&oacute;n estad&iacute;stica correcta y adecuada para cada tipo de usuario.
      </td>
      <td>
        - Base de Datos Completada y conectada. 
      </td>
    </tr>
    <tr>
      <td>
        11
      </td>
      <td>
        Pruebas Integrales
      </td>
      <td>
        Manejo de Solicitudes: Probar que la plataforma maneja correctamente y actualiza la informaci&oacute;n referente a el estado de las solicitudes tanto de compra como de prueba de manejo.
      </td>
      <td>
        - Base de Datos Completada y Conectada. <br>
        - Interfaz de modificaci&oacute;n de solicitudes completada. 
      </td>
    </tr>
    <tr>
      <td>
        12
      </td>
      <td>
        Pruebas Integrales
      </td>
      <td>
        Compra de un auto: Probar que el proceso de compra funciona en todos sus casos (tanto de aprobaci&oacute;n como negaci&oacute;n de la solicitud).
      </td>
      <td>
        - Conexi&oacute;n funcional entre estado de solicitud y cliente. <br>
        - An&aacute;lisis de documentos completamente funcional. <br>
        - Sistema de Chat completamente funcional. <br>
        - Funcional completa del sistema de pagos. <br>
      </td>
    </tr>
    <tr>
      <td>
        13
      </td>
      <td>
        Pruebas Integrales
      </td>
      <td>
        Agendado de una prueba de manejo: Probar que el proceso de agendado de un prueba de manejo funciona en todos sus casos (aprobaci&oacute;n y negaci&oacute;n de la solicitud).
      </td>
      <td>
        - Conexi&oacute;n funcional entre estado de solicitud y cliente. <br>
        - An&aacute;lisis de documentos completamente funcional. <br>
        - Sistema de Chat completamente funcional. <br>
        - Conexi&oacute;n funcional entre agenda del vendedor y el cliente. <br>
      </td>
    </tr>
    <tr>
      <td>
        14
      </td>
      <td>
        Pruebas de Validaci&oacute;n/Aceptaci&oacute;n
      </td>
      <td>
        El dise&ntilde;o (UI/UX) cumple con los est&aacute;ndares del cliente.
      </td>
      <td>
        Interfaz de dise&ntilde;o completada.
      </td>
    </tr>
    <tr>
      <td>
        15
      </td>
      <td>
        Pruebas Est&aacute;ticas de Recorrido
      </td>
      <td>
        Cada uno de los flujos para cada tipo de usuario se relacionan correctamente entre s&iacute;, y cumplen con los est&aacute;ndares y funcionalidad solicitada por el cliente.
      </td>
      <td>
        - Conexi&oacute;n e integraci&oacute;n completa entre el front-end y back-end. <br>
        - Configuraciones de seguridad completas. 
      </td>
    </tr>
    <tr>
      <td>
        16
      </td>
      <td>
        Manual de Usuario
      </td>
      <td>
        Se documenta el instructivo de uso para cada uno de los flujos de la plataforma.
      </td>
      <td>
        - Software completado y flujo completamente funcional
      </td>
    </tr>
  </table>

## 2.10 Estimación de esfuerzo de las pruebas

### Pruebas Estáticas
<table>
  <thead>
    <tr>
      <th>
        Tipo de Prueba
      </th>
      <th>
        Horas
      </th>
      <th>
        D&iacute;as
      </th>
      <th>
        Porcentaje del Proyecto
      </th>
    </tr>
  </thead>
    <tr>
      <td>
        SRS
      </td>
      <td>
        56 
      </td>
      <td>
        7
      </td>
      <td>
        7.72%
      </td>
    </tr>
    <tr>
      <td>
        Plan de Pruebas
      </td>
      <td>
        56
      </td>
      <td>
        7 
      </td>
    </tr>
    <tr>
      <td>
        Recorrido Est&aacute;tico
      </td>
      <td>
        24
      </td>
      <td>
        3
      </td>
    </tr>
  </table>

### Pruebas Funcionales

<table>
  <thead>
    <tr>
      <th>
        Tipo de Prueba
      </th>
      <th>
        Horas
      </th>
      <th>
        D&iacute;as
      </th>
      <th>
        Porcentaje del Proyecto
      </th>
    </tr>
  </thead>
    <tr>
      <td>
        Pruebas Informales
      </td>
      <td>
        N/A
      </td>
      <td>
        N/A
      </td>
      <td>
        10.61%
      </td>
    </tr>
    <tr>
      <td>
        Pruebas de Integraci&oacute;n
      </td>
      <td>
        28
      </td>
      <td>
        3.5
      </td>
    </tr>
    <tr>
      <td>
        Pruebas de Caja Negra
      </td>
      <td>
        56
      </td>
      <td>
        7
      </td>
    </tr>
    <tr>
      <td>
        Pruebas de Caja Blanca
        *porcentaje variable dependiendo de qu&eacute; componentes lo necesiten</span>
        </p>
      </td>
      <td>
        98
      </td>
      <td>
        12.25
      </td>
    </tr>
  </table>

La estimación de esfuerzos anterior representa un 18.33% del total del proyecto.


# 3. Proceso de gestión de pruebas
## 3.1 Proceso de ejecución de pruebas

1. Aprobación del plan de pruebas y funcionamiento del ambiente de pruebas en todos los dispositivos que serán utilizados.
  
    - El ambiente de pruebas se comprueba por medio de una prueba informal que hagan de manera individual los desarrolladores. 

2. Siguiendo el cronograma del proyecto y el plan de pruebas, el project manager en conjunto con el líder de pruebas asignará a cada líder sus respectivas pruebas.

3. Conforme se finalicen componentes pero el cronograma no indique una prueba, los desarrolladores estarán a cargo de las pruebas informales, y darles seguimiento.

4. Cuando se indique la ejecución de una prueba, cada líder tiene la responsabilidad de asegurarse de delegar las pruebas a sus equipos y darles seguimiento. 

5. Cada desarrollador encargado de una prueba tiene la responsabilidad de documentar su proceso, el resultado de dicha prueba, el seguimiento que se le dará y la corrección de los errores. 

    - El desarrollador tiene la responsabilidad de hacer su proceso de QA e informar si se pasa o no la prueba.

    - Primero se ejecutarán las pruebas de caja negra y en caso de que algún componente falle dicha prueba, se aplicará la prueba de caja blanca de cobertura en general y en algún componente crítico camino básico.

    - Una vez que cada componente pase las pruebas unitarias, se ejecutarán las pruebas de integración.

6. El desarrollador tiene la responsabilidad de informar a sus respectivos líderes acerca del resultado de las pruebas de sus componentes. 

7. Si hay fallas, se le informará a los líderes y al project manager de acuerdo a la gravedad de ellas y se incluirán capturas de pantalla y llenar los formularios propuestos, si es necesario.

8. Este proceso se repite hasta que todos los casos de prueba se ejecuten por completo y tengan un estado en el que ya sea que pasen o fallen.

    - Durante el ciclo siguiente, se probarán las pruebas falladas corregidas y los resultados se actualizarán en el documento durante el ciclo hasta que todas las pruebas pasen. El proceso continúa hasta que se llegue a un estándar comercial, promoviendo fiabilidad, fácil acceso y alta estabilidad.

## 3.2 Riesgos de prueba y factores de mitigación

<table>
  <thead>
    <tr>
      <th>
        ID
      </th>
      <th>
        Riesgo
      </th>
      <th>
        Fase del Proyecto
      </th>
      <th>
        Sprint
      </th>
      <th>
        Descripci&oacute;n
      </th>
      <th>
        Acciones de Mitigaci&oacute;n
      </th>
      <th>
        Estatus
      </th>
      <th>
        Due&ntilde;o
      </th>
      <th>
        Probabilidad
      </th>
      <th>
        Impacto
      </th>
    </tr>
  </thead>
    <tr>
      <td>
        R_01
      </td>
      <td>
        Que no se d&eacute; el presupuesto necesario para el hosting de la plataforma en la nube.
      </td>
      <td>
        Cloud Deployment
      </td>
      <td>
        Desde 7
      </td>
      <td>
        Los servicios de cloud son costosos pero garantizan seguridad y escalabilidad, se debe de llegar a un acuerdo con el Tec para el uso de estos servicios
      </td>
      <td>
        - Contar con alternativas gratuitas de respaldo como las cuentas con &quot;trial&quot; del servicio con suficiente alcance de tiempo para la entrega del proyecto.
      </td>
      <td>
      </td>
      <td>
        G501
      </td>
      <td>
        Media
      </td>
      <td>
        Alto
      </td>
    </tr>
    <tr>
      <td>
        R_02
      </td>
      <td>
        Errores en la administraci&oacute;n del GitHub
      </td>
      <td>
        Project Development
      </td>
      <td>
        Desde 5
      </td>
      <td>
        Al ser Github la plataforma en la que compartimos y organizamos nuestros avances, si existe alg&uacute;n error en la plataforma o si nosotros cometemos alg&uacute;n error, nuestro repositorio puede perder informaci&oacute;n o perderse por completo
      </td>
      <td>
        - Regresar a la versi&oacute;n m&aacute;s estable dentro del historial de versiones <br>
        - Utilizar la versi&oacute;n del dispositivo de alguien
      </td>
      <td>
      </td>
      <td>
        G501
      </td>
      <td>
        Baja
      </td>
      <td>
        Alto
      </td>
    </tr>
    <tr>
      <td>
        R_03
      </td>
      <td>
        Inclusi&oacute;n de nuevos miembros al equipo
      </td>
      <td>
        Project Development
      </td>
      <td>
        Desde 5
      </td>
      <td>
        Debido a la naturaleza del proyecto, de 4 equipos se formar&aacute; solo un equipo, por lo que la integraci&oacute;n de las ideas y los integrantes puede resultr retadora
      </td>
      <td>
        - Trabajar en c&eacute;lulas de trabajo compuestas de todos los aspectos del proyecto <br>
        - Utilizar las mejores ideas de cada equipo
      </td>
      <td>
      </td>
      <td>
        PM
      </td>
      <td>
        Media
      </td>
      <td>
        Medio
      </td>
    </tr>
    <tr>
      <td>
        R_04
      </td>
      <td>
        Divergencia entre los distintos ambientes de desarrollo
      </td>
      <td>
        Project Development
      </td>
      <td>
        Desde 6
      </td>
      <td>
        Ya que se utilizan diferentes librer&iacute;as y dependencias, si el sistema operativo del dispositivo de alg&uacute;n integrante no es compatible con dichos componentes, el desarrollo de la aplicaci&oacute;n puede retrasarse y la productividad y participaci&oacute;n del integrante puede verse afectada
      </td>
      <td>
        - Estandarizar un ambiente de desarrollo <br>
        - Creaci&oacute;n de un ambiente virtual (anaconda)
      </td>
      <td>
      </td>
      <td>
        G501
      </td>
      <td>
        Media
      </td>
      <td>
        Medio
      </td>
    </tr>
  </table>

  ## 3.3 Plan de comunicaciones y lista de equipos

  <table>
    <thead>
    <tr>
      <th>
        Rol
      </th>
      <th>
        Descripci&oacute;n
      </th>
    </tr>
    </thead>
    <tr>
      <td>
        Project Manager 
      </td>
      <td>
        El miembro que est&aacute; a cargo de un equipo. Deben organizar y planificar las tareas del equipo para que el proyecto tenga &eacute;xito, asegur&aacute;ndose de que se entreguen en tiempo, forma y retroalimentadas. 
      </td>
    </tr>
    <tr >
      <td>
        L&iacute;der de Pruebas
      </td>
      <td>
        Miembro del equipo que es responsable de participar y supervisar el desarrollo de las pruebas. Debe de tener en cuenta todos los alcances y criterios de validaci&oacute;n de cada prueba para asegurarse de que se cumplan en tiempo y forma. 
      </td>
    </tr>
    <tr >
      <td>
        L&iacute;der de Back-End
      </td>
      <td>
        Miembro del equipo que es responsable de participar y supervisar el desarrollo del back-end. Debe coordinar con todos los equipos de desarrollo el avance y los componentes del proyecto, asignar tareas, asegurarse de que se completen en tiempo y forma y coordinarse con el project manager.
      </td>
    </tr>
    <tr >
      <td>
        L&iacute;der de Front-End
      </td>
      <td>
        Miembro del equipo que es responsable de participar y supervisar el desarrollo del front-end. Debe coordinar con todos los equipos de desarrollo, el avance y los componentes del proyecto, asignar tareas, asegurarse de que se completen en tiempo y forma y coordinarse con el project manager.
      </td>
    </tr>
    <tr >
      <td>
        L&iacute;der de Base de Datos
      </td>
      <td>
        Miembro del equipo que es responsable de participar y supervisar el desarrollo de la base de datos. Debe coordinar con todos los equipos de desarrollo, el avance y los componentes del proyecto, asignar tareas, asegurarse de que se completen en tiempo y forma y coordinarse con el project manager.
      </td>
    </tr>
    <tr >
      <td>
        L&iacute;der de Seguridad
      </td>
      <td>
        Miembro del equipo que es responsable de participar y supervisar la protecci&oacute;n de los diferentes aspectos del proyecto y la autenticaci&oacute;n de los usuarios. Debe coordinar con todos los equipos de desarrollo, el avance y los componentes del proyecto, asignar tareas, asegurarse de que se completen en tiempo y forma y coordinarse con el project manager.
      </td>
    </tr>
    <tr >
      <td>
        Equipo de Desarrollo
      </td>
      <td>
        C&eacute;lula de trabajo encargada de requerimientos espec&iacute;ficos,compuesta de un miembro de back-end, uno de front-end, uno de base de datos, uno de seguridad, de pruebas y un project manager.
      </td>
    </tr>
  </table>

## Expectativas del Rol 
Es importante aclarar que dentro del proyecto presente, todos los involucrados en el desarrollo de la aplicación cumpliran un rol como tester a pesar de las responsabilidades que tengan en otro rol. Por lo antes mencionado, por cada componente que sea finalizado por cualquier persona en el equipo de desarrollo se realizará una prueba informal. De la misma manera, todo el equipo de desarrollo tiene como responsabilidad validar con el cliente los componentes de la aplicación y el entregable final.

La siguiente lista define en términos generales las expectativas relacionadas a los roles que están involucrados con el manejo, planeación o ejecución de la prueba para el proyecto.

## Project Manager 
Revisa el contenido del plan de pruebas, la estrategia de las pueblas, los estimados, criterios de validación con los equipos de trabajo, líderes y los stakeholders. Recopila la retroalimentación e informa a los demás. Tiene la responsabilidad de darle acompañamiento a las pruebas de caja blanca.

## Líder de Pruebas 
Junto con el project manager, crea y revisa el contenido del plan de pruebas, la estrategia de las pueblas, los estimados y criterios de validación coordinando la ejecución con las actividades programadas en el cronograma del proyecto. Recibe retroalimentación de los equipos de trabajo, líderes y los stakeholders, se asegura que las pruebas se ejecuten en tiempo y forma y documenta el proceso y los resultados.

## Líder de Back-End 
Junto con el líder de pruebas y el project manager, suma al contenido del plan de pruebas considerando las actividades programadas para el desarrollo del back-end, el avance del mismo y se asegura de la ejecución de las pruebas de sus componentes y que la integración con los otros equipos sea probada y documentada. Se le asignan pruebas, es parte y delega dichas pruebas y se asegura que las funcionalidades críticas de su desarrollo sean consideradas como parte del plan de pruebas. Tiene un seguimiento de las pruebas informales que sus desarrolladores han ejecutado. 

## Líder de Front-End 
Junto con el líder de pruebas y el project manager, suma al contenido del plan de pruebas considerando las actividades programadas para el desarrollo del front-end, el avance del mismo y se asegura de la ejecución de las pruebas de sus componentes y que la integración con los otros equipos sea probada y documentada. Se le asignan pruebas, es parte y delega dichas pruebas y se asegura que las funcionalidades críticas de su desarrollo sean consideradas como parte del plan de pruebas. Tiene un seguimiento de las pruebas informales que sus desarrolladores han ejecutado. 

## Líder de Base de Datos 
Junto con el líder de pruebas y el project manager, suma al contenido del plan de pruebas considerando las actividades programadas para el desarrollo de la base de datos, el avance de la misma y se asegura de la ejecución de las pruebas de sus componentes y que la integración con los otros equipos sea probada y documentada. Se le asignan pruebas, es parte y delega dichas pruebas y se asegura que las funcionalidades críticas de su desarrollo sean consideradas como parte del plan de pruebas. Tiene un seguimiento de las pruebas informales que sus desarrolladores han ejecutado. 

## Líder de Seguridad 
Junto con el líder de pruebas y el project manager, suma al contenido del plan de pruebas considerando las actividades programadas para la protección de los diferentes aspectos del proyecto y la autenticación de los usuarios, y se asegura de la ejecución de las pruebas de sus componentes y que la integración con los otros equipos sea probada y documentada. Se le asignan pruebas, es parte y delega dichas pruebas y se asegura que las funcionalidades críticas de su desarrollo sean consideradas como parte del plan de pruebas. Tiene un seguimiento de las pruebas informales que sus desarrolladores han ejecutado.

## Equipo de Desarrollo / Testers
Junto con sus respectivos líderes ejecutan las diferentes pruebas establecidas en el plan y se aseguran de que estas sean ejecutadas en el mismo ambiente siguiendo la metodología. Proveen y dan seguimiento a la retroalimentación y documentan el proceso y los resultados, así garantizando un proceso de QA transparente. Informan a los líderes si existe algún problema o si algún componente necesita ser corregido, se encargan de hacer las pruebas en tiempo y forma (de acuerdo al cronograma), llevan un seguimiento de sus pruebas informales y corrigen sus funcionalidades. Cada integrante del desarrollo tiene la responsabilidad de realizar sus pruebas asignadas de caja negra y junto con el SCRUM Master y el Project Manager realizar las pruebas de caja blanca. 

## Cronograma de Actividades
[Gantt](https://tec95061.monday.com/boards/4072044099/)

# 4. Ambiente de Pruebas

- El entorno de prueba consistirá en un entorno de Windows 11 como mínimo, un núcleo Intel i5 o equivalente; 8 GB de RAM.
- Se utilizarán los servicios de AWS, donde se busca alojar la aplicación web y la base de datos. 
- Todos los testers trabajaran en la misma versión de la aplicación y base de datos y tendrán las mismas versiones del software utilizado (incluyendo las librerías y dependencias).
- En caso de ser necesario se usará docker para poder ejecutar las pruebas y estandarizar el ambiente de trabajo.


# 5. Pruebas

# 6. Conclusiones
En conclusión, la aplicación de un plan de pruebas exhaustivo es esencial para el éxito del proyecto, sobre todo al tratarse de desarrollo de software. Esto ya que las pruebas continuas y sistematizadas  permiten identificar así como abordar posibles problemas emergentes antes de que se conviertan en riesgos  mayores. Con acceso al documento del plan de pruebas, los miembros del equipo tendrán una comprensión clara de los requisitos y expectativas del proyecto, que puede servir de guía para la toma de decisiones y la resolución de problemas.

El compromiso tanto del equipo de pruebas como de los desarrolladores, es crucial para la aplicación eficaz de este plan de pruebas. La adhesión a los contenidos acordados del documento garantiza que todos estén en la misma página y trabajen por el mismo objetivo, así facilitando un desarrollo fluido y el cumplimiento de los planes elaborados antes de la implantación.

Asimismo, el plan de pruebas puede ayudar al equipo a evaluar y mejorar el rendimiento general del proyecto. Mediante el seguimiento del progreso y la identificación de áreas de mejora, el equipo puede perfeccionar el plan del proyecto, optimizar los recursos y mejorar la eficiencia general del proyecto. En términos generales, la aplicación de un plan de pruebas exhaustivo es esencial para el éxito de cualquier proyecto. Con pruebas continuas, directrices claras y el compromiso de los miembros del equipo, el proyecto puede entregarse a tiempo, dentro del presupuesto y con la calidad esperada.
