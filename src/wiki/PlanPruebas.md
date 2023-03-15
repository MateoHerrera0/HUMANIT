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
1. Introducción

    a. Propósito

    b. Audiencia

2. Estrategia de Pruebas

    a. Descripción de las Pruebas
    
    b. Objetivos de las Pruebas

    c. Suposiciones de las Pruebas

    d. Objetos de Pruebas

    e. Alcance

    f. Niveles de las Pruebas

    g. Criterios de Validación

    h. Entregables de las Pruebas

    i. Lista de Hitos

    j. Estimado de Esfuerzo

3. Estrategia de Ejecución

    a. Criterios de Entrada y Salida

4. Proceso de Manejo de Pruebas

    a. Proceso de Ejecución de Pruebas

    b. Riesgos y Mitigación

    c. Plan de Comunicación y Roles del Equipo

    d. Expectativas de Roles

    i. Project Management

    ii. Líder de Pruebas

    ii. Líder de Back-End

    iii. Líder de Front-End

    iv. Líder de Base de Datos 

    iiv. Líder de Seguridad

    iiiv. Equipo de Desarrollo

    e. Cronograma de Actividades

5. Ambiente de Pruebas

6. Pruebas

7. Conclusiones

<html>

<head>
    <meta content="text/html; charset=UTF-8" http-equiv="content-type">
</head>

<body class="c106 doc-content">
    <p class="c80"><span class="c33"><a class="c14" href="#h.mx6gxsm2t7jg">1.
                Introducci&oacute;n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3</a></span></p>
    <p class="c13"><span class="c37"><a class="c14" href="#h.4jat4228tqo5">1.1.
                Prop&oacute;sito&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3</a></span></p>
    <p class="c13"><span class="c37"><a class="c14" href="#h.2w8d162qwulj">1.2.
                Audiencia&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3</a></span></p>
    <p class="c80"><span class="c33"><a class="c14" href="#h.kvw8q2v7aqxc">2. Estrategia de
                pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4</a></span></p>
    <p class="c13"><span class="c37"><a class="c14" href="#h.gbeixwb2ake5">2.1. Descripci&oacute;n de
                pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4</a></span></p>
    <p class="c13"><span class="c37"><a class="c14" href="#h.qpfdlx4dm8zo">2.2. Objetivo de las
                pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6</a></span></p>
    <p class="c13"><span class="c37"><a class="c14" href="#h.z6088tyel1xj">2.3. Suposiciones de las
                pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;7</a></span></p>
    <p class="c13"><span class="c37"><a class="c14" href="#h.ja9xqids1cyt">2.4. Objetivos de las
                pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;8</a></span></p>
    <p class="c13"><span class="c37"><a class="c14" href="#h.j8zy2j5g5i1t">2.5.
                Alcance&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;11</a></span></p>
    <p class="c13"><span class="c37"><a class="c14" href="#h.h904v6h0rrrr">2.6. Niveles de
                pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;18</a></span></p>
    <p class="c6"><span class="c37"><a class="c14" href="#h.bod9fnw9qu1w">Prueba
                Unitaria&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;18</a></span></p>
    <p class="c6"><span class="c37"><a class="c14" href="#h.91fzm9dtgvmr">Prueba de Caja
                Blanca&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;19</a></span></p>
    <p class="c6"><span class="c37"><a class="c14" href="#h.xhc6264rls1i">Prueba de
                Integraci&oacute;n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;19</a></span></p>
    <p class="c6"><span class="c37"><a class="c14" href="#h.j8epsprogp2p">Prueba de
                Validaci&oacute;n/Aceptaci&oacute;n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;20</a></span></p>
    <p class="c6"><span class="c25"><a class="c14" href="#h.qsyst13rz67j">Prueba de
                Sistema/Recorrido&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;20</a></span></p>
    <p class="c13"><span class="c37"><a class="c14" href="#h.cwh2skhwocng">2.7. Criterios de aceptaci&oacute;n de
                pruebas INFORMAL NO OLVIDAR&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;21</a></span></p>
    <p class="c6"><span class="c37"><a class="c14" href="#h.fsv2ynwal6n0">Pruebas Unitarias /
                Informales&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;21</a></span></p>
    <p class="c6"><span class="c37"><a class="c14" href="#h.kzej3b9e4wfe">Prueba de
                Integraci&oacute;n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;21</a></span></p>
    <p class="c6"><span class="c37"><a class="c14" href="#h.ns3vrtfyjguc">Prueba de
                Validaci&oacute;n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;21</a></span></p>
    <p class="c6"><span class="c37"><a class="c14" href="#h.7krppuwc58yf">Prueba de
                Sistema&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;22</a></span></p>
    <p class="c13"><span class="c37"><a class="c14" href="#h.s6ntvdjxs5wr">2.8. Entregables de
                pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;22</a></span></p>
    <p class="c13"><span class="c37"><a class="c14" href="#h.vqt91vksszs0">2.9. Lista de
                hitos&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;23</a></span></p>
    <p class="c13"><span class="c37"><a class="c14" href="#h.tttcgn6nmo2n">2.10. Estimaci&oacute;n de esfuerzo de las
                pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;27</a></span></p>
    <p class="c80"><span class="c33"><a class="c14" href="#h.3b7gmogqu7x8">3. Estrategia de
                ejecuci&oacute;n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;28</a></span></p>
    <p class="c13"><span class="c37"><a class="c14" href="#h.g57zhm96h5z0">3.1. Criterios de Entrada y
                Salida&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;28</a></span></p>
    <p class="c80"><span class="c33"><a class="c14" href="#h.rggsbldjdzgj">4. Proceso de gesti&oacute;n de
                pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;30</a></span></p>
    <p class="c13"><span class="c37"><a class="c14" href="#h.l5voq2cnpp4q">4.1. Proceso de ejecuci&oacute;n de
                pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;30</a></span></p>
    <p class="c13"><span class="c37"><a class="c14" href="#h.nsa8lxrnmxkd">4.2. Riesgos de prueba y factores de
                mitigaci&oacute;n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;31</a></span></p>
    <p class="c13"><span class="c37"><a class="c14" href="#h.5h8w5mqda6gh">4.3. Plan de comunicaciones y lista de
                equipos&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;32</a></span></p>
    <p class="c6"><span class="c37"><a class="c14" href="#h.shiwdz2v0drx">Expectativas del
                Rol&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;34</a></span></p>
    <p class="c6"><span class="c37"><a class="c14" href="#h.vajm4pu401qs">Project
                Manager&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;34</a></span></p>
    <p class="c6"><span class="c37"><a class="c14" href="#h.cup1cc33x1cr">L&iacute;der de
                Pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;34</a></span></p>
    <p class="c6"><span class="c37"><a class="c14" href="#h.15iz1ry18o">L&iacute;der de
                Back-End&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;34</a></span></p>
    <p class="c6"><span class="c37"><a class="c14" href="#h.bpgnszel0u1j">Cronograma de
                Actividades&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;36</a></span></p>
    <p class="c80"><span class="c33"><a class="c14" href="#h.6ngo7ertvrlx">5. Ambiente de
                pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;36</a></span></p>
    <p class="c80"><span class="c33"><a class="c14" href="#h.e0bh1ws8hyem">6.
                Pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;36</a></span></p>
    <p class="c80"><span class="c33"><a class="c14" href="#h.j9dbb7pex1fz">7.
                Conclusiones&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;37</a></span></p>
    <p class="c4 c12"><span class="c17"></span></p>
    <p class="c4 c12 c83"><span class="c17"></span></p>
    <p class="c4 c12"><span class="c1"></span></p>
    <ol class="c0 lst-kix_d3i63clc3lgg-0 start" start="1">
        <li class="c4 c7 c79 li-bullet-0">
            <h1 id="h.mx6gxsm2t7jg" style="display:inline"><span class="c39">Introducci&oacute;n</span></h1>
        </li>
    </ol>
    <ol class="c0 lst-kix_d3i63clc3lgg-1 start" start="1">
        <li class="c4 c15 c46 li-bullet-0">
            <h2 id="h.4jat4228tqo5" style="display:inline"><span class="c35">Prop&oacute;sito</span></h2>
        </li>
    </ol>
    <p class="c4 c108"><span class="c1">El documento presente tiene el objetivo de describir el programa de pruebas que
            se realizar&aacute; durante el desarrollo del proyecto con NDS; una plataforma para la venta de
            autom&oacute;viles en l&iacute;nea. En particular, este documento contendr&aacute;:</span></p>
    <ol class="c0 lst-kix_xdqyscxb1zsk-0 start" start="1">
        <li class="c4 c42 li-bullet-0"><span class="c1">La estrategia y objetivos de las pruebas a realizarse en cada
                uno de los componentes de la aplicaci&oacute;n.</span></li>
        <li class="c4 c42 li-bullet-0"><span class="c1">Una justificaci&oacute;n acerca de las pruebas
                seleccionadas.</span></li>
        <li class="c4 c42 li-bullet-0"><span class="c1">Los criterios de validaci&oacute;n para los componentes de la
                aplicaci&oacute;n y los criterios de aceptaci&oacute;n de cada una de las pruebas.</span></li>
        <li class="c4 c42 li-bullet-0"><span class="c1">El plan de ejecuci&oacute;n de las pruebas a realizarse, al
                igual que el plan de remediaci&oacute;n &nbsp;en caso de que una de estas pruebas termine con un
                resultado negativo.</span></li>
        <li class="c4 c42 li-bullet-0"><span class="c1">Las responsabilidades de los integrantes del equipo en
                relaci&oacute;n a las pruebas.</span></li>
        <li class="c4 c42 li-bullet-0"><span class="c1">Una descripci&oacute;n del ambiente, al igual que las
                herramientas &nbsp;herramientas que ser&aacute;n utilizadas para las pruebas.</span></li>
    </ol>
    <p class="c4 c12 c97"><span class="c1"></span></p>
    <ol class="c0 lst-kix_d3i63clc3lgg-1" start="2">
        <li class="c4 c15 c46 li-bullet-0">
            <h2 id="h.2w8d162qwulj" style="display:inline"><span class="c117">Audiencia</span><span
                    class="c100">&nbsp;</span><sup><a href="#cmnt1" id="cmnt_ref1">[a]</a></sup></h2>
        </li>
    </ol>
    <p class="c4 c36 c69"><span class="c1">En esta secci&oacute;n se encuentra la descripci&oacute;n detallada de la
            audiencia a la que se dirige el presente escrito:</span></p>
    <ol class="c0 lst-kix_notb3jec8k49-0 start" start="1">
        <li class="c3 li-bullet-0"><span class="c1">El siguiente documento est&aacute; dise&ntilde;ado para ser
                consultado principalmente por los miembros del equipo de desarrollo del proyecto, profesores
                responsables del mismo, el cliente (NDS) y sus representantes.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">&nbsp;El director del proyecto es responsable de utilizar el
                documento para garantizar que se sigue el calendario de pruebas acordado y que se supervisa el progreso
                de acuerdo con las instrucciones del documento. Asimismo, esta figura es responsable de los resultados y
                el rendimiento de cada prueba.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">El cliente (NDS), las partes interesadas o sus representantes tienen
                la opci&oacute;n de revisar el documento para verificar que el desarrollo se ajusta a sus requisitos e
                intereses.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">El equipo de desarrollo se encarga de garantizar que el plan de
                pruebas y los resultados especificados en el documento son coherentes con lo acordado durante la fase de
                dise&ntilde;o.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">&nbsp;El equipo de desarrollo es responsable de resolver cualquier
                prueba fallida se&ntilde;alada en el documento.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Otros miembros del equipo y las partes interesadas tambi&eacute;n
                pueden utilizar el documento como punto de referencia en todo momento para diversos asuntos relacionados
                con el proyecto.</span></li>
    </ol>
    <p class="c4 c36 c56 c12"><span class="c1"></span></p>
    <ol class="c0 lst-kix_d3i63clc3lgg-0" start="2">
        <li class="c4 c38 li-bullet-0">
            <h1 id="h.kvw8q2v7aqxc" style="display:inline"><span class="c39">Estrategia de pruebas </span></h1>
        </li>
    </ol>
    <ol class="c0 lst-kix_d3i63clc3lgg-1 start" start="1">
        <li class="c4 c15 c46 li-bullet-0">
            <h2 id="h.gbeixwb2ake5" style="display:inline"><span>Descripci&oacute;n de pruebas</span></h2>
        </li>
    </ol>
    <p class="c4 c118"><span class="c1">En el presente apartado se describe a profundidad la estrategia de pruebas que
            se seguir&aacute; durante el proceso de desarrollo de la plataforma web para el cliente NDS.</span></p>
    <p class="c4 c12 c118"><span class="c1"></span></p>
    <p class="c30"><span class="c52">Etapa 1 &ndash; Comprensi&oacute;n de los Requerimientos, Especificaciones del
            Proyecto y Pruebas Est&aacute;ticas:</span><span class="c1">&nbsp;Antes de crear una estrategia de pruebas,
            primero se comprenden y establecen de manera detallada los requerimientos del proyecto. Para ello se tiene
            una serie de interacciones semanales con el cliente NDS en el cual se documentan de forma clara las
            caracter&iacute;sticas de la soluci&oacute;n que cumplen con sus necesidades y objetivos. Al finalizar esta
            etapa se espera que haya pocos o nulos cambios, ya que el resto del proyecto se desarrollar&aacute; en base
            a lo establecido en esta etapa, por lo cu&aacute;l queda fuera de las etapas de iteraci&oacute;n. </span>
    </p>
    <p class="c30 c12"><span class="c17"></span></p>
    <p class="c30"><span class="c52">Etapa 2 - Pruebas </span><span class="c52">Informales</span><span class="c52">:
        </span><span class="c1">En un principio, se comenzar&aacute; realizando pruebas informales durante el desarrollo
            del software. Esto incluir&iacute;a pruebas realizadas individualmente por cada uno de los desarrolladores
            sin supervisi&oacute;n, teniendo un enfoque en comprobar la funcionalidad de componentes creados. En esta
            etapa comienza el proceso iterativo de las pruebas y va dentro de las pruebas din&aacute;micas. </span></p>
    <p class="c30 c12"><span class="c17"></span></p>
    <p class="c30"><span class="c52">Etapa 3 &ndash; Realizaci&oacute;n de Pruebas Unitarias:</span><span
            class="c1">&nbsp;Esta etapa tambi&eacute;n va dentro de las pruebas din&aacute;micas y se pretende comenzar
            realizando las pruebas unitarias para cada componente de software de la plataforma. Esto
            concentr&aacute;ndose en pruebas de caja negra (black box tests) tomando especial atenci&oacute;n en la
            entrada y salida esperadas en su correcto funcionamiento. Simult&aacute;neamente a esto, se acordar&aacute;
            de manera iterativa con NDS las pruebas de historias de usuario van de acuerdo a sus criterios de
            aceptaci&oacute;n. Esto ayudar&aacute; a garantizar que la p&aacute;gina web satisfaga correctamente las
            necesidades de NDS y de sus clientes.</span></p>
    <p class="c30 c12"><span class="c1"></span></p>
    <p class="c30"><span class="c52">Etapa 4 </span><sup><a href="#cmnt2" id="cmnt_ref2">[b]</a></sup><sup><a
                href="#cmnt3" id="cmnt_ref3">[c]</a></sup><span class="c52">- Pruebas de Caja Blanca de cobertura (White
            Box Testing):</span><span class="c1">&nbsp;En esta etapa, que tambi&eacute;n va dentro de las
            din&aacute;micas, se realizan las pruebas de caja blanca a los componentes definidos en este documento,
            especialmente dando prioridad a aquellos componentes que generaron errores en las pruebas de caja negra. De
            esta manera, se podr&aacute; analizar el c&oacute;digo de dichos componentes, as&iacute; permitiendo
            arreglar errores persistentes en pruebas anteriores o eliminar redundancias. </span></p>
    <p class="c30"><span class="c1">Para hacer m&aacute;s eficaz nuestro proceso de pruebas de caja blanca, usaremos la
            t&eacute;cnica de cobertura en donde se probaran los caminos m&aacute;s utilizados para hacer uso de cada
            funci&oacute;n de cada tipo de usuario. </span></p>
    <p class="c12 c30"><span class="c1"></span></p>
    <p class="c30"><span class="c52">Etapa 5 - Pruebas de Integraci&oacute;n:</span><span class="c1">&nbsp;En esta
            etapa, que es la &uacute;ltima dentro de las etapas din&aacute;micas, despu&eacute;s de que todas las
            pruebas unitarias hayan pasado con &eacute;xito se pasan a las pruebas de integraci&oacute;n donde de manera
            ascendente se van uniendo los diferentes componentes para validar su correcto funcionamiento en conjunto.
            Las pruebas de integraci&oacute;n se llevar&aacute;n a cabo mediante pruebas de caja negra de casos de uso
            aleatorias, las cuales ser&aacute;n elegidas y supervisadas por el Project Manager responsable del equipo de
            desarrollo.</span></p>
    <p class="c30 c12"><span class="c17"></span></p>
    <p class="c30 c12"><span class="c17"></span></p>
    <p class="c30"><span class="c52">Etapa 6 &ndash; Pruebas de Validaci&oacute;n/Aceptaci&oacute;n:</span><span
            class="c1">&nbsp;En esta etapa, se requiere que haya pocos o ning&uacute;n cambio, ya qu&eacute;,
            despu&eacute;s de que las pruebas de integraci&oacute;n hayan sido exitosas se realizan las pruebas de
            validaci&oacute;n en las que se revisar&aacute; con el cliente NDS que los criterios de validaci&oacute;n
            definidos en etapas anteriores se cumplen hasta el momento del proceso de pruebas.</span></p>
    <p class="c30 c12"><span class="c1"></span></p>
    <p class="c30"><span class="c52">Etapa 7 &ndash; Pruebas de </span><span class="c52">Est&aacute;tica de
            Recorridos</span><span class="c52">: </span><span class="c1">Una vez que se haya tenido la aprobaci&oacute;n
            de NDS se realizar&aacute; la prueba del funcionamiento del sistema como un todo, verificando el
            comportamiento y correcto funcionamiento de toda la plataforma en el nivel m&aacute;s alto posible.</span>
    </p>
    <p class="c30 c12"><span class="c1"></span></p>
    <p class="c30"><span class="c52">Etapa 8 - Manual de Usuario:</span><span class="c52">&nbsp;</span><span
            class="c5">En esta etapa final, una vez que se haya completado las etapas anteriores y son pocos o nulos los
            cambios se crea el manual de usuario en el que se le proveer&aacute; informaci&oacute;n e instrucciones al
            usuario de c&oacute;mo usar el software desarrollado. En el manual de usuario se incluir&aacute;n los
            caminos previamente establecidos en las pruebas de caja blanca de cobertura. </span></p>
    <p class="c30 c12"><span class="c17 c50"></span></p>
    <p class="c30"><span class="c52">1,6,7 -&gt; poquitos o nulos cambios</span><sup><a href="#cmnt4"
                id="cmnt_ref4">[d]</a></sup></p>
    <p class="c30"><span class="c1">Es relevante mencionar, que en esta estrategia se mantiene un flujo iterativo, donde
            de ser necesario se actualizar&aacute; el documento de pruebas o se podr&aacute; regresar a etapas de
            pruebas anteriores para as&iacute; solucionar cualquier fallo o error en cualquier nivel de la
            plataforma.</span></p>
    <p class="c4 c12 c111"><span class="c1"></span></p>
    <ol class="c0 lst-kix_d3i63clc3lgg-1" start="2">
        <li class="c4 c15 c46 li-bullet-0">
            <h2 id="h.qpfdlx4dm8zo" style="display:inline"><span>Objetivo de las pruebas</span></h2>
        </li>
    </ol>
    <p class="c4 c70 c110"><span class="c5">El objetivo de las pruebas que se realizar&aacute;n durante el transcurso
            del proyecto es la validaci&oacute;n de las funcionalidades fundamentales de la aplicaci&oacute;n, al igual
            que comprobar la correcta implementaci&oacute;n de los requerimientos establecidos en el documento
        </span><span class="c5 c50">SRS (LINK)</span><span class="c1">. En consideraci&oacute;n de este objetivo, las
            pruebas a realizarse comprender&aacute;n:</span></p>
    <ul class="c0 lst-kix_1ymfzvnh8b2w-0 start">
        <li class="c4 c42 c70 li-bullet-0"><span class="c1">Pruebas que aseguren la correcta autorizaci&oacute;n de
                usuarios, al igual que la asignaci&oacute;n de los premios asociados.</span></li>
        <li class="c4 c42 c70 li-bullet-0"><span class="c1">Pruebas que comprueben el correcto funcionamiento en la
                b&uacute;squeda y filtrado del cat&aacute;logo de autos.</span></li>
        <li class="c4 c42 c70 li-bullet-0"><span class="c1">Pruebas que comprueben el correcto funcionamiento del
                guardado de autom&oacute;viles en la base de datos.</span></li>
        <li class="c4 c42 c70 li-bullet-0"><span class="c1">Pruebas que garanticen el funcionamiento de la
                recopilaci&oacute;n, an&aacute;lisis, y generaci&oacute;n de estad&iacute;stica relacionada con usuarios
                agentes de la aplicaci&oacute;n.</span></li>
        <li class="c4 c42 c70 li-bullet-0"><span class="c1">Pruebas relacionadas al servicio de chat implementado en la
                aplicaci&oacute;n.</span></li>
        <li class="c4 c42 c70 li-bullet-0"><span class="c1">Pruebas con el objetivo de comprobar el correcto
                funcionamiento del proceso de compra de un autom&oacute;vil.</span></li>
        <li class="c4 c42 c70 li-bullet-0"><span class="c1">Pruebas asociadas a la creaci&oacute;n de usuarios con
                diferentes permisos. </span></li>
        <li class="c4 c42 c70 li-bullet-0"><span class="c5">Pruebas asociadas al funcionamiento de un software estable y
                listo para producci&oacute;n.</span></li>
    </ul>
    <ol class="c0 lst-kix_d3i63clc3lgg-1 start" start="1">
        <li class="c4 c15 c46 li-bullet-0">
            <h2 id="h.z6088tyel1xj" style="display:inline"><span>Suposiciones de las pruebas</span></h2>
        </li>
    </ol>
    <p class="c4 c56"><span class="c52">Suposiciones clave</span></p>
    <ol class="c0 lst-kix_2ppqn3k0um83-0 start" start="1">
        <li class="c4 c42 c74 li-bullet-0"><span class="c5">Se dar&aacute; prioridad a las pruebas funcionales debido a
                limitantes de tiempo y presupuesto</span><span class="c1">. </span></li>
        <li class="c4 c42 c63 li-bullet-0"><span class="c5">Todas las pruebas se har&aacute;n en el mismo
                ambiente.</span></li>
        <li class="c4 c42 li-bullet-0"><span class="c5">Todas las pruebas se har&aacute;n inicialmente con pruebas
                Informales y posteriormente en Caja Negra.</span></li>
    </ol>
    <p class="c4 c56"><span class="c52">Suposiciones g</span><span class="c17">eneral</span><span class="c52">es</span>
    </p>
    <ol class="c0 lst-kix_vmd3n8uqgg1o-0 start" start="1">
        <li class="c4 c42 li-bullet-0"><span class="c5">Las pruebas funcionales ser&aacute;n las m&aacute;s relevantes
                del plan de pruebas.</span></li>
        <li class="c4 c42 li-bullet-0"><span class="c1">Realizar las mismas pruebas conlleva a los mismos
                resultados.</span></li>
        <li class="c4 c42 li-bullet-0"><span class="c1">Las pruebas con variedad en el rol de acceso no son
                equivalentes, y debe definirse una prueba por cada rol</span></li>
        <li class="c4 c42 c112 li-bullet-0"><span class="c5">Si el ambiente de pruebas deja de estar disponible; el
                equipo de pruebas crear&aacute; uno lo m&aacute;s similar lo antes posible.</span></li>
        <li class="c4 c42 li-bullet-0"><span class="c5">Todas las funciones han sido probadas meticulosamente.</span>
        </li>
        <li class="c4 c24 li-bullet-0"><span class="c5">Las pruebas de caja blanca y pruebas paso a paso solo se
                ejecutar&aacute;n si los resultados son distintos a lo esperado</span><span class="c1">.</span></li>
        <li class="c4 c42 c63 li-bullet-0"><span class="c5">El equipo de pruebas documentar&aacute; sus resultados de
                acuerdo a lo evaluado.</span></li>
        <li class="c4 c42 c121 li-bullet-0"><span class="c1">El equipo de pruebas asume que tod</span><span
                class="c5">as las entradas o inputs requeridos durante el dise&ntilde;o y la ejecuci&oacute;n de las
                pruebas estar&aacute;n apoyados por el desarrollador/analista </span><span
                class="c5">respectivamente</span><span class="c5">. </span></li>
        <li class="c4 c42 li-bullet-0"><span class="c5">Todos los documentos personales del usuario ser&aacute;n
                guardados con el mismo formato y nomenclatura.</span></li>
        <li class="c4 c24 li-bullet-0"><span class="c5">El PM verificar&aacute; los resultados de todas las pruebas
                efectuadas.</span></li>
        <li class="c4 c24 li-bullet-0"><span class="c5">El PM aprueba todos los casos de prueba propuestos previo a la
                ejecuci&oacute;n de los mismos</span></li>
        <li class="c4 c24 li-bullet-0"><span class="c1">El equipo de pruebas </span><span
                class="c5">manejar&aacute;</span><span class="c1">&nbsp;todo el esfuerzo de </span><span
                class="c5">ejecuci&oacute;n</span><span class="c1">&nbsp;de prueba </span><span class="c1">de forma
                coordinada con el PM.</span></li>
        <li class="c4 c42 c86 li-bullet-0"><span class="c1">El recorrido y manual de usuario se realizar&aacute; en los
                &uacute;ltimos sprints.</span></li>
    </ol>
    <p class="c4 c86 c12 c101"><span class="c1"></span></p>
    <ol class="c0 lst-kix_d3i63clc3lgg-1" start="2">
        <li class="c4 c15 c46 li-bullet-0">
            <h2 id="h.ja9xqids1cyt" style="display:inline"><span>Objetivos de las pruebas</span></h2>
        </li>
    </ol>
    <p class="c4 c36 c56"><span class="c55 c5">Flujo del Cliente:</span></p>
    <ol class="c0 lst-kix_732m4c7tqfpy-0 start" start="1">
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de Login.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de b&uacute;squeda de
                cat&aacute;logo.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de filtrado de cat&aacute;logo.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad del agendado &nbsp;de la prueba de
                manejo.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de la subida de documentos para la solicitud
                de prueba de manejo.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de la subida de documentos para la compra de
                un auto.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de la transacci&oacute;n del pago para la
                prueba de manejo.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de la transacci&oacute;n de la compra de
                auto</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad del seguimiento de acciones del usuario
                (prueba de manejo o compras).</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad del sistema de Chat.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad del sistema de favoritos (wishlist).</span>
        </li>
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de la edici&oacute;n de datos en el
                perfil.</span></li>
    </ol>
    <p class="c4 c36 c56 c12"><span class="c1"></span></p>
    <p class="c4 c36 c56"><span class="c5 c55">Flujo del Super Administrador:</span></p>
    <ol class="c0 lst-kix_2f59h085xe11-0 start" start="1">
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de Login.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de b&uacute;squeda de usuarios.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar las funcionalidad de filtrado de usuarios.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de la modificaci&oacute;n de datos de un
                grupo automotriz.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de la b&uacute;squeda de solicitudes.</span>
        </li>
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad del filtrado de solicitudes.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar funcionalidad de la aprobaci&oacute;n/negaci&oacute;n de una
                solicitud.</span></li>
        <li class="c42 c36 c75 li-bullet-0"><span class="c1">Probar la funcionalidad del registro de un grupo
                automotriz.</span></li>
        <li class="c75 c42 c36 li-bullet-0"><span class="c1">Probar la funcionalidad del dashboard estad&iacute;stico.
            </span></li>
    </ol>
    <p class="c4 c36 c56"><span class="c55 c5">Flujo del Grupo Automotriz:</span></p>
    <p class="c4 c36 c73"><span class="c1">Etapa 1:</span></p>
    <ol class="c0 lst-kix_iqtl5xa2cmxc-0 start" start="1">
        <li class="c2 li-bullet-0"><span class="c1">Probar funcionalidad del Login.</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Probar funcionalidad para realizar una aplicaci&oacute;n.</span>
        </li>
        <li class="c2 li-bullet-0"><span class="c1">Probar funcionalidad del panel de seguimiento a una
                aplicaci&oacute;n.</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Probar funcionalidad de la modificaci&oacute;n de los datos del
                perfil.</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Probar funcionalidad de la eliminaci&oacute;n de una cuenta.</span>
        </li>
    </ol>
    <p class="c4 c36 c85 c56"><span class="c1">Etapa 2:</span></p>
    <ol class="c0 lst-kix_9sstyjjxvcqu-0 start" start="1">
        <li class="c2 li-bullet-0"><span class="c1">Probar funcionalidad de Login.</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Probar funcionalidad del registro de una agencia.</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Probar funcionalidad de la b&uacute;squeda de usuarios.</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Probar funcionalidad del filtrado de usuarios.</span></li>
        <li class="c2 li-bullet-0"><span class="c1">&nbsp;Probar funcionalidad para la modificaci&oacute;n de datos de
                una agencia.</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Probar funcionalidad del dashboard estad&iacute;stico.</span></li>
    </ol>
    <p class="c4 c36 c12"><span class="c1"></span></p>
    <p class="c4 c36 c56"><span class="c55 c5">Flujo de la Agencia:</span></p>
    <ol class="c0 lst-kix_7h0jbu1x222k-0 start" start="1">
        <li class="c3 li-bullet-0"><span class="c1">Probar funcionalidad de Login.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar funcionalidad de la b&uacute;squeda de usuarios.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar funcionalidad del filtrado de usuarios.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar funcionalidad del registro de un gerente.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar funcionalidad para la modificaci&oacute;n de datos de un
                gerente.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar funcionalidad para la
                actualizaci&oacute;n/modificaci&oacute;n del cat&aacute;logo de autos.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar funcionalidad del dashboard estad&iacute;stico.</span></li>
    </ol>
    <p class="c4 c36 c12 c73"><span class="c1"></span></p>
    <p class="c4 c36 c56"><span class="c55 c5">Flujo del Gerente:</span></p>
    <ol class="c0 lst-kix_7hnw7pp31c96-0 start" start="1">
        <li class="c3 li-bullet-0"><span class="c1">Probar funcionalidad de Login.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar funcionalidad de la b&uacute;squeda de usuarios.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar funcionalidad del filtrado de usuarios.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar funcionalidad del registro de un vendedor.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar funcionalidad para la modificaci&oacute;n de datos de un
                vendedor.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar funcionalidad para la
                actualizaci&oacute;n/modificaci&oacute;n del cat&aacute;logo de autos.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar funcionalidad del dashboard estad&iacute;stico.</span></li>
    </ol>
    <p class="c4 c36 c12"><span class="c55 c5"></span></p>
    <p class="c4 c36 c12"><span class="c55 c5"></span></p>
    <p class="c4 c36 c56"><span class="c55 c5">Flujo del Vendedor:</span></p>
    <ol class="c0 lst-kix_mg52369i75sn-0 start" start="1">
        <li class="c3 li-bullet-0"><span class="c1">Probar funcionalidad del Login.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de b&uacute;squeda de
                cat&aacute;logo.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de filtrado de cat&aacute;logo.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de la b&uacute;squeda de solicitudes.</span>
        </li>
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad del filtrado de solicitudes.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar funcionalidad del manejo de una solicitud.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar funcionalidad del sistema de chat.</span></li>
        <li class="c3 li-bullet-0"><span class="c1">Probar funcionalidad del dashboard estad&iacute;stico.</span></li>
    </ol>
    <h2 class="c4 c20" id="h.1cjsyuq850k3"><span class="c52 c82"></span></h2>
    <ol class="c0 lst-kix_d3i63clc3lgg-1" start="3">
        <li class="c4 c15 c46 li-bullet-0">
            <h2 id="h.j8zy2j5g5i1t" style="display:inline"><span>Alcance</span></h2>
        </li>
    </ol>
    <p class="c4 c36 c56"><span class="c55 c5">Flujo del Cliente:</span></p>
    <ol class="c0 lst-kix_rg52xa75v2qv-0 start" start="1">
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de Login.</span></li>
    </ol>
    <ul class="c0 lst-kix_34xw20osf7pl-0 start">
        <li class="c2 li-bullet-0"><span class="c1">Acceso v&aacute;lido con Credenciales correctas de
                super-administrador.</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Acceso no autorizado con correo invalido/cuenta inexistente.</span>
        </li>
        <li class="c2 li-bullet-0"><span class="c1">Acceso no autorizado con contrase&ntilde;a incorrecta.</span></li>
    </ul>
    <ol class="c0 lst-kix_rg52xa75v2qv-0" start="2">
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de b&uacute;squeda de
                cat&aacute;logo.</span></li>
    </ol>
    <ul class="c0 lst-kix_pzlvm0ag2zpq-0 start">
        <li class="c2 li-bullet-0"><span class="c1">Se hace una b&uacute;squeda de un auto dentro del
                cat&aacute;logo</span></li>
        <li class="c2 li-bullet-0"><span class="c1">El sistema muestra los resultados de los autos segun la
                b&uacute;squeda</span></li>
    </ul>
    <ol class="c0 lst-kix_rg52xa75v2qv-0" start="3">
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de filtrado de cat&aacute;logo.</span></li>
    </ol>
    <ul class="c0 lst-kix_kszrschy9h6a-0 start">
        <li class="c2 li-bullet-0"><span class="c1">Dentro de la b&uacute;squeda de un auto del cat&aacute;logo se
                muestran los filtros disponibles para la b&uacute;squeda</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Se seleccionan los filtros deseados</span></li>
        <li class="c2 li-bullet-0"><span class="c1">El sistema muestra los resultados de los autos seg&uacute;n los
                filtros aplicados</span></li>
    </ul>
    <ol class="c0 lst-kix_rg52xa75v2qv-0" start="4">
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad del agendado de la prueba de manejo.</span>
        </li>
    </ol>
    <ul class="c0 lst-kix_d2dmeguqo78-0 start">
        <li class="c2 li-bullet-0"><span class="c1">El usuario cliente selecciona el auto de su preferencia para
                solicitar una prueba de manejo</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Para poder solicitar la prueba es necesario que llene un formulario
                y suba los documentos necesarios</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Una vez completado lo anterior su solicitud se confirma y
                autom&aacute;ticamente se le asigna un usuario vendedor que le dar&aacute; seguimiento a su
                solicitud</span></li>
        <li class="c2 li-bullet-0"><span class="c1">El usuario vendedor se pone en contacto con el cliente a
                trav&eacute;s del chat de la plataforma, en caso de que tenga dudas, adem&aacute;s puede ver el estatus
                de su solicitud en un apartado donde se listaran las solicitudes del cliente</span></li>
        <li class="c2 li-bullet-0"><span class="c1">El vendedor revisa los documentos de la solicitud, si est&aacute;n
                correctos se aprueban, de lo contrario el vendedor le tiene que notificar al cliente para que pueda
                volver a subir sus documentos correctamente</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Una vez que los documentos son aprobados por el vendedor, en caso de
                que el auto seleccionado se requiera pagar una cuota para la prueba de manejo, se hace la
                transacci&oacute;n necesaria </span></li>
        <li class="c2 li-bullet-0"><span class="c5">Una vez completada la transacci&oacute;n el cliente agenda
            </span><span class="c5">su prueba</span><span class="c1">&nbsp;de manejo</span></li>
    </ul>
    <ol class="c0 lst-kix_rg52xa75v2qv-0" start="5">
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de la subida de documentos para la solicitud
                de prueba de manejo.</span></li>
    </ol>
    <ul class="c0 lst-kix_piws44cnashc-0 start">
        <li class="c2 li-bullet-0"><span class="c1">El usuario cliente selecciona el auto de su preferencia para
                solicitar una prueba de manejo</span></li>
        <li class="c2 li-bullet-0"><span class="c1">El cliente llena el formulario con los datos necesarios y sube los
                documentos que se le piden</span></li>
        <li class="c2 li-bullet-0"><span class="c1">El vendedor revisa los documentos de la solicitud, si est&aacute;n
                correctos se aprueban, de lo contrario el vendedor le tiene que notificar al cliente para que pueda
                volver a subir sus documentos correctamente</span></li>
    </ul>
    <ol class="c0 lst-kix_rg52xa75v2qv-0" start="6">
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de la subida de documentos para la compra de
                un auto.</span></li>
    </ol>
    <ul class="c0 lst-kix_8phg914ssidx-0 start">
        <li class="c2 li-bullet-0"><span class="c1">El usuario cliente selecciona un veh&iacute;culo y solicita
                comprarlo</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Para poder solicitar la comprar es necesario que llene un formulario
                y suba los documentos necesarios</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Despu&eacute;s de subirlos se le asignar&aacute; un vendedor quien
                revisar&aacute; sus documentos y le dar&aacute; seguimiento a su compra</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Una vez que complete esto el cliente puede ver el estatus de su
                solicitud en un apartado donde se listaran sus solicitudes</span></li>
        <li class="c2 li-bullet-0"><span class="c1">El vendedor al revisar los documentos si est&aacute;n correctos los
                aprueba y puede continuar con el proceso de compra, de lo contrario le tiene que notificar al usuario
                para que los vuelva a subir</span></li>
    </ul>
    <ol class="c0 lst-kix_rg52xa75v2qv-0" start="7">
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de la transacci&oacute;n del pago para la
                prueba de manejo.</span></li>
    </ol>
    <ul class="c0 lst-kix_rzviu7jw11bm-0 start">
        <li class="c2 li-bullet-0"><span class="c1">Una vez que los documentos de la prueba de manejo fueron aprobados,
                si el veh&iacute;culo necesita una cuota para realizar la prueba se le notifica al cliente</span></li>
        <li class="c2 li-bullet-0"><span class="c1">El cliente revisa el seguimiento de su solicitud y hace el
                pago</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Una vez que termina el pago el sistema le confirma de recibido el
                pago y se actualiza el seguimiento</span></li>
    </ul>
    <ol class="c0 lst-kix_rg52xa75v2qv-0" start="8">
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de la transacci&oacute;n de la compra de
                auto</span></li>
    </ol>
    <ul class="c0 lst-kix_xnlyfuqgi6j3-0 start">
        <li class="c2 li-bullet-0"><span class="c1">Una vez que los documentos de la compra fueron aprobados, se le
                notifica al cliente para pueda realizar el pago del veh&iacute;culo</span></li>
        <li class="c2 li-bullet-0"><span class="c1">El cliente revisa el seguimiento de su solicitud y hace el
                pago</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Una vez que termina el pago el sistema le confirma de recibido el
                pago y se actualiza el seguimiento</span></li>
    </ul>
    <ol class="c0 lst-kix_rg52xa75v2qv-0" start="9">
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad del seguimiento de acciones del usuario
                (prueba de manejo o compras).</span></li>
    </ol>
    <ul class="c0 lst-kix_zfbk09w23seu-0 start">
        <li class="c2 li-bullet-0"><span class="c1">Una vez que el cliente sube los documentos necesarios ya sea para la
                prueba de manejo o para la compra de un auto puede realizar el seguimiento de su solicitud</span></li>
        <li class="c2 li-bullet-0"><span class="c1">En el apartado indicado de seguimiento, puede ver en qu&eacute; fase
                va su solicitud</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Mientras el vendedor asignado a su solicitud la revisa y mientras va
                avanzando el proceso el vendedor va actualizando la etapa en la que se encuentra el cliente</span></li>
    </ul>
    <ol class="c0 lst-kix_rg52xa75v2qv-0" start="10">
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad del sistema de Chat.</span></li>
    </ol>
    <ul class="c0 lst-kix_6bgajs6h3l6j-0 start">
        <li class="c2 li-bullet-0"><span class="c1">Entrada a la vista de chats y contactos con acceso de cliente</span>
        </li>
        <li class="c2 li-bullet-0"><span class="c1">El cliente revisa si tiene alg&uacute;n mensaje</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Selecciona una conversaci&oacute;n iniciada</span></li>
        <li class="c2 li-bullet-0"><span class="c1">El vendedor y el cliente pueden tener un medio de contacto
                directo</span></li>
    </ul>
    <ol class="c0 lst-kix_rg52xa75v2qv-0" start="11">
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad del sistema de favoritos (wishlist).</span>
        </li>
    </ol>
    <ul class="c0 lst-kix_443kk3whga57-0 start">
        <li class="c2 li-bullet-0"><span class="c1">Se muestra el cat&aacute;logo de autos</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Si al cliente le interesa alg&uacute;n auto lo marca como
                favorito</span></li>
        <li class="c2 li-bullet-0"><span class="c1">En el apartado indicado el cliente puede revisar su lista de
                favoritos con los autos que marc&oacute; previamente </span></li>
    </ul>
    <ol class="c0 lst-kix_rg52xa75v2qv-0" start="12">
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de la edici&oacute;n de datos en el
                perfil.</span></li>
    </ol>
    <ul class="c0 lst-kix_vwqv628w1cm9-0 start">
        <li class="c2 li-bullet-0"><span class="c1">El cliente puede acceder a los ajustes de su cuenta en el apartado
                indicado</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Dentro de los ajustes puede seleccionar la opci&oacute;n de
                modificar sus datos</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Al entrar a la opci&oacute;n modifica los datos necesarios y al
                final selecciona el bot&oacute;n de guardar cambios</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Los datos se actualizan tanto en la vista del cliente, como en la
                base de datos</span></li>
    </ul>
    <p class="c4 c36 c12"><span class="c1"></span></p>
    <p class="c4 c36 c12"><span class="c1"></span></p>
    <p class="c4 c36 c56"><span class="c55 c5">Flujo del Super Administrador:</span></p>
    <ol class="c0 lst-kix_gcnxpnn6kj0u-0 start" start="1">
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de Login.</span></li>
    </ol>
    <ul class="c0 lst-kix_wcxg857dis8q-0 start">
        <li class="c2 li-bullet-0"><span class="c1">Acceso v&aacute;lido con Credenciales correctas de
                super-administrador</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Acceso no autorizado con correo invalido/cuenta inexistente</span>
        </li>
        <li class="c2 li-bullet-0"><span class="c1">Acceso no autorizado con contrase&ntilde;a incorrecta</span></li>
    </ul>
    <ol class="c0 lst-kix_gcnxpnn6kj0u-0" start="2">
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de b&uacute;squeda de usuarios.</span></li>
    </ol>
    <ul class="c0 lst-kix_cj4e1u6rjkyy-0 start">
        <li class="c2 li-bullet-0"><span class="c1">Se hace una b&uacute;squeda de un usuario dentro del
                cat&aacute;logo</span></li>
        <li class="c2 li-bullet-0"><span class="c1">El sistema muestra los resultados de los usuarios seg&uacute;n la
                b&uacute;squeda</span></li>
    </ul>
    <ol class="c0 lst-kix_gcnxpnn6kj0u-0" start="3">
        <li class="c3 li-bullet-0"><span class="c1">Probar las funcionalidad de filtrado de usuarios.</span></li>
    </ol>
    <ul class="c0 lst-kix_px402vn9x8-0 start">
        <li class="c2 li-bullet-0"><span class="c1">Dentro de la b&uacute;squeda de usuarios se muestran los filtros
                disponibles para la b&uacute;squeda</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Se seleccionan los filtros deseados</span></li>
        <li class="c2 li-bullet-0"><span class="c1">El sistema muestra los resultados de lo usuarios seg&uacute;n los
                filtros aplicados</span></li>
    </ul>
    <ol class="c0 lst-kix_gcnxpnn6kj0u-0" start="4">
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de la modificaci&oacute;n de datos de un
                grupo automotriz.</span></li>
    </ol>
    <ul class="c0 lst-kix_mo3vsi1bdout-0 start">
        <li class="c2 li-bullet-0"><span class="c1">Se accede a la p&aacute;gina de la cuenta del grupo automotriz con
                acceso de super-administrador</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Se efect&uacute;a un cambio de la informaci&oacute;n del grupo
                automotriz desde la p&aacute;gina de la cuenta.</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Se guardan los cambios de la cuenta del grupo automotriz.</span>
        </li>
    </ul>
    <ol class="c0 lst-kix_gcnxpnn6kj0u-0" start="5">
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de la b&uacute;squeda de solicitudes.</span>
        </li>
    </ol>
    <ul class="c0 lst-kix_vkx9pph5x7p6-0 start">
        <li class="c2 li-bullet-0"><span class="c1">Se hace una b&uacute;squeda de una solicitud dentro del
                cat&aacute;logo</span></li>
        <li class="c2 li-bullet-0"><span class="c1">El sistema muestra los resultados de las solicitudes y sus
                estados</span></li>
    </ul>
    <ol class="c0 lst-kix_gcnxpnn6kj0u-0" start="6">
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad del filtrado de solicitudes.</span></li>
    </ol>
    <ul class="c0 lst-kix_y2tifijecnbl-0 start">
        <li class="c2 li-bullet-0"><span class="c1">Dentro de la b&uacute;squeda de solicitudes se muestran los filtros
                disponibles para la b&uacute;squeda</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Se seleccionan los filtros deseados</span></li>
        <li class="c2 li-bullet-0"><span class="c1">El sistema muestra los resultados de las solicitudes seg&uacute;n
                los filtros aplicados (aprobada/pendiente/denegada)</span></li>
    </ul>
    <ol class="c0 lst-kix_gcnxpnn6kj0u-0" start="7">
        <li class="c3 li-bullet-0"><span class="c1">Probar funcionalidad de la aprobaci&oacute;n/negaci&oacute;n de una
                solicitud.</span></li>
    </ol>
    <ul class="c0 lst-kix_6y7yxgsemxkh-0 start">
        <li class="c2 li-bullet-0"><span class="c1">Se elige una solicitud pendiente con acceso de
                super-administrador</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Se efect&uacute;a la aprobaci&oacute;n de una solicitud en
                espera</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Se efect&uacute;a la negaci&oacute;n de una solicitud en
                espera</span></li>
    </ul>
    <ol class="c0 lst-kix_gcnxpnn6kj0u-0" start="8">
        <li class="c75 c42 c36 li-bullet-0"><span class="c1">Probar la funcionalidad del registro de un grupo
                automotriz.</span></li>
    </ol>
    <ul class="c0 lst-kix_chmh4a308mm1-0 start">
        <li class="c75 c36 c46 c90 li-bullet-0"><span class="c1">Se accede al landing-page de creaci&oacute;n de grupo
                automotriz.</span></li>
        <li class="c75 c36 c46 c90 li-bullet-0"><span class="c1">Creaci&oacute;n exitosa de un grupo automotriz</span>
        </li>
        <li class="c75 c36 c46 c90 li-bullet-0"><span class="c1">Acceso exitoso a la cuenta del grupo automotriz</span>
        </li>
    </ul>
    <ol class="c0 lst-kix_gcnxpnn6kj0u-0" start="9">
        <li class="c75 c42 c36 li-bullet-0"><span class="c1">Probar la funcionalidad del dashboard estad&iacute;stico.
            </span></li>
    </ol>
    <ul class="c0 lst-kix_avq738omluz-0 start">
        <li class="c2 li-bullet-0"><span class="c1">Acceso al dashboard con una cuenta de nivel valido muestra las
                estad&iacute;sticas y m&eacute;tricas de la plataforma</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Las estad&iacute;sticas son v&aacute;lidas y representativas de los
                datos dentro del sistema</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Las opciones y par&aacute;metros presentes dentro de la vista
                permiten ver estad&iacute;sticas particulares de acuerdo a la selecci&oacute;n de las mismas.</span>
        </li>
    </ul>
    <p class="c4 c12 c36"><span class="c1"></span></p>
    <p class="c4 c36 c56"><span class="c55 c5">Flujo del Vendedor:</span></p>
    <ol class="c0 lst-kix_mg52369i75sn-0" start="9">
        <li class="c3 li-bullet-0"><span class="c1">Probar funcionalidad del Login.</span></li>
    </ol>
    <ul class="c0 lst-kix_hdfcogwop0vx-0 start">
        <li class="c2 li-bullet-0"><span class="c1">Acceso v&aacute;lido con Credenciales correctas de vendedor</span>
        </li>
        <li class="c2 li-bullet-0"><span class="c1">Acceso no autorizado con correo invalido/cuenta inexistente</span>
        </li>
        <li class="c2 li-bullet-0"><span class="c1">Acceso no autorizado con contrase&ntilde;a incorrecta</span></li>
    </ul>
    <ol class="c0 lst-kix_mg52369i75sn-0" start="10">
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de b&uacute;squeda de
                cat&aacute;logo.</span></li>
    </ol>
    <ul class="c0 lst-kix_e5d5ipugdti2-0 start">
        <li class="c2 li-bullet-0"><span class="c1">Se hace una b&uacute;squeda de un auto dentro del
                cat&aacute;logo</span></li>
        <li class="c2 li-bullet-0"><span class="c1">El sistema muestra los resultados de los autos segun la
                b&uacute;squeda</span></li>
    </ul>
    <ol class="c0 lst-kix_mg52369i75sn-0" start="11">
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de filtrado de cat&aacute;logo.</span></li>
    </ol>
    <ul class="c0 lst-kix_9ovnuv191t9a-0 start">
        <li class="c2 li-bullet-0"><span class="c1">Dentro de la b&uacute;squeda de un auto del cat&aacute;logo se
                muestran los filtros disponibles para la b&uacute;squeda</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Se seleccionan los filtros deseados</span></li>
        <li class="c2 li-bullet-0"><span class="c1">El sistema muestra los resultados de los autos seg&uacute;n los
                filtros aplicados</span></li>
    </ul>
    <ol class="c0 lst-kix_mg52369i75sn-0" start="12">
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad de la b&uacute;squeda de solicitudes.</span>
        </li>
    </ol>
    <ul class="c0 lst-kix_yhyf0j2galop-0 start">
        <li class="c2 li-bullet-0"><span class="c1">Se hace una b&uacute;squeda de una solicitud dentro del
                cat&aacute;logo</span></li>
        <li class="c2 li-bullet-0"><span class="c1">El sistema muestra los resultados de las solicitudes y sus
                estados</span></li>
    </ul>
    <ol class="c0 lst-kix_mg52369i75sn-0" start="13">
        <li class="c3 li-bullet-0"><span class="c1">Probar la funcionalidad del filtrado de solicitudes.</span></li>
    </ol>
    <ul class="c0 lst-kix_ma8jl2wvcrl-0 start">
        <li class="c2 li-bullet-0"><span class="c1">Dentro de la b&uacute;squeda de solicitudes se muestran los filtros
                disponibles para la b&uacute;squeda</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Se seleccionan los filtros deseados</span></li>
        <li class="c2 li-bullet-0"><span class="c1">El sistema muestra los resultados de las solicitudes seg&uacute;n
                los filtros aplicados (aprobada/pendiente/denegada)</span></li>
    </ul>
    <ol class="c0 lst-kix_mg52369i75sn-0" start="14">
        <li class="c3 li-bullet-0"><span class="c1 c50">Probar funcionalidad del manejo de una solicitud.</span></li>
    </ol>
    <ul class="c0 lst-kix_nzvnkv2irake-0 start">
        <li class="c2 c12 li-bullet-0"><span class="c1"></span></li>
    </ul>
    <ol class="c0 lst-kix_mg52369i75sn-0" start="15">
        <li class="c3 li-bullet-0"><span class="c1">Probar funcionalidad del sistema de chat.</span></li>
    </ol>
    <ul class="c0 lst-kix_sxsbp83evw5r-0 start">
        <li class="c2 li-bullet-0"><span class="c1">Entrada a la vista de chats y contactos con acceso de
                vendedor</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Selecci&oacute;n de una conversaci&oacute;n iniciada</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Creaci&oacute;n de una conversaci&oacute;n desde vista de
                contacto</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Enviar mensaje al cliente</span></li>
    </ul>
    <ol class="c0 lst-kix_mg52369i75sn-0" start="16">
        <li class="c3 li-bullet-0"><span class="c1">Probar funcionalidad del dashboard estad&iacute;stico.</span></li>
    </ol>
    <ul class="c0 lst-kix_87xx17fjt6sp-0 start">
        <li class="c2 li-bullet-0"><span class="c1">Acceso al dashboard con una cuenta de nivel valido muestra las
                estad&iacute;sticas y m&eacute;tricas de la plataforma</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Las estad&iacute;sticas son v&aacute;lidas y representativas de los
                datos dentro del sistema</span></li>
        <li class="c2 li-bullet-0"><span class="c1">Las opciones y par&aacute;metros presentes dentro de la vista
                permiten ver estad&iacute;sticas particulares de acuerdo a la selecci&oacute;n de las mismas.</span>
        </li>
    </ul>
    <p class="c4 c36"><span
            class="c1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>
    </p>
    <ol class="c0 lst-kix_d3i63clc3lgg-1" start="4">
        <li class="c4 c15 c46 li-bullet-0">
            <h2 id="h.h904v6h0rrrr" style="display:inline"><span class="c35">Niveles de pruebas</span></h2>
        </li>
    </ol>
    <p class="c4 c36"><span class="c1">A continuaci&oacute;n se muestran el nivel de las pruebas que se
            realizar&aacute;n durante el desarrollo del proyecto, adem&aacute;s de detallar algunas de los
            m&eacute;todos que se utilizaran al igual que los responsables de dichas pruebas.</span></p>
    <p class="c4 c36 c69"><span class="c35">Pruebas Informales</span></p>
    <p class="c4 c36 c85"><span class="c5">El prop&oacute;sito de este tipo de pruebas es verificar r&aacute;pidamente
            el funcionamiento de los componentes del software. Las pruebas de este estilo no tienen ning&uacute;n tipo
            de entrega.</span></p>
    <ol class="c0 lst-kix_p4d0i57im8n6-0 start" start="1">
        <li class="c4 c7 li-bullet-0"><span class="c1">Alcance: Todas las secciones desarrolladas ser&aacute;n probadas
                mediante pruebas unitarias informales.</span></li>
        <li class="c4 c7 li-bullet-0"><span class="c1">Responsables: Todos los integrantes del equipo llevar&aacute;n a
                cabo pruebas unitarias informales.</span></li>
        <li class="c4 c7 li-bullet-0"><span class="c1">Metodolog&iacute;a: Los desarrolladores responsables del
                componentes se encargaran de realizar pruebas de Input-Output para comprobar su correcto
                funcionamiento.</span></li>
        <li class="c4 c7 li-bullet-0"><span class="c1">Cada cuando: En cuanto se finalice, o se modifique alg&uacute;n
                componente.</span></li>
    </ol>
    <p class="c4 c36 c56 c12"><span class="c1"></span></p>
    <p class="c4 c36 c69"><span class="c52 c88">Prueba de Caja Negra</span></p>
    <p class="c4 c36 c85"><span class="c5">El prop&oacute;sito de las pruebas unitarias es probar cada uno de los
            componentes y funcionalidades &nbsp;que comprenden la aplicaci&oacute;n que se desarrollar&aacute;.</span>
    </p>
    <p class="c4 c36 c56 c12"><span class="c35"></span></p>
    <ol class="c0 lst-kix_xs41mtxr57df-0 start" start="1">
        <li class="c4 c7 li-bullet-0"><span class="c5">Alcanc</span><sup><a href="#cmnt5"
                    id="cmnt_ref5">[e]</a></sup><span class="c1">e: Todas las secciones desarrolladas ser&aacute;n
                probadas mediante pruebas de caja negra.</span></li>
        <li class="c4 c7 li-bullet-0"><span class="c1">Responsables: Los desarrolladores de software y los
                testers.</span></li>
        <li class="c4 c7 li-bullet-0"><span class="c1">Metodolog&iacute;a: Los desarrolladores probar&aacute;n
                componentes de la aplicaci&oacute;n sin tener conocimiento del c&oacute;digo detr&aacute;s de los mismos
                componentes, reportando errores en caso de encontrarlos. Espec&iacute;ficamente, el tipo de pruebas de
                caja negra que se realizar&aacute;n ser&aacute;n pruebas de tipo de casos de uso. Dentro de estas
                pruebas se realizar&aacute;n tres bater&iacute;as negativas y tres bater&iacute;as positivas que se
                deber&aacute;n cumplir cuando se realicen este tipo de pruebas.</span></li>
        <li class="c4 c7 li-bullet-0"><span class="c1">Cada cu&aacute;ndo: Al finalizar cada componente.</span></li>
    </ol>
    <p class="c58 c36 c12"><span class="c37"></span></p>
    <h3 class="c4 c67" id="h.91fzm9dtgvmr"><span>Prueba de Caja Blanca</span><sup><a href="#cmnt6"
                id="cmnt_ref6">[f]</a></sup><sup><a href="#cmnt7" id="cmnt_ref7">[g]</a></sup></h3>
    <p class="c19"><span class="c5">El prop&oacute;sito de este tipo de pruebas es encontrar la causa de alg&uacute;n
            tipo de falla que se </span><sup><a href="#cmnt8" id="cmnt_ref8">[h]</a></sup><span class="c5">haya
            encontrado en otro tipo de pruebas. En espec&iacute;fico, las pruebas de caja blanca que se realizan son
            pruebas de cobertura, es decir, se probar&aacute;n los tres caminos m&aacute;s utilizados por los usuarios
            para as&iacute; justificar que el componente funciona bien. </span><span class="c1 c50">A&Ntilde;ADIR
            PORCENTAJE</span></p>
    <ol class="c0 lst-kix_wzt0u5vle4mu-0 start" start="1">
        <li class="c7 c58 li-bullet-0"><span class="c1">Alcance: Cualquier componente de software que presente alguna
                falla dentro de alg&uacute;n otro tipo de prueba.</span></li>
        <li class="c7 c58 li-bullet-0"><span class="c1">Responsables: Los desarrolladores de software y los
                testers..</span></li>
        <li class="c7 c58 li-bullet-0"><span class="c1">Metodolog&iacute;a: Los desarrolladores que se encargaron de
                crear los componentes en donde se encontraron los errores ser&aacute;n los encargados de realizar
                pruebas de caja blanca con el objetivo de encontrar que pedazo de c&oacute;digo es el que est&aacute;
                causando dicho error.</span></li>
        <li class="c7 c58 li-bullet-0"><span class="c1">Cada cu&aacute;ndo: Al finalizar cada sprint.</span></li>
    </ol>
    <h3 class="c4 c20 c31" id="h.7e2hupja93t3"><span class="c35"></span></h3>
    <h3 class="c4 c67" id="h.xhc6264rls1i"><span class="c35">Prueba de Integraci&oacute;n</span></h3>
    <p class="c19"><span class="c5">El prop&oacute;sito de las pruebas de integraci&oacute;n es comprobar el correcto
            funcionamiento de la aplicaci&oacute;n cuando todos los componentes son utilizados en conjunto. </span><span
            class="c1 c50">DESCRIBIR QUE SOLO SE HAR&Aacute; CON LOS COMPONENTES CR&Iacute;TICOS</span></p>
    <ol class="c0 lst-kix_dgjxhhel0iia-0 start" start="1">
        <li class="c7 c58 li-bullet-0"><span class="c1">Alcance: Todo el software en conjunto ser&aacute; probado de
                esta manera.</span></li>
        <li class="c7 c58 li-bullet-0"><span class="c1">Responsables: Los responsables de cada c&eacute;lula de
                trabajo.</span></li>
        <li class="c7 c58 li-bullet-0"><span class="c1">Metodolog&iacute;a: Los desarrolladores responsables de cada
                c&eacute;lula, al terminar m&aacute;s de un componente relacionado, empezaran a realizar pruebas e
                integraci&oacute;n. De la misma manera, al terminar el proyecto, se realizar&aacute;n &nbsp;nuevas
                pruebas de este estilo.</span></li>
        <li class="c7 c58 li-bullet-0"><span class="c5">Cada cu&aacute;ndo: Al </span><span class="c5">terminarse
                pedazos</span><span class="c1">&nbsp;de software relacionados y al acabar todos los componentes de la
                aplicaci&oacute;n.</span></li>
    </ol>
    <p class="c58 c36 c12"><span class="c1"></span></p>
    <h3 class="c4 c67" id="h.j8epsprogp2p"><span class="c35">Prueba de Aceptaci&oacute;n</span></h3>
    <p class="c19"><span class="c1">El prop&oacute;sito de este tipo de pruebas es validar con NDS si el sistema
            est&aacute; a la par con sus expectativas y cumple las funcionalidades que fueron discutidas en el documento
            SRS.</span></p>
    <ol class="c0 lst-kix_i0244pw02jv6-0 start" start="1">
        <li class="c7 c58 li-bullet-0"><span class="c1">Alcance: Todos los aspectos del pedazo de software ser&aacute;n
                probados pruebas de validaci&oacute;n. Esto con el objetivo de revisar si aspectos de dise&ntilde;o y
                funcionalidad de la aplicaci&oacute;n est&aacute;n a la par de las expectativas de NDS.</span></li>
        <li class="c7 c58 li-bullet-0"><span class="c1">Responsables: Rub&eacute;n Raya (NDS), los desarrolladores, los
                testers y el SCRUM master..</span></li>
        <li class="c7 c58 li-bullet-0"><span class="c1">Metodolog&iacute;a: Los desarrolladores se reunir&aacute;n con
                Rub&eacute;n Raya y bajo su supervisi&oacute;n se encargar&aacute; de validar los aspectos importantes
                de la aplicaci&oacute;n desarrollada.</span></li>
        <li class="c7 c58 li-bullet-0"><span class="c1">Cada cu&aacute;ndo:En cuanto se cumplan las pruebas de
                integraci&oacute;n.</span></li>
    </ol>
    <p class="c36 c48"><span class="c52 c88">Prueba de Validaci&oacute;n</span><sup><a href="#cmnt9"
                id="cmnt_ref9">[i]</a></sup></p>
    <p class="c48 c36 c12"><span class="c1"></span></p>
    <h3 class="c4 c67" id="h.qsyst13rz67j"><span class="c35">Prueba de Recorrido Est&aacute;tico</span></h3>
    <p class="c19"><span class="c1">El prop&oacute;sito de este tipo de pruebas es asegurar que el servicio, en
            t&eacute;rminos de funcionalidad y desempe&ntilde;o, act&uacute;e de manera satisfactoria..</span></p>
    <ol class="c0 lst-kix_rg98grvtj3pg-0 start" start="1">
        <li class="c7 c58 li-bullet-0"><span class="c1">Alcance: Dado que se trata de una prueba de sistema, el software
                ser&aacute; probado en completud.</span></li>
        <li class="c7 c58 li-bullet-0"><span class="c1">Responsables: Desarrolladores no pertenecientes al
                proyecto.</span></li>
        <li class="c7 c58 li-bullet-0"><span class="c1">Metodolog&iacute;a: Crear escenarios de acuerdo a las
                situaciones m&aacute;s usuales de los usuarios.</span></li>
        <li class="c7 c58 li-bullet-0"><span class="c1">Cada cu&aacute;ndo: Al final del proyecto.</span></li>
    </ol>
    <h2 class="c4 c20" id="h.gwsxrckj7v6b"><span class="c35"></span></h2>
    <ol class="c0 lst-kix_d3i63clc3lgg-1" start="5">
        <li class="c4 c15 c36 c46 li-bullet-0">
            <h2 id="h.cwh2skhwocng" style="display:inline"><span class="c50">Criterios de aceptaci&oacute;n de
                    pruebas</span><sup><a href="#cmnt10" id="cmnt_ref10">[j]</a></sup></h2>
        </li>
    </ol>
    <p class="c84 c36 c56"><span class="c66">Pruebas Informales</span></p>
    <h3 class="c4 c15" id="h.fsv2ynwal6n0"><span>Pruebas Unitarias / Informales</span><span class="c35">&nbsp;</span>
    </h3>
    <ul class="c0 lst-kix_q48tat6aasri-0 start">
        <li class="c4 c42 c94 li-bullet-0"><span class="c5 c104">Funcionalidad de Login:</span><span
                class="c1">&nbsp;Esta funcionalidad nunca debe fallar. Todas las pruebas deben proporcionar el usuario y
                la p&aacute;gina de inicio correctos, o bien enviar un mensaje de error indicando que el usuario no
                existe. Esto para cada tipo de usuario que permite la plataforma.</span></li>
        <li class="c4 c42 c94 li-bullet-0"><span class="c5 c104">Funcionalidad de Registro:</span><span
                class="c1">&nbsp;Todas las pruebas deben de crear las credenciales ingresadas de forma correcta en la
                base de datos o bien enviar un mensaje de error indicando la raz&oacute;n por la cual las credenciales
                no son permitidas. Igualmente, el registro debe agregar la cuenta con los privilegios y permisos
                correspondientes a cada tipo de usuario.</span></li>
        <li class="c4 c42 c94 li-bullet-0"><span class="c1">Funcionalidad CRUD del Cat&aacute;logo: </span></li>
    </ul>
    <p class="c4 c12 c73 c94"><span class="c1"></span></p>
    <h3 class="c4 c15" id="h.kzej3b9e4wfe"><span>Prueba de Integraci&oacute;n</span></h3>
    <ul class="c0 lst-kix_u2d5nq9gvteo-0 start">
        <li class="c4 c42 li-bullet-0"><span class="c1">&nbsp; </span></li>
    </ul>
    <h3 class="c4 c15 c102" id="h.ns3vrtfyjguc"><span>Prueba de Validaci&oacute;n</span></h3>
    <ul class="c0 lst-kix_3rm0szfqxvyi-0 start">
        <li class="c4 c42 li-bullet-0"><span class="c1">The clients and stakeholders are satisfied with the
                functionalities. &nbsp;</span></li>
    </ul>
    <h3 class="c4 c15" id="h.7krppuwc58yf"><span>Prueba de Sistema</span></h3>
    <ul class="c0 lst-kix_5e4latf0qe1x-0 start">
        <li class="c4 c42 c98 li-bullet-0"><span class="c1">The basic flow is able to be completed in one run, from log
                in to log out. Agents are &nbsp;able to log in, record a video, save it, and log out; while
                Administrators and &nbsp;Supervisors can log in, see their analysis, and log out.</span></li>
    </ul>
    <p class="c4 c12 c98"><span class="c1"></span></p>
    <ol class="c0 lst-kix_d3i63clc3lgg-1" start="6">
        <li class="c4 c15 c36 c46 li-bullet-0">
            <h2 id="h.s6ntvdjxs5wr" style="display:inline"><span class="c35">Entregables de pruebas</span></h2>
        </li>
    </ol>
    <h2 class="c4 c20 c115" id="h.ev54v0h5kuu0"><span class="c35"></span></h2><a
        id="t.bc86d7e36674b8ba87018d9096ba7e3ada76be7c"></a><a id="t.2"></a>
    <table class="c103">
        <tr class="c44">
            <td class="c26" colspan="1" rowspan="1">
                <p class="c4"><span class="c17">No.</span></p>
            </td>
            <td class="c40" colspan="1" rowspan="1">
                <p class="c4"><span class="c17">Nombre de entregable</span></p>
            </td>
            <td class="c47" colspan="1" rowspan="1">
                <p class="c4"><span class="c17">Autor</span></p>
            </td>
            <td class="c72" colspan="1" rowspan="1">
                <p class="c4"><span class="c17">Reviewer</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c26" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">1.</span></p>
            </td>
            <td class="c40" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Plan de Pruebas</span></p>
            </td>
            <td class="c47" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Director de Pruebas</span></p>
            </td>
            <td class="c72" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Project Manager/Analista de Negocios</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c26" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">2.</span></p>
            </td>
            <td class="c40" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Revisi&oacute;n T&eacute;cnica Formal</span></p>
            </td>
            <td class="c47" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Director de Pruebas</span></p>
            </td>
            <td class="c72" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Project Manager/Analista de Negocios</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c26" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">3.</span></p>
            </td>
            <td class="c40" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Resultados de Pruebas Unitarias</span></p>
            </td>
            <td class="c47" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Equipo de Pruebas</span></p>
            </td>
            <td class="c72" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Project Manager</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c26" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">4.</span></p>
            </td>
            <td class="c40" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Resultados de Pruebas Integrales</span></p>
            </td>
            <td class="c47" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Equipo de Pruebas</span></p>
            </td>
            <td class="c72" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Project Manager</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c26" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">5.</span></p>
            </td>
            <td class="c40" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Resultados de Pruebas de Validaci&oacute;n</span></p>
            </td>
            <td class="c47" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Equipo de Pruebas</span></p>
            </td>
            <td class="c72" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Project Manager</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c26" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">6.</span></p>
            </td>
            <td class="c40" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Resultados de la Prueba de Sistema</span></p>
            </td>
            <td class="c47" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Equipo de Pruebas</span></p>
            </td>
            <td class="c72" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Project Manager</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c26" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">7.</span></p>
            </td>
            <td class="c40" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Reporte Diario/Semanal del Estatus</span></p>
            </td>
            <td class="c47" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Director de Pruebas/ Equipo de Pruebas</span></p>
            </td>
            <td class="c72" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Director de Pruebas/Project Manager</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c26" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">8.</span></p>
            </td>
            <td class="c40" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Reporte de Cierre</span></p>
            </td>
            <td class="c47" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Director de Pruebas</span></p>
            </td>
            <td class="c72" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Project Manager</span></p>
            </td>
        </tr>
    </table>
    <p class="c4 c12"><span class="c17"></span></p>
    <ol class="c0 lst-kix_d3i63clc3lgg-1" start="7">
        <li class="c4 c15 c46 li-bullet-0">
            <h2 id="h.vqt91vksszs0" style="display:inline"><span>Lista de hitos</span><sup><a href="#cmnt11"
                        id="cmnt_ref11">[k]</a></sup><span>&nbsp;</span></h2>
        </li>
    </ol>
    <p class="c4"><span class="c1">La lista de hitos es tentativa y puede cambiar por las siguientes razones</span></p>
    <ol class="c0 lst-kix_4ch1bnhitet1-0 start" start="1">
        <li class="c4 c69 c46 li-bullet-0"><span class="c1">Cualquier problema con la preparaci&oacute;n del entorno del
                Sistema</span></li>
        <li class="c4 c69 c46 li-bullet-0"><span class="c1">Cualquier cambio en el alcance o cosas agregadas al alcance
                del proyecto</span></li>
        <li class="c4 c69 c46 li-bullet-0"><span class="c5">Cualquier otra dependencia que afecte el esfuerzo y el
                tiempo</span></li>
    </ol>
    <p class="c4 c12"><span class="c1"></span></p><a id="t.f760153bda7e5d92abca3374153b0383accecd2f"></a><a
        id="t.3"></a>
    <table class="c69 c113">
        <tr class="c44">
            <td class="c21" colspan="1" rowspan="1">
                <p class="c4"><span class="c17">No.</span></p>
            </td>
            <td class="c34" colspan="1" rowspan="1">
                <p class="c4"><span class="c17">Tipo de prueba</span></p>
            </td>
            <td class="c41" colspan="1" rowspan="1">
                <p class="c4"><span class="c17">Ejemplo de Prueba (SUT)</span></p>
            </td>
            <td class="c32" colspan="1" rowspan="1">
                <p class="c4"><span class="c17">Dependencia (DOC)</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c21" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">1</span></p>
            </td>
            <td class="c34" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Pruebas Unitarias</span></p>
            </td>
            <td class="c41" colspan="1" rowspan="1">
                <p class="c4"><span class="c52">Registro de la Plataforma: </span><span class="c1">Probar que el proceso
                        de registro funciona correctamente para cada tipo de usuario.</span></p>
            </td>
            <td class="c32" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">- Base de Datos Completada y conectada. </span></p>
                <p class="c4"><span class="c1">- API Completado y Funcional.</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c21" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">3</span></p>
            </td>
            <td class="c34" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Pruebas Unitarias</span></p>
                <p class="c4 c12"><span class="c1"></span></p>
            </td>
            <td class="c41" colspan="1" rowspan="1">
                <p class="c4"><span class="c52">Login de la Plataforma: </span><span class="c1">Probar que el proceso de
                        Login funciona correctamente para cada tipo de usuario.</span></p>
            </td>
            <td class="c32" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">- Base de Datos Completada y conectada. </span></p>
                <p class="c4"><span class="c1">- API Completado y Funcional.</span></p>
                <p class="c4"><span class="c1">- Configuraci&oacute;n de Autenticaci&oacute;n y
                        Autorizaci&oacute;n</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c21" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">4</span></p>
            </td>
            <td class="c34" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Pruebas Unitarias</span></p>
                <p class="c4 c12"><span class="c1"></span></p>
            </td>
            <td class="c41" colspan="1" rowspan="1">
                <p class="c4"><span class="c52">Modificaci&oacute;n del Cat&aacute;logo:</span><span
                        class="c1">&nbsp;Probar que los usuarios autorizados pueden subir, modificar y eliminar
                        elementos del cat&aacute;logo correctamente.</span></p>
            </td>
            <td class="c32" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">- Base de Datos Completada y conectada.</span></p>
                <p class="c4"><span class="c1">- API Completado y Funcional.</span></p>
                <p class="c4"><span class="c1">- Configuraci&oacute;n de privilegios completada. </span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c21" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">5</span></p>
            </td>
            <td class="c34" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Pruebas Unitarias</span></p>
                <p class="c4 c12"><span class="c1"></span></p>
            </td>
            <td class="c41" colspan="1" rowspan="1">
                <p class="c4"><span class="c52">Funcionalidad de B&uacute;squeda:</span><span class="c1">&nbsp;Probar
                        que los diferentes tipos de usuarios pueden buscar correctamente la informaci&oacute;n que
                        desean mediante la barra de navegaci&oacute;n </span></p>
            </td>
            <td class="c32" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">- Base de Datos Completada y conectada. </span></p>
                <p class="c4"><span class="c1">- API Completado y Funcional.</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c21" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">6</span></p>
            </td>
            <td class="c34" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Pruebas Unitarias</span></p>
                <p class="c4 c12"><span class="c1"></span></p>
            </td>
            <td class="c41" colspan="1" rowspan="1">
                <p class="c4"><span class="c52">Funcionalidad de Filtrado: </span><span class="c1">Probar que los
                        diferentes tipos de usuarios pueden filtrar correctamente la informaci&oacute;n que
                        desean.</span></p>
            </td>
            <td class="c32" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">- Base de Datos Completada y conectada. </span></p>
                <p class="c4"><span class="c1">- API Completado y Funcional.</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c21" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">7</span></p>
            </td>
            <td class="c34" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Pruebas Unitarias</span></p>
                <p class="c4 c12"><span class="c1"></span></p>
            </td>
            <td class="c41" colspan="1" rowspan="1">
                <p class="c4"><span class="c52">Funcionalidad de Pago: </span><span class="c1">Probar el proceso de
                        pagos asegurando que los usuarios pueden completar el pago de un auto de manera f&aacute;cil y
                        segura.</span></p>
            </td>
            <td class="c32" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">- Integraci&oacute;n de la herramienta externa de Pago/Transacciones
                        (Stripe)</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c21" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">8</span></p>
            </td>
            <td class="c34" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Pruebas Unitarias</span></p>
                <p class="c4 c12"><span class="c1"></span></p>
            </td>
            <td class="c41" colspan="1" rowspan="1">
                <p class="c4"><span class="c52">Funcionalidad de Chat: </span><span class="c1">Probar que los diferentes
                        tipos de usuario pueden comunicarse exitosamente entre s&iacute; mediante el Chat interno de la
                        plataforma.</span></p>
            </td>
            <td class="c32" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">- Base de Datos completada y conectada.</span></p>
                <p class="c4"><span class="c1">- Integraci&oacute;n de librer&iacute;a externa para desarrollo del Chat
                        (Socket IO).</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c21" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">9</span></p>
            </td>
            <td class="c34" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Pruebas Unitarias</span></p>
                <p class="c4 c12"><span class="c1"></span></p>
            </td>
            <td class="c41" colspan="1" rowspan="1">
                <p class="c4"><span class="c52">Funcionalidad de Favoritos</span><span class="c1">: Probar que los
                        usuarios puedan seleccionar y guardar sus autos favoritos.</span></p>
            </td>
            <td class="c32" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">- Base de Datos Completada y conectada. </span></p>
                <p class="c4"><span class="c1">- API Completado y Funcional.</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c21" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">10</span></p>
            </td>
            <td class="c34" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Pruebas Unitarias</span></p>
                <p class="c4 c12"><span class="c1"></span></p>
            </td>
            <td class="c41" colspan="1" rowspan="1">
                <p class="c4"><span class="c17">Funcionalidad de An&aacute;lisis de Documentos:</span></p>
                <p class="c4"><span class="c1">Probar que autom&aacute;ticamente se analiza correctamente la validez de
                        un documento.</span></p>
            </td>
            <td class="c32" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">- Integraci&oacute;n de servicio de AWS Textract</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c21" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">11</span></p>
            </td>
            <td class="c34" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Pruebas Unitarias</span></p>
                <p class="c12 c107"><span class="c1"></span></p>
            </td>
            <td class="c41" colspan="1" rowspan="1">
                <p class="c4"><span class="c52">Funcionalidad Anal&iacute;tica: </span><span class="c1">Probar que el
                        dashboard muestre la informaci&oacute;n estad&iacute;stica correcta y adecuada para cada tipo de
                        usuario.</span></p>
            </td>
            <td class="c32" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">- Base de Datos Completada y conectada. </span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c21" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">12</span></p>
            </td>
            <td class="c34" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Pruebas Integrales</span></p>
            </td>
            <td class="c41" colspan="1" rowspan="1">
                <p class="c4"><span class="c17">Manejo de Solicitudes:</span></p>
                <p class="c4"><span class="c1">Probar que la plataforma maneja correctamente y actualiza la
                        informaci&oacute;n referente a el estado de las solicitudes tanto de compra como de prueba de
                        manejo.</span></p>
            </td>
            <td class="c32" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">- Base de Datos Completada y Conectada. </span></p>
                <p class="c4"><span class="c1">- Interfaz de modificaci&oacute;n de solicitudes completada. </span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c21" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">13</span></p>
            </td>
            <td class="c34" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Pruebas Integrales</span></p>
            </td>
            <td class="c41" colspan="1" rowspan="1">
                <p class="c4"><span class="c52">Aprobaci&oacute;n para compra de un auto: </span><span class="c1">Probar
                        que el proceso de compra funciona en todos sus casos (tanto de aprobaci&oacute;n como
                        negaci&oacute;n de la solicitud).</span></p>
            </td>
            <td class="c32" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">- Conexi&oacute;n funcional entre estado de solicitud y cliente.</span>
                </p>
                <p class="c4"><span class="c1">- An&aacute;lisis de documentos completamente funcional.</span></p>
                <p class="c4"><span class="c1">- Sistema de Chat completamente funcional.</span></p>
                <p class="c4"><span class="c1">- Funcional completa del sistema de pagos.</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c21" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">14</span></p>
            </td>
            <td class="c34" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Pruebas Integrales</span></p>
            </td>
            <td class="c41" colspan="1" rowspan="1">
                <p class="c4"><span class="c52">Aprobaci&oacute;n para agendado de una prueba de manejo: </span><span
                        class="c1">Probar que el proceso de agendado de un prueba de manejo funciona en todos sus casos
                        (aprobaci&oacute;n y negaci&oacute;n de la solicitud).</span></p>
            </td>
            <td class="c32" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">- Conexi&oacute;n funcional entre estado de solicitud y cliente.</span>
                </p>
                <p class="c4"><span class="c1">- An&aacute;lisis de documentos completamente funcional.</span></p>
                <p class="c4"><span class="c1">- Sistema de Chat completamente funcional.</span></p>
                <p class="c4"><span class="c1">- Conexi&oacute;n funcional entre agenda del vendedor y el
                        cliente.</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c21" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">15</span></p>
            </td>
            <td class="c34" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Pruebas de Validaci&oacute;n/Aceptaci&oacute;n</span></p>
            </td>
            <td class="c41" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">El dise&ntilde;o (UI/UX) cumple con los est&aacute;ndares del cliente.
                    </span></p>
            </td>
            <td class="c32" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Interfaz de dise&ntilde;o completada.</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c21" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">16</span></p>
            </td>
            <td class="c34" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Pruebas Est&aacute;ticas de Recorrido</span></p>
            </td>
            <td class="c41" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Cada uno de los flujos para cada tipo de usuario se relacionan
                        correctamente entre s&iacute;, y cumplen con los est&aacute;ndares y funcionalidad solicitada
                        por el cliente.</span></p>
            </td>
            <td class="c32" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">- Conexi&oacute;n e integraci&oacute;n completa entre el front-end y
                        back-end.</span></p>
                <p class="c4"><span class="c1">- Configuraciones de seguridad completas.</span></p>
                <p class="c4 c12"><span class="c1"></span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c21" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">17</span></p>
            </td>
            <td class="c34" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Manual de Usuario</span></p>
            </td>
            <td class="c41" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Se documenta el instructivo de uso para cada uno de los flujos de la
                        plataforma.</span></p>
            </td>
            <td class="c32" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">- Software completado y flujo completamente funcional</span></p>
            </td>
        </tr>
    </table>
    <p class="c4 c86 c12"><span class="c71"></span></p>
    <p class="c4 c69 c12 c86"><span class="c71"></span></p>
    <ol class="c0 lst-kix_d3i63clc3lgg-1" start="8">
        <li class="c4 c15 c46 li-bullet-0">
            <h2 id="h.tttcgn6nmo2n" style="display:inline"><span>E</span><span>stimaci&oacute;n de esfuerzo de las
                    pruebas</span></h2>
        </li>
    </ol>
    <p class="c4 c89"><span class="c1">Pruebas Est&aacute;ticas</span></p><a
        id="t.1de78adc822e329353f5d2b478cfd0db52769ad3"></a><a id="t.4"></a>
    <table class="c54">
        <tr class="c44">
            <td class="c57" colspan="1" rowspan="1">
                <p class="c28"><span class="c17">Tipo de Prueba</span></p>
            </td>
            <td class="c43" colspan="1" rowspan="1">
                <p class="c28"><span class="c17">Horas</span></p>
            </td>
            <td class="c78" colspan="1" rowspan="1">
                <p class="c28"><span class="c17">D&iacute;as</span></p>
            </td>
            <td class="c81" colspan="1" rowspan="1">
                <p class="c28"><span class="c17">Porcentaje del Proyecto</span></p>
            </td>
        </tr>
        <tr class="c45">
            <td class="c57" colspan="1" rowspan="1">
                <p class="c28"><span class="c1">SRS</span></p>
            </td>
            <td class="c43" colspan="1" rowspan="1">
                <p class="c28"><span class="c1">56 </span></p>
            </td>
            <td class="c78" colspan="1" rowspan="1">
                <p class="c28"><span class="c1">7</span></p>
            </td>
            <td class="c81" colspan="1" rowspan="2">
                <p class="c28"><span class="c1">6.41%</span></p>
            </td>
        </tr>
        <tr class="c45">
            <td class="c57" colspan="1" rowspan="1">
                <p class="c28"><span class="c1">Plan de Pruebas</span></p>
            </td>
            <td class="c43" colspan="1" rowspan="1">
                <p class="c28"><span class="c1">56</span></p>
            </td>
            <td class="c78" colspan="1" rowspan="1">
                <p class="c28"><span class="c1">7 </span></p>
            </td>
        </tr>
    </table>
    <p class="c4 c89 c12"><span class="c1"></span></p>
    <p class="c4 c89"><span class="c5">Pruebas Funcionales</span></p><a
        id="t.58acefe26023bb5ce6a5cee68e4cc83b83aa43d8"></a><a id="t.5"></a>
    <table class="c54">
        <tr class="c44">
            <td class="c59" colspan="1" rowspan="1">
                <p class="c28"><span class="c17">Tipo de Prueba</span></p>
            </td>
            <td class="c62" colspan="1" rowspan="1">
                <p class="c28"><span class="c17">Horas</span></p>
            </td>
            <td class="c53" colspan="1" rowspan="1">
                <p class="c28"><span class="c17">D&iacute;as</span></p>
            </td>
            <td class="c76" colspan="1" rowspan="1">
                <p class="c28"><span class="c17">Porcentaje del Proyecto</span></p>
            </td>
        </tr>
        <tr class="c45">
            <td class="c59" colspan="1" rowspan="1">
                <p class="c28"><span class="c1">Pruebas Informales</span></p>
            </td>
            <td class="c62" colspan="1" rowspan="1">
                <p class="c28"><span class="c1">N/A</span></p>
            </td>
            <td class="c53" colspan="1" rowspan="1">
                <p class="c28"><span class="c1">N/A</span></p>
            </td>
            <td class="c76" colspan="1" rowspan="5">
                <p class="c28"><span class="c1">11.68%</span></p>
            </td>
        </tr>
        <tr class="c45">
            <td class="c59" colspan="1" rowspan="1">
                <p class="c28"><span class="c1">Pruebas de Integraci&oacute;n</span></p>
            </td>
            <td class="c62" colspan="1" rowspan="1">
                <p class="c28"><span class="c1">28</span></p>
            </td>
            <td class="c53" colspan="1" rowspan="1">
                <p class="c28"><span class="c1">3.5</span></p>
            </td>
        </tr>
        <tr class="c45">
            <td class="c59" colspan="1" rowspan="1">
                <p class="c28"><span class="c1">Pruebas de Caja Negra</span></p>
            </td>
            <td class="c62" colspan="1" rowspan="1">
                <p class="c28"><span class="c1">56</span></p>
            </td>
            <td class="c53" colspan="1" rowspan="1">
                <p class="c28"><span class="c1">7</span></p>
            </td>
        </tr>
        <tr class="c45">
            <td class="c59" colspan="1" rowspan="1">
                <p class="c28"><span class="c1">Pruebas de Caja Blanca</span></p>
                <p class="c28"><span class="c1">*porcentaje variable dependiendo de qu&eacute; componentes lo
                        necesiten</span></p>
            </td>
            <td class="c62" colspan="1" rowspan="1">
                <p class="c28"><span class="c1">98</span></p>
            </td>
            <td class="c53" colspan="1" rowspan="1">
                <p class="c28"><span class="c1">12.25</span></p>
            </td>
        </tr>
        <tr class="c45">
            <td class="c59" colspan="1" rowspan="1">
                <p class="c28"><span class="c1">Prueba Pen-Testing </span></p>
            </td>
            <td class="c62" colspan="1" rowspan="1">
                <p class="c28"><span class="c1">22</span></p>
            </td>
            <td class="c53" colspan="1" rowspan="1">
                <p class="c28"><span class="c1">2.75</span></p>
            </td>
        </tr>
    </table>
    <p class="c36 c84"><span class="c5">La estimaci&oacute;n de esfuerzos anterior representa un 18.1% del total del
            proyecto.</span></p>
    <p class="c84 c36 c12 c108"><span class="c37"></span></p>
    <ol class="c0 lst-kix_d3i63clc3lgg-0" start="3">
        <li class="c4 c38 li-bullet-0">
            <h1 id="h.rggsbldjdzgj" style="display:inline"><span class="c39">Proceso de gesti&oacute;n de pruebas</span>
            </h1>
        </li>
    </ol>
    <ol class="c0 lst-kix_d3i63clc3lgg-1 start" start="1">
        <li class="c4 c15 c46 li-bullet-0">
            <h2 id="h.l5voq2cnpp4q" style="display:inline"><span class="c35">Proceso de ejecuci&oacute;n de
                    pruebas</span></h2>
        </li>
    </ol>
    <ol class="c0 lst-kix_lmcsya18g09n-0 start" start="1">
        <li class="c7 c49 li-bullet-0"><span class="c1">Aprobaci&oacute;n del plan de pruebas y funcionamiento del
                ambiente de pruebas en todos los dispositivos que ser&aacute;n utilizados.</span></li>
        <li class="c7 c49 li-bullet-0"><span class="c1">El ambiente de pruebas se comprueba por medio de una prueba
                informal que hagan de manera individual los desarrolladores. </span></li>
        <li class="c7 c49 li-bullet-0"><span class="c1">Siguiendo el cronograma del proyecto y el plan de pruebas, el
                project manager en conjunto con el l&iacute;der de pruebas asignar&aacute; a cada l&iacute;der sus
                respectivas pruebas.</span></li>
        <li class="c7 c49 li-bullet-0"><span class="c1">Conforme se finalicen componentes pero el cronograma no indique
                una prueba, los desarrolladores estar&aacute;n a cargo de las pruebas informales, y darles
                seguimiento.</span></li>
        <li class="c7 c49 li-bullet-0"><span class="c1">Cuando se indique la ejecuci&oacute;n de una prueba, cada
                l&iacute;der tiene la responsabilidad de asegurarse de delegar las pruebas a sus equipos y darles
                seguimiento. </span></li>
        <li class="c7 c58 li-bullet-0"><span class="c1">Cada desarrollador encargado de una prueba tiene la
                responsabilidad de documentar su proceso, el resultado de dicha prueba, el seguimiento que se le
                dar&aacute; y la correcci&oacute;n de los errores. </span></li>
    </ol>
    <ol class="c0 lst-kix_lmcsya18g09n-1 start" start="1">
        <li class="c48 c36 c46 li-bullet-0"><span class="c1">El desarrollador tiene la responsabilidad de hacer su
                proceso de QA e informar si se pasa o no la prueba.</span></li>
        <li class="c48 c36 c46 li-bullet-0"><span class="c1">Primero se ejecutar&aacute;n las pruebas de caja negra y en
                caso de que alg&uacute;n componente falle dicha prueba, se aplicar&aacute; la prueba de caja
                blanca.</span></li>
        <li class="c48 c36 c46 li-bullet-0"><span class="c1">Una vez que cada componente pase las pruebas unitarias, se
                ejecutar&aacute;n las pruebas de integraci&oacute;n.</span></li>
    </ol>
    <ol class="c0 lst-kix_lmcsya18g09n-0" start="7">
        <li class="c7 c58 li-bullet-0"><span class="c1">El desarrollador tiene la responsabilidad de informar a sus
                respectivos l&iacute;deres acerca del resultado de las pruebas de sus componentes. </span></li>
        <li class="c7 c58 li-bullet-0"><span class="c1">Si hay fallas, se le informar&aacute; a los l&iacute;deres y al
                project manager de acuerdo a la gravedad de ellas y se incluir&aacute;n capturas de pantalla, si es
                necesario.</span></li>
        <li class="c7 c58 li-bullet-0"><span class="c1">Este proceso se repite hasta que todos los casos de prueba se
                ejecuten por completo y tengan un estado en el que ya sea que pasen o fallen.</span></li>
    </ol>
    <ol class="c0 lst-kix_lmcsya18g09n-1 start" start="1">
        <li class="c48 c36 c46 li-bullet-0"><span class="c5">Durante el ciclo siguiente, se probar&aacute;n las pruebas
                falladas corregidas y los resultados se actualizar&aacute;n en el documento durante el ciclo hasta que
                todas las pruebas pasen.</span></li>
    </ol>
    <p class="c4 c56 c12"><span class="c1"></span></p>
    <ol class="c0 lst-kix_d3i63clc3lgg-1" start="2">
        <li class="c4 c15 c36 c46 li-bullet-0">
            <h2 id="h.nsa8lxrnmxkd" style="display:inline"><span>Riesgos de prueba y factores de
                    mitigaci&oacute;n</span></h2>
        </li>
    </ol><a id="t.631e0a8bdeec5841d70663f7694b22eef0646943"></a><a id="t.6"></a>
    <table class="c113 c123">
        <tr class="c44">
            <td class="c21" colspan="1" rowspan="1">
                <p class="c4"><span class="c17">ID</span></p>
            </td>
            <td class="c8" colspan="1" rowspan="1">
                <p class="c4"><span class="c17">Riesgo</span></p>
            </td>
            <td class="c96" colspan="1" rowspan="1">
                <p class="c4"><span class="c17">Descripci&oacute;n</span></p>
            </td>
            <td class="c23" colspan="1" rowspan="1">
                <p class="c4"><span class="c17">Acciones de Mitigaci&oacute;n</span></p>
            </td>
            <td class="c18" colspan="1" rowspan="1">
                <p class="c4"><span class="c17">Probabilidad</span></p>
            </td>
            <td class="c64" colspan="1" rowspan="1">
                <p class="c4"><span class="c17">Impacto</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c21" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">R_01</span></p>
            </td>
            <td class="c8" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Latencia en el acceso al GitHub </span></p>
            </td>
            <td class="c96" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Al ser Github la plataforma en la que compartimos y organizamos nuestros
                        avances, si existe alg&uacute;n error en la plataforma o si nosotros cometemos alg&uacute;n
                        error, nuestro repositorio puede perder informaci&oacute;n o perderse por completo</span></p>
            </td>
            <td class="c23" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">- Regresar a la versi&oacute;n m&aacute;s estable dentro del historial de
                        versiones </span></p>
                <p class="c4"><span class="c1">- Utilizar la versi&oacute;n de alguien del equipo que no haya </span>
                </p>
            </td>
            <td class="c18" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Media</span></p>
            </td>
            <td class="c64" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Alta</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c21" colspan="1" rowspan="1">
                <p class="c4"><span class="c5">R_02</span></p>
            </td>
            <td class="c8" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Que no se d&eacute; el presupuesto necesario para el hosting de la
                        plataforma en la nube</span></p>
            </td>
            <td class="c96" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Los servicios de cloud son costosos pero garantizan seguridad y
                        escalabilidad, se debe de llegar a un acuerdo con el Tec para el uso de estos servicios</span>
                </p>
            </td>
            <td class="c23" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">- Contar con alternativas gratuitas de respaldo o cuentas con
                        &quot;trial&quot; del servicio con suficiente alcance de tiempo para la entrega del
                        proyecto.</span></p>
                <p class="c4"><span class="c1">- Uso del servidor</span></p>
            </td>
            <td class="c18" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Media</span></p>
            </td>
            <td class="c64" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Alta</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c21" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">R_ 03</span></p>
            </td>
            <td class="c8" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Inclusi&oacute;n de nuevos miembros al equipo</span></p>
            </td>
            <td class="c96" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Debido a la naturaleza del proyecto, de 4 equipos se formar&aacute;
                        s&oacute;lo un equipo, por lo que &nbsp;la integraci&oacute;n de las ideas y los integrantes
                        puede resultar retadora</span></p>
            </td>
            <td class="c23" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">- En cuanto sea detectado, restringir el acceso por completo al
                        individuo</span></p>
                <p class="c4"><span class="c1">- Contactar a las autoridades</span></p>
                <p class="c4"><span class="c1">- Contactar al equipo legal</span></p>
            </td>
            <td class="c18" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Media</span></p>
            </td>
            <td class="c64" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Alta</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c21" colspan="1" rowspan="1">
                <p class="c4"><span class="c5">R_04</span></p>
            </td>
            <td class="c8" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Divergencia entre los distintos ambientes de desarrollo </span></p>
            </td>
            <td class="c96" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Ya que se utilizar&aacute;n diferentes librer&iacute;as y dependencias,
                        si el sistema operativo del dispositivo de alg&uacute;n integrante no es compatible con dichos
                        componentes, el desarrollo de la aplicaci&oacute;n puede retrasarse y la productividad y
                        participaci&oacute;n del integrante puede verse afectada. </span></p>
            </td>
            <td class="c23" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">- Utilizar un docker o una m&aacute;quina virtual</span></p>
                <p class="c4"><span class="c1">- Estandarizar un ambiente de desarrollo</span></p>
            </td>
            <td class="c18" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Media</span></p>
            </td>
            <td class="c64" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Media</span></p>
            </td>
        </tr>
    </table>
    <p class="c4 c12"><span class="c10"></span></p>
    <p class="c4 c12"><span class="c1"></span></p>
    <p class="c4 c12"><span class="c1"></span></p>
    <ol class="c0 lst-kix_d3i63clc3lgg-1" start="3">
        <li class="c4 c15 c36 c46 li-bullet-0">
            <h2 id="h.5h8w5mqda6gh" style="display:inline"><span>Plan de comunicaciones y lista de equipos</span></h2>
        </li>
    </ol><a id="t.113000c59697455fb59036e97da4ef320a61d27c"></a><a id="t.7"></a>
    <table class="c54">
        <tr class="c44">
            <td class="c60" colspan="1" rowspan="1">
                <p class="c4"><span class="c17">Rol</span></p>
            </td>
            <td class="c22" colspan="1" rowspan="1">
                <p class="c4"><span class="c17">Descripci&oacute;n</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c60" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Project Manager </span></p>
            </td>
            <td class="c22" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">El miembro que est&aacute; a cargo de un equipo. Deben organizar y
                        planificar las tareas del equipo para que el proyecto tenga &eacute;xito, asegur&aacute;ndose de
                        que se entreguen en tiempo, forma y retroalimentadas. </span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c60" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">L&iacute;der de Pruebas</span></p>
            </td>
            <td class="c22" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Miembro del equipo que es responsable de participar y supervisar el
                        desarrollo de las pruebas. Debe de tener en cuenta todos los alcances y criterios de
                        validaci&oacute;n de cada prueba para asegurarse de que se cumplan en tiempo y forma. </span>
                </p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c60" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">L&iacute;der de Back-End</span></p>
            </td>
            <td class="c22" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Miembro del equipo que es responsable de participar y supervisar el
                        desarrollo del back-end. Debe coordinar con todos los equipos de desarrollo el avance y los
                        componentes del proyecto, asignar tareas, asegurarse de que se completen en tiempo y forma y
                        coordinarse con el project manager.</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c60" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">L&iacute;der de Front-End</span></p>
            </td>
            <td class="c22" colspan="1" rowspan="1">
                <p class="c4"><span class="c5">Miembro del equipo que es responsable de participar y supervisar el
                        desarrollo del front-end. Debe coordinar con todos los equipos de desarrollo, el avance y los
                        componentes del proyecto, asignar tareas, asegurarse de que se completen en tiempo y forma y
                        coordinarse con el project manager.</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c60" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">L&iacute;der de Base de Datos</span></p>
            </td>
            <td class="c22" colspan="1" rowspan="1">
                <p class="c4"><span class="c5">Miembro del equipo que es responsable de participar y supervisar el
                        desarrollo de la base de datos. Debe coordinar con todos los equipos de desarrollo, el avance y
                        los componentes del proyecto, asignar tareas, asegurarse de que se completen en tiempo y forma y
                        coordinarse con el project manager.</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c60" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">L&iacute;der de Seguridad</span></p>
            </td>
            <td class="c22" colspan="1" rowspan="1">
                <p class="c4"><span class="c5">Miembro del equipo que es responsable de participar y supervisar la
                        protecci&oacute;n de los diferentes aspectos del proyecto y la autenticaci&oacute;n de los
                        usuarios. Debe coordinar con todos los equipos de desarrollo, el avance y los componentes del
                        proyecto, asignar tareas, asegurarse de que se completen en tiempo y forma y coordinarse con el
                        project manager.</span></p>
            </td>
        </tr>
        <tr class="c44">
            <td class="c60" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Equipo de Desarrollo</span></p>
            </td>
            <td class="c22" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">C&eacute;lula de trabajo encargada de requerimientos espec&iacute;ficos,
                        compuesta de un miembro de back-end, uno de front-end, uno de base de datos, uno de seguridad,
                        de pruebas y un project manager.</span></p>
            </td>
        </tr>
    </table>
    <p class="c4 c12"><span class="c1"></span></p>
    <h3 class="c4 c79" id="h.shiwdz2v0drx"><span>Expectativas del Rol </span></h3>
    <p class="c30 c74"><span class="c1">Es importante aclarar que dentro del proyecto presente, todos los involucrados
            en el desarrollo de la aplicaci&oacute;n cumpliran un rol como tester a pesar de las responsabilidades que
            tengan en otro rol. Por lo antes mencionado, por cada componente que sea finalizado por cualquier persona en
            el equipo de desarrollo se realizar&aacute; una prueba informal. De la misma manera, todo el equipo de
            desarrollo tiene como responsabilidad validar con el cliente los componentes de la aplicaci&oacute;n y el
            entregable final.</span></p>
    <p class="c30 c74 c12"><span class="c1"></span></p>
    <p class="c30 c74"><span class="c1">La siguiente lista define en t&eacute;rminos generales las expectativas
            relacionadas a los roles que est&aacute;n involucrados con el manejo, planeaci&oacute;n o ejecuci&oacute;n
            de la prueba para el proyecto. </span></p>
    <p class="c30 c74 c12"><span class="c1"></span></p>
    <h3 class="c4 c67" id="h.vajm4pu401qs"><span class="c87">Project Manag</span><span>er </span></h3>
    <p class="c4 c68"><span class="c5">R</span><span class="c1">evisa el contenido de</span><span class="c1">l plan de
            pruebas, la estrategia de las pueblas, los estimados, criterios de validaci&oacute;n con los equipos de
            trabajo, l&iacute;deres y los stakeholders. Recopila la retroalimentaci&oacute;n e informa a los
            dem&aacute;s. Tiene la responsabilidad de darle acompa&ntilde;amiento a las pruebas de caja blanca.</span>
    </p>
    <p class="c4 c12 c68"><span class="c1"></span></p>
    <h3 class="c4 c67" id="h.cup1cc33x1cr"><span class="c35">L&iacute;der de Pruebas </span></h3>
    <p class="c30 c68"><span class="c1">Junto con el project manager, crea y revisa el contenido del plan de pruebas, la
            estrategia de las pueblas, los estimados y criterios de validaci&oacute;n coordinando la ejecuci&oacute;n
            con las actividades programadas en el cronograma del proyecto. Recibe retroalimentaci&oacute;n de los
            equipos de trabajo, l&iacute;deres y los stakeholders, se asegura que las pruebas se ejecuten en tiempo y
            forma y documenta el proceso y los resultados.</span></p>
    <p class="c4 c12 c68"><span class="c1"></span></p>
    <h3 class="c4 c67" id="h.15iz1ry18o"><span class="c35">L&iacute;der de Back-End </span></h3>
    <p class="c30 c68"><span class="c5">Junto con el l&iacute;der de pruebas y el project manager, suma al contenido del
            plan de pruebas considerando las actividades programadas para el desarrollo del back-end, el avance del
            mismo y se asegura de la ejecuci&oacute;n de las pruebas de sus componentes y que la integraci&oacute;n con
            los otros equipos sea probada y documentada. Se le asignan pruebas, es parte y </span><span
            class="c5">delega</span><span class="c1">&nbsp;dichas pruebas y se asegura que las funcionalidades
            cr&iacute;ticas de su desarrollo sean consideradas como parte del plan de pruebas. Tiene un seguimiento de
            las pruebas informales que sus desarrolladores han ejecutado. </span></p>
    <p class="c4 c12 c68"><span class="c1"></span></p>
    <p class="c4 c68"><span class="c5">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span
            class="c35">L&iacute;der de Front-End </span></p>
    <p class="c30 c68"><span class="c5">Junto con el l&iacute;der de pruebas y el project manager, suma al contenido del
            plan de pruebas considerando las actividades programadas para el desarrollo del front-end, el avance del
            mismo y se asegura de la ejecuci&oacute;n de las pruebas de sus componentes y que la integraci&oacute;n con
            los otros equipos sea probada y documentada. Se le asignan pruebas, es parte y </span><span
            class="c5">delega</span><span class="c1">&nbsp;dichas pruebas y se asegura que las funcionalidades
            cr&iacute;ticas de su desarrollo sean consideradas como parte del plan de pruebas. Tiene un seguimiento de
            las pruebas informales que sus desarrolladores han ejecutado. </span></p>
    <p class="c4 c12 c68"><span class="c1"></span></p>
    <p class="c4 c9"><span class="c35">L&iacute;der de Base de Datos </span></p>
    <p class="c30 c68"><span class="c5">Junto con el l&iacute;der de pruebas y el project manager, suma al contenido del
            plan de pruebas considerando las actividades programadas para el desarrollo de la base de datos, el avance
            de la misma y se asegura de la ejecuci&oacute;n de las pruebas de sus componentes y que la
            integraci&oacute;n con los otros equipos sea probada y documentada. Se le asignan pruebas, es parte y
        </span><span class="c5">delega</span><span class="c1">&nbsp;dichas pruebas y se asegura que las funcionalidades
            cr&iacute;ticas de su desarrollo sean consideradas como parte del plan de pruebas. Tiene un seguimiento de
            las pruebas informales que sus desarrolladores han ejecutado. </span></p>
    <p class="c4 c12 c68"><span class="c1"></span></p>
    <p class="c4 c9"><span class="c35">L&iacute;der de Seguridad </span></p>
    <p class="c4 c68"><span class="c5">Junto con el l&iacute;der de pruebas y el project manager, suma al contenido del
            plan de pruebas considerando las actividades programadas para la protecci&oacute;n de los diferentes
            aspectos del proyecto y la autenticaci&oacute;n de los usuarios, y se asegura de la ejecuci&oacute;n de las
            pruebas de sus componentes y que la integraci&oacute;n con los otros equipos sea probada y documentada. Se
            le asignan pruebas, es parte y </span><span class="c5">delega</span><span class="c1">&nbsp;dichas pruebas y
            se asegura que las funcionalidades cr&iacute;ticas de su desarrollo sean consideradas como parte del plan de
            pruebas. Tiene un seguimiento de las pruebas informales que sus desarrolladores han ejecutado.</span></p>
    <p class="c4 c12 c68"><span class="c1"></span></p>
    <p class="c4 c9"><span class="c35">Equipo de Desarrollo</span></p>
    <p class="c4 c68"><span class="c5">Junto con sus respectivos l&iacute;deres ejecutan las diferentes pruebas
            establecidas en el plan y se aseguran de que estas sean ejecutadas en el mismo ambiente siguiendo la
            metodolog&iacute;a. Proveen y dan seguimiento a la retroalimentaci&oacute;n y documentan el proceso y los
            resultados, as&iacute; garantizando un proceso de QA transparente. Informan a los l&iacute;deres si existe
            alg&uacute;n problema o si alg&uacute;n componente necesita ser corregido, se encargan de hacer las pruebas
            en tiempo y forma (de acuerdo al cronograma), llevan un seguimiento de sus pruebas informales y corrigen sus
            funcionalidades. Cada integrante del desarrollo tiene la responsabilidad de realizar sus pruebas asignadas
            de caja negra y junto con el SCRUM Master y el Project Manager realizar las pruebas de caja blanca. </span>
    </p>
    <p class="c4 c12 c93"><span class="c1"></span></p>
    <h3 class="c4 c79" id="h.bpgnszel0u1j"><span class="c35">Cronograma de Actividades</span></h3>
    <p class="c58 c36"><span class="c99"><a class="c14"
                href="https://www.google.com/url?q=https://tec95061.monday.com/boards/4072044099/views/92404971&amp;sa=D&amp;source=editors&amp;ust=1678847025926092&amp;usg=AOvVaw3EsjH0JCBD454MFd_59uUm">Gantt
                (Monday.com)</a></span></p>
    <p class="c4 c12 c109"><span class="c52 c87 c91"></span></p>
    <ol class="c0 lst-kix_d3i63clc3lgg-0" start="4">
        <li class="c4 c38 li-bullet-0">
            <h1 id="h.6ngo7ertvrlx" style="display:inline"><span class="c100">Ambiente de pruebas</span></h1>
        </li>
    </ol>
    <ul class="c0 lst-kix_6tpu3jq5w4b9-0 start">
        <li class="c4 c51 c46 li-bullet-0"><span class="c1">El entorno de prueba consistir&aacute; en un entorno de
                Windows 11 como m&iacute;nimo, un n&uacute;cleo Intel i5 o equivalente; 8 GB de RAM.</span></li>
        <li class="c4 c46 c51 li-bullet-0"><span class="c1">Se utilizar&aacute;n los servicios de AWS, donde se busca
                alojar la aplicaci&oacute;n web y la base de datos. </span></li>
        <li class="c4 c51 c46 li-bullet-0"><span class="c1">Todos los testers trabajaran en la misma versi&oacute;n de
                la aplicaci&oacute;n y base de datos y tendr&aacute;n las mismas versiones del software utilizado
                (incluyendo las librer&iacute;as y dependencias).</span></li>
        <li class="c4 c51 c46 li-bullet-0"><span class="c5">En caso de ser necesario se usar&aacute; docker para poder
                ejecutar las pruebas y estandarizar el ambiente de trabajo.</span></li>
    </ul>
    <p class="c4 c51 c12"><span class="c1 c50"></span></p>
    <ol class="c0 lst-kix_d3i63clc3lgg-0" start="5">
        <li class="c4 c38 li-bullet-0">
            <h1 id="h.e0bh1ws8hyem" style="display:inline"><span>Pruebas</span><sup><a href="#cmnt12"
                        id="cmnt_ref12">[l]</a></sup></h1>
        </li>
    </ol>
    <p class="c58 c36 c69"><span class="c50">Esto se llenar&aacute; con en la fase de despliegue de la unidad de
            formaci&oacute;n &ldquo;CLAVE DE MATERIA&rdquo;</span></p>
    <ol class="c0 lst-kix_d3i63clc3lgg-0" start="6">
        <li class="c4 c38 li-bullet-0">
            <h1 id="h.j9dbb7pex1fz" style="display:inline"><span>Conclusiones</span></h1>
        </li>
    </ol>
    <p class="c30 c85"><span class="c1">En conclusi&oacute;n, la aplicaci&oacute;n de un plan de pruebas exhaustivo es
            esencial para el &eacute;xito del proyecto, sobre todo al tratarse de desarrollo de software. Esto ya que
            las pruebas continuas y sistematizadas &nbsp;permiten identificar as&iacute; como abordar posibles problemas
            emergentes antes de que se conviertan en riesgos &nbsp;mayores. Con acceso al documento del plan de pruebas,
            los miembros del equipo tendr&aacute;n una comprensi&oacute;n clara de los requisitos y expectativas del
            proyecto, que puede servir de gu&iacute;a para la toma de decisiones y la resoluci&oacute;n de
            problemas.</span></p>
    <p class="c30 c85"><span class="c1">El compromiso tanto del equipo de pruebas como de los desarrolladores, es
            crucial para la aplicaci&oacute;n eficaz de este plan de pruebas. La adhesi&oacute;n a los contenidos
            acordados del documento garantiza que todos est&eacute;n en la misma p&aacute;gina y trabajen por el mismo
            objetivo, as&iacute; facilitando un desarrollo fluido y el cumplimiento de los planes elaborados antes de la
            implantaci&oacute;n.</span></p>
    <p class="c30 c85"><span class="c1">Asimismo, el plan de pruebas puede ayudar al equipo a evaluar y mejorar el
            rendimiento general del proyecto. Mediante el seguimiento del progreso y la identificaci&oacute;n de
            &aacute;reas de mejora, el equipo puede perfeccionar el plan del proyecto, optimizar los recursos y mejorar
            la eficiencia general del proyecto. En t&eacute;rminos generales, la aplicaci&oacute;n de un plan de pruebas
            exhaustivo es esencial para el &eacute;xito de cualquier proyecto. Con pruebas continuas, directrices claras
            y el compromiso de los miembros del equipo, el proyecto puede entregarse a tiempo, dentro del presupuesto y
            con la calidad esperada.</span></p>
    <div>
        <p class="c36 c12 c105"><span class="c37"></span></p>
    </div>
    <div class="c16">
        <p class="c28"><a href="#cmnt_ref1" id="cmnt1">[a]</a><span class="c25">En esto tenemos que agregar lo de que
                las pruebas unitarias son para los desarrolladores, etc</span></p>
    </div>
    <div class="c16">
        <p class="c28"><a href="#cmnt_ref2" id="cmnt2">[b]</a><span class="c25">ya complete la descripci&oacute;n leanla
                si quieren jeje</span></p>
    </div>
    <div class="c16">
        <p class="c28"><a href="#cmnt_ref3" id="cmnt3">[c]</a><span class="c25">se ve bien&nbsp;&#x1f44d;</span></p>
    </div>
    <div class="c16">
        <p class="c28"><a href="#cmnt_ref4" id="cmnt4">[d]</a><span class="c25">agregar en la descripci&oacute;n</span>
        </p>
    </div>
    <div class="c16">
        <p class="c28"><a href="#cmnt_ref5" id="cmnt5">[e]</a><span class="c25">agregar descripci&oacute;n</span></p>
    </div>
    <div class="c16">
        <p class="c28"><a href="#cmnt_ref6" id="cmnt6">[f]</a><span class="c25">Camino basico o cobertura</span></p>
    </div>
    <div class="c16">
        <p class="c28"><a href="#cmnt_ref7" id="cmnt7">[g]</a><span class="c25">ya puse lo de cobertura</span></p>
    </div>
    <div class="c16">
        <p class="c28"><a href="#cmnt_ref8" id="cmnt8">[h]</a><span class="c25">agregar descripcion</span></p>
    </div>
    <div class="c16">
        <p class="c28"><a href="#cmnt_ref9" id="cmnt9">[i]</a><span class="c25">aceptacion desarrolladores con ruben
                raya</span></p>
        <p class="c28"><span class="c25">validacion otro salon, esteban, ruben raya</span></p>
    </div>
    <div class="c16">
        <p class="c28"><a href="#cmnt_ref10" id="cmnt10">[j]</a><span class="c25">agregar pruebas informales</span></p>
    </div>
    <div class="c16">
        <p class="c28"><a href="#cmnt_ref11" id="cmnt11">[k]</a><span class="c25">andreina</span></p>
    </div>
    <div class="c16">
        <p class="c28"><a href="#cmnt_ref12" id="cmnt12">[l]</a><span class="c25">esto tambien lo dejaron
                vac&iacute;o</span></p>
    </div>
</body>

</html>
