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
    <p class="c23"><span class="c112 c62"><a class="c14" href="#h.mx6gxsm2t7jg">1.
                Introducci&oacute;n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3</a></span></p>
    <p class="c23 c36"><span class="c42"><a class="c14" href="#h.4jat4228tqo5">1.1.
                Prop&oacute;sito&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3</a></span></p>
    <p class="c23 c36"><span class="c42"><a class="c14" href="#h.2w8d162qwulj">1.2.
                Audiencia&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3</a></span></p>
    <p class="c23"><span class="c62 c112"><a class="c14" href="#h.kvw8q2v7aqxc">2. Estrategia de
                pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4</a></span></p>
    <p class="c23 c36"><span class="c42"><a class="c14" href="#h.gbeixwb2ake5">2.1. Descripci&oacute;n de
                pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4</a></span></p>
    <p class="c23 c36"><span class="c42"><a class="c14" href="#h.qpfdlx4dm8zo">2.2. Objetivo de las
                pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6</a></span></p>
    <p class="c23 c36"><span class="c42"><a class="c14" href="#h.z6088tyel1xj">2.3. Suposiciones de las
                pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;7</a></span></p>
    <p class="c23 c36"><span class="c42"><a class="c14" href="#h.ja9xqids1cyt">2.4. Objetivos de las
                pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;8</a></span></p>
    <p class="c23 c36"><span class="c42"><a class="c14" href="#h.j8zy2j5g5i1t">2.5.
                Alcance&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;11</a></span></p>
    <p class="c23 c36"><span class="c42"><a class="c14" href="#h.h904v6h0rrrr">2.6. Niveles de
                pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;18</a></span></p>
    <p class="c23 c89"><span class="c42"><a class="c14" href="#h.91fzm9dtgvmr">Prueba de Caja Blanca (Prueba
                Funcional)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;19</a></span></p>
    <p class="c23 c89"><span class="c42"><a class="c14" href="#h.xhc6264rls1i">Prueba de Integraci&oacute;n (Prueba
                Funcional)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;19</a></span></p>
    <p class="c23 c89"><span class="c42"><a class="c14" href="#h.j8epsprogp2p">Prueba de Aceptaci&oacute;n (Prueba
                Funcional)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;20</a></span></p>
    <p class="c23 c89"><span class="c32"><a class="c14" href="#h.qsyst13rz67j">Prueba de Recorrido Est&aacute;tico
                (Validaci&oacute;n)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;20</a></span></p>
    <p class="c23 c36"><span class="c42"><a class="c14" href="#h.cwh2skhwocng">2.7. Criterios de aceptaci&oacute;n de
                pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;21</a></span></p>
    <p class="c23 c89"><span class="c32"><a class="c14" href="#h.j39ka7pd5nwf">Pruebas
                Informales&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;21</a></span></p>
    <p class="c23 c89"><span class="c42"><a class="c14" href="#h.fsv2ynwal6n0">Pruebas
                Unitarias&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;21</a></span></p>
    <p class="c23 c89"><span class="c42"><a class="c14" href="#h.kzej3b9e4wfe">Prueba de
                Integraci&oacute;n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;25</a></span></p>
    <p class="c23 c89"><span class="c42"><a class="c14" href="#h.ns3vrtfyjguc">Prueba de
                Validaci&oacute;n/Aceptaci&oacute;n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;26</a></span></p>
    <p class="c23 c89"><span class="c42"><a class="c14" href="#h.7krppuwc58yf">Pruebas Est&aacute;ticas de
                Recorrido&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;26</a></span></p>
    <p class="c23 c36"><span class="c42"><a class="c14" href="#h.s6ntvdjxs5wr">2.8. Entregables de
                pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;26</a></span></p>
    <p class="c23 c36"><span class="c42"><a class="c14" href="#h.vqt91vksszs0">2.9. Lista de
                hitos&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;27</a></span></p>
    <p class="c23 c36"><span class="c42"><a class="c14" href="#h.tttcgn6nmo2n">2.10. Estimaci&oacute;n de esfuerzo de
                las pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;32</a></span></p>
    <p class="c23"><span class="c112 c62"><a class="c14" href="#h.rggsbldjdzgj">3. Proceso de gesti&oacute;n de
                pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;32</a></span></p>
    <p class="c23 c36"><span class="c42"><a class="c14" href="#h.l5voq2cnpp4q">3.1. Proceso de ejecuci&oacute;n de
                pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;32</a></span></p>
    <p class="c23 c36"><span class="c42"><a class="c14" href="#h.nsa8lxrnmxkd">3.2. Riesgos de prueba y factores de
                mitigaci&oacute;n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;33</a></span></p>
    <p class="c23 c36"><span class="c42"><a class="c14" href="#h.5h8w5mqda6gh">3.3. Plan de comunicaciones y lista de
                equipos&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;35</a></span></p>
    <p class="c23 c89"><span class="c42"><a class="c14" href="#h.shiwdz2v0drx">Expectativas del
                Rol&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;36</a></span></p>
    <p class="c23 c89"><span class="c42"><a class="c14" href="#h.vajm4pu401qs">Project
                Manager&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;36</a></span></p>
    <p class="c23 c89"><span class="c42"><a class="c14" href="#h.cup1cc33x1cr">L&iacute;der de
                Pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;37</a></span></p>
    <p class="c23 c89"><span class="c42"><a class="c14" href="#h.15iz1ry18o">L&iacute;der de
                Back-End&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;37</a></span></p>
    <p class="c23 c89"><span class="c42"><a class="c14" href="#h.bpgnszel0u1j">Cronograma de
                Actividades&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;38</a></span></p>
    <p class="c23"><span class="c112 c62"><a class="c14" href="#h.6ngo7ertvrlx">4. Ambiente de
                pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;39</a></span></p>
    <p class="c23"><span class="c112 c62"><a class="c14" href="#h.e0bh1ws8hyem">5.
                Pruebas&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;39</a></span></p>
    <p class="c23"><span class="c112 c62"><a class="c14" href="#h.j9dbb7pex1fz">6.
                Conclusiones&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;39</a></span></p>
    <p class="c6"><span class="c18"></span></p>
    <p class="c6 c150"><span class="c18"></span></p>
    <p class="c6"><span class="c1"></span></p>
    <ol class="c3 lst-kix_d3i63clc3lgg-0 start" start="1">
        <li class="c7 c49 li-bullet-0">
            <h1 id="h.mx6gxsm2t7jg" style="display:inline"><span class="c31">Introducci&oacute;n</span></h1>
        </li>
    </ol>
    <ol class="c3 lst-kix_d3i63clc3lgg-1 start" start="1">
        <li class="c7 c24 li-bullet-0">
            <h2 id="h.4jat4228tqo5" style="display:inline"><span class="c16">Prop&oacute;sito</span></h2>
        </li>
    </ol>
    <p class="c7 c77"><span class="c1">El documento presente tiene el objetivo de describir el programa de pruebas que
            se realizar&aacute; durante el desarrollo del proyecto con NDS; una plataforma para la venta de
            autom&oacute;viles en l&iacute;nea. En particular, este documento contendr&aacute;:</span></p>
    <ol class="c3 lst-kix_xdqyscxb1zsk-0 start" start="1">
        <li class="c7 c30 li-bullet-0"><span class="c1">La estrategia y objetivos de las pruebas a realizarse en cada
                uno de los componentes de la aplicaci&oacute;n.</span></li>
        <li class="c7 c30 li-bullet-0"><span class="c1">Una justificaci&oacute;n acerca de las pruebas
                seleccionadas.</span></li>
        <li class="c7 c30 li-bullet-0"><span class="c1">Los criterios de validaci&oacute;n para los componentes de la
                aplicaci&oacute;n y los criterios de aceptaci&oacute;n de cada una de las pruebas.</span></li>
        <li class="c7 c30 li-bullet-0"><span class="c1">El plan de ejecuci&oacute;n de las pruebas a realizarse, al
                igual que el plan de remediaci&oacute;n &nbsp;en caso de que una de estas pruebas termine con un
                resultado negativo.</span></li>
        <li class="c7 c30 li-bullet-0"><span class="c1">Las responsabilidades de los integrantes del equipo en
                relaci&oacute;n a las pruebas.</span></li>
        <li class="c7 c30 li-bullet-0"><span class="c1">Una descripci&oacute;n del ambiente, al igual que las
                herramientas &nbsp;herramientas que ser&aacute;n utilizadas para las pruebas.</span></li>
    </ol>
    <p class="c6 c108"><span class="c1"></span></p>
    <ol class="c3 lst-kix_d3i63clc3lgg-1" start="2">
        <li class="c7 c24 li-bullet-0">
            <h2 id="h.2w8d162qwulj" style="display:inline"><span class="c155">Audiencia</span><span
                    class="c86">&nbsp;</span></h2>
        </li>
    </ol>
    <p class="c7 c66 c89"><span class="c1">En esta secci&oacute;n se encuentra la descripci&oacute;n detallada de la
            audiencia a la que se dirige el presente escrito: &nbsp;</span></p>
    <ol class="c3 lst-kix_notb3jec8k49-0 start" start="1">
        <li class="c7 c20 li-bullet-0"><span class="c1">El siguiente documento est&aacute; dise&ntilde;ado para ser
                consultado principalmente por los miembros del equipo de desarrollo del proyecto, profesores
                responsables del mismo, el cliente (NDS) y sus representantes.</span></li>
    </ol>
    <ol class="c3 lst-kix_notb3jec8k49-1 start" start="1">
        <li class="c25 c7 li-bullet-0"><span class="c1">Las pruebas funcionales o din&aacute;micas est&aacute;n
                orientadas a la compresi&oacute;n de los desarrolladores y del Project Manager.</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c8">Las pruebas est&aacute;ticas est&aacute;n dise&ntilde;adas para
                ser entendidas no solo por el equipo de desarrollo, sino tambi&eacute;n por cualquier persona fuera del
                &aacute;rea de tecnolog&iacute;a. </span></li>
    </ol>
    <ol class="c3 lst-kix_notb3jec8k49-0" start="2">
        <li class="c7 c20 li-bullet-0"><span class="c1">&nbsp;El director del proyecto es responsable de utilizar el
                documento para garantizar que se sigue el calendario de pruebas acordado y que se supervisa el progreso
                de acuerdo con las instrucciones del documento. Asimismo, esta figura es responsable de los resultados y
                el rendimiento de cada prueba.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">El cliente (NDS), las partes interesadas o sus representantes
                tienen la opci&oacute;n de revisar el documento para verificar que el desarrollo se ajusta a sus
                requisitos e intereses.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">El equipo de desarrollo se encarga de garantizar que el plan de
                pruebas y los resultados especificados en el documento son coherentes con lo acordado durante la fase de
                dise&ntilde;o.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">&nbsp;El equipo de desarrollo es responsable de resolver
                cualquier prueba fallida se&ntilde;alada en el documento.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Otros miembros del equipo y las partes interesadas
                tambi&eacute;n pueden utilizar el documento como punto de referencia en todo momento para diversos
                asuntos relacionados con el proyecto.</span></li>
    </ol>
    <p class="c2 c17"><span class="c1"></span></p>
    <ol class="c3 lst-kix_d3i63clc3lgg-0" start="2">
        <li class="c7 c94 c80 c89 li-bullet-0">
            <h1 id="h.kvw8q2v7aqxc" style="display:inline"><span class="c31">Estrategia de pruebas </span></h1>
        </li>
    </ol>
    <ol class="c3 lst-kix_d3i63clc3lgg-1 start" start="1">
        <li class="c7 c24 li-bullet-0">
            <h2 id="h.gbeixwb2ake5" style="display:inline"><span>Descripci&oacute;n de pruebas</span></h2>
        </li>
    </ol>
    <p class="c7 c88"><span class="c1">En el presente apartado se describe a profundidad la estrategia de pruebas que se
            seguir&aacute; durante el proceso de desarrollo de la plataforma web para el cliente NDS.</span></p>
    <p class="c6 c127"><span class="c1"></span></p>
    <p class="c38"><span class="c47">Etapa 1 &ndash; Comprensi&oacute;n de los Requerimientos, Especificaciones del
            Proyecto y Pruebas Est&aacute;ticas:</span><span class="c1">&nbsp;Antes de crear una estrategia de pruebas,
            primero se comprenden y establecen de manera detallada los requerimientos del proyecto. Para ello se tiene
            una serie de interacciones semanales con el cliente NDS en el cual se documentan de forma clara las
            caracter&iacute;sticas de la soluci&oacute;n que cumplen con sus necesidades y objetivos. Al finalizar esta
            etapa se espera que haya pocos o nulos cambios, ya que el resto del proyecto se desarrollar&aacute; en base
            a lo establecido en esta etapa, por lo cu&aacute;l queda fuera de las etapas de iteraci&oacute;n. </span>
    </p>
    <p class="c38 c17"><span class="c18"></span></p>
    <p class="c38"><span class="c47">Etapa 2 - Pruebas </span><span class="c47">Informales</span><span class="c47">:
        </span><span class="c1">En un principio, se comenzar&aacute; realizando pruebas informales durante el desarrollo
            del software. Esto incluir&iacute;a pruebas realizadas individualmente por cada uno de los desarrolladores
            sin supervisi&oacute;n, teniendo un enfoque en comprobar la funcionalidad de componentes creados. En esta
            etapa comienza el proceso iterativo de las pruebas y va dentro de las pruebas din&aacute;micas. </span></p>
    <p class="c38 c17"><span class="c18"></span></p>
    <p class="c38"><span class="c47">Etapa 3 &ndash; Realizaci&oacute;n de Pruebas Unitarias:</span><span
            class="c1">&nbsp;Esta etapa tambi&eacute;n va dentro de las pruebas din&aacute;micas y se pretende comenzar
            realizando las pruebas unitarias para cada componente de software de la plataforma. Esto
            concentr&aacute;ndose en pruebas de caja negra (black box tests) tomando especial atenci&oacute;n en la
            entrada y salida esperadas en su correcto funcionamiento. Simult&aacute;neamente a esto, se acordar&aacute;
            de manera iterativa con NDS las pruebas de historias de usuario van de acuerdo a sus criterios de
            aceptaci&oacute;n. Esto ayudar&aacute; a garantizar que la p&aacute;gina web satisfaga correctamente las
            necesidades de NDS y de sus clientes.</span></p>
    <p class="c38 c17"><span class="c1"></span></p>
    <p class="c38"><span class="c47">Etapa 4 </span><span class="c47">- Pruebas de Caja Blanca de cobertura (White Box
            Testing):</span><span class="c1">&nbsp;En esta etapa, que tambi&eacute;n va dentro de las din&aacute;micas,
            se realizan las pruebas de caja blanca a los componentes definidos en este documento, especialmente dando
            prioridad a aquellos componentes que generaron errores en las Pruebas de Caja Negra. De esta manera, se
            podr&aacute; analizar el c&oacute;digo de dichos componentes, as&iacute; permitiendo arreglar errores
            persistentes en pruebas anteriores o eliminar redundancias. </span></p>
    <p class="c38"><span class="c1">Para hacer m&aacute;s eficaz nuestro proceso de pruebas de caja blanca, usaremos la
            t&eacute;cnica de cobertura en donde se probaran los caminos m&aacute;s utilizados para hacer uso de cada
            funci&oacute;n de cada tipo de usuario. </span></p>
    <p class="c38 c17"><span class="c1"></span></p>
    <p class="c38"><span class="c47">Etapa 5 - Pruebas de Integraci&oacute;n:</span><span class="c1">&nbsp;En esta
            etapa, que es la &uacute;ltima dentro de las etapas din&aacute;micas, despu&eacute;s de que todas las
            pruebas unitarias hayan pasado con &eacute;xito se pasan a las pruebas de integraci&oacute;n donde de manera
            ascendente se van uniendo los diferentes componentes para validar su correcto funcionamiento en conjunto.
            Las pruebas de integraci&oacute;n se llevar&aacute;n a cabo mediante pruebas de caja negra de casos de uso
            aleatorias, las cuales ser&aacute;n elegidas y supervisadas por el Project Manager responsable del equipo de
            desarrollo.</span></p>
    <p class="c38 c17"><span class="c18"></span></p>
    <p class="c38"><span class="c47">Etapa 6 &ndash; Pruebas de Validaci&oacute;n/Aceptaci&oacute;n:</span><span
            class="c1">&nbsp;En esta etapa, se requiere que haya pocos o ning&uacute;n cambio, ya qu&eacute;,
            despu&eacute;s de que las pruebas de integraci&oacute;n hayan sido exitosas se realizan las pruebas de
            validaci&oacute;n en las que se revisar&aacute; con el cliente NDS que los criterios de validaci&oacute;n
            definidos en etapas anteriores se cumplen hasta el momento del proceso de pruebas.</span></p>
    <p class="c38 c17"><span class="c1"></span></p>
    <p class="c38"><span class="c47">Etapa 7 &ndash; Pruebas de </span><span class="c47">Est&aacute;tica de
            Recorridos</span><span class="c47">: </span><span class="c1">Una vez que se haya tenido la aprobaci&oacute;n
            de NDS se realizar&aacute; la prueba del funcionamiento del sistema como un todo, verificando el
            comportamiento y correcto funcionamiento de toda la plataforma en el nivel m&aacute;s alto posible.</span>
    </p>
    <p class="c38 c17"><span class="c1"></span></p>
    <p class="c38"><span class="c47">Etapa 8 - Manual de Usuario:</span><span class="c47">&nbsp;</span><span
            class="c8">En esta etapa final, una vez que se haya completado las etapas anteriores y son pocos o nulos los
            cambios se crea el manual de usuario en el que se le proveer&aacute; informaci&oacute;n e instrucciones al
            usuario de c&oacute;mo usar el software desarrollado. En el manual de usuario se incluir&aacute;n los
            caminos previamente establecidos en las pruebas de caja blanca de cobertura. El manual toma en cuenta la
            versi&oacute;n m&aacute;s actualizada y funcional de la aplicaci&oacute;n.</span></p>
    <p class="c38 c17"><span class="c18"></span></p>
    <p class="c38"><span class="c1">Es relevante mencionar, que en esta estrategia se mantiene un flujo iterativo, donde
            de ser necesario se actualizar&aacute; el documento de pruebas o se podr&aacute; regresar a etapas de
            pruebas anteriores para as&iacute; solucionar cualquier fallo o error en cualquier nivel de la
            plataforma.</span></p>
    <p class="c6 c127 c156"><span class="c1"></span></p>
    <ol class="c3 lst-kix_d3i63clc3lgg-1" start="2">
        <li class="c7 c24 li-bullet-0">
            <h2 id="h.qpfdlx4dm8zo" style="display:inline"><span>Objetivo de las pruebas</span></h2>
        </li>
    </ol>
    <p class="c7 c146"><span class="c8">El objetivo de las pruebas que se realizar&aacute;n durante el transcurso del
            proyecto es la validaci&oacute;n de las funcionalidades fundamentales de la aplicaci&oacute;n, al igual que
            comprobar la correcta implementaci&oacute;n de los requerimientos establecidos en el documento</span><span
            class="c123 c8"><a class="c14"
                href="https://www.google.com/url?q=https://github.com/MateoHerrera0/HUMANIT/blob/main/src/wiki/SRS.md&amp;sa=D&amp;source=editors&amp;ust=1678937539941871&amp;usg=AOvVaw2XeLn6StlJEy3x6-15GyXn">&nbsp;</a></span><span
            class="c123 c8"><a class="c14"
                href="https://www.google.com/url?q=https://github.com/MateoHerrera0/HUMANIT/blob/main/src/wiki/SRS.md&amp;sa=D&amp;source=editors&amp;ust=1678937539942191&amp;usg=AOvVaw0MftLTXnJqrLidqEqn8l_A">SRS</a></span><span
            class="c1">. En consideraci&oacute;n de este objetivo, las pruebas a realizarse comprender&aacute;n:</span>
    </p>
    <ul class="c3 lst-kix_1ymfzvnh8b2w-0 start">
        <li class="c7 c29 li-bullet-0"><span class="c1">Pruebas que aseguren la correcta autorizaci&oacute;n de
                usuarios, al igual que la asignaci&oacute;n de los premios asociados.</span></li>
        <li class="c7 c29 li-bullet-0"><span class="c1">Pruebas que comprueben el correcto funcionamiento en la
                b&uacute;squeda y filtrado del cat&aacute;logo de autos.</span></li>
        <li class="c7 c29 li-bullet-0"><span class="c1">Pruebas que comprueben el correcto funcionamiento del guardado
                de autom&oacute;viles en la base de datos.</span></li>
        <li class="c7 c29 li-bullet-0"><span class="c1">Pruebas que garanticen el funcionamiento de la
                recopilaci&oacute;n, an&aacute;lisis, y generaci&oacute;n de estad&iacute;stica relacionada con usuarios
                agentes de la aplicaci&oacute;n.</span></li>
        <li class="c7 c29 li-bullet-0"><span class="c1">Pruebas relacionadas al servicio de chat implementado en la
                aplicaci&oacute;n.</span></li>
        <li class="c7 c29 li-bullet-0"><span class="c1">Pruebas con el objetivo de comprobar el correcto funcionamiento
                del proceso de compra de un autom&oacute;vil.</span></li>
        <li class="c7 c29 li-bullet-0"><span class="c1">Pruebas asociadas a la creaci&oacute;n de usuarios con
                diferentes permisos. </span></li>
        <li class="c7 c29 li-bullet-0"><span class="c8">Pruebas asociadas al funcionamiento de un software estable y
                listo para producci&oacute;n.</span></li>
    </ul>
    <ol class="c3 lst-kix_d3i63clc3lgg-1 start" start="1">
        <li class="c7 c24 li-bullet-0">
            <h2 id="h.z6088tyel1xj" style="display:inline"><span>Suposiciones de las pruebas</span></h2>
        </li>
    </ol>
    <p class="c7 c79"><span class="c47">Suposiciones clave</span></p>
    <ol class="c3 lst-kix_2ppqn3k0um83-0 start" start="1">
        <li class="c7 c30 c61 li-bullet-0"><span class="c8">Se dar&aacute; prioridad a las pruebas funcionales debido a
                limitantes de tiempo y presupuesto</span><span class="c1">. </span></li>
        <li class="c7 c30 c147 li-bullet-0"><span class="c8">Todas las pruebas se har&aacute;n en el mismo
                ambiente.</span></li>
        <li class="c7 c30 li-bullet-0"><span class="c8">Todas las pruebas se har&aacute;n inicialmente con pruebas
                Informales y posteriormente en Caja Negra.</span></li>
    </ol>
    <p class="c7 c79"><span class="c47">Suposiciones g</span><span class="c18">eneral</span><span class="c47">es</span>
    </p>
    <ol class="c3 lst-kix_vmd3n8uqgg1o-0 start" start="1">
        <li class="c7 c30 li-bullet-0"><span class="c8">Las pruebas funcionales ser&aacute;n las m&aacute;s relevantes
                del plan de pruebas.</span></li>
        <li class="c7 c30 li-bullet-0"><span class="c1">Realizar las mismas pruebas conlleva a los mismos
                resultados.</span></li>
        <li class="c7 c30 li-bullet-0"><span class="c1">Las pruebas con variedad en el rol de acceso no son
                equivalentes, y debe definirse una prueba por cada rol</span></li>
        <li class="c7 c30 c95 li-bullet-0"><span class="c8">Si el ambiente de pruebas deja de estar disponible; el
                equipo de pruebas crear&aacute; uno lo m&aacute;s similar lo antes posible.</span></li>
        <li class="c7 c30 li-bullet-0"><span class="c8">Todas las funciones han sido probadas meticulosamente.</span>
        </li>
        <li class="c7 c30 c59 li-bullet-0"><span class="c8">Las pruebas de caja blanca y pruebas paso a paso solo se
                ejecutar&aacute;n si los resultados son distintos a lo esperado</span><span class="c1">.</span></li>
        <li class="c7 c30 c147 li-bullet-0"><span class="c8">El equipo de pruebas documentar&aacute; sus resultados de
                acuerdo a lo evaluado.</span></li>
        <li class="c7 c30 c88 li-bullet-0"><span class="c1">El equipo de pruebas asume que tod</span><span class="c8">as
                las entradas o inputs requeridos durante el dise&ntilde;o y la ejecuci&oacute;n de las pruebas
                estar&aacute;n apoyados por el desarrollador/analista </span><span
                class="c8">respectivamente</span><span class="c8">. </span></li>
        <li class="c7 c30 li-bullet-0"><span class="c8">Todos los documentos personales del usuario ser&aacute;n
                guardados con el mismo formato y nomenclatura.</span></li>
        <li class="c7 c30 c59 li-bullet-0"><span class="c8">El PM verificar&aacute; los resultados de todas las pruebas
                efectuadas.</span></li>
        <li class="c7 c30 c59 li-bullet-0"><span class="c8">El PM aprueba todos los casos de prueba propuestos previo a
                la ejecuci&oacute;n de los mismos</span></li>
        <li class="c7 c30 c59 li-bullet-0"><span class="c1">El equipo de pruebas </span><span
                class="c8">manejar&aacute;</span><span class="c1">&nbsp;todo el esfuerzo de </span><span
                class="c8">ejecuci&oacute;n</span><span class="c1">&nbsp;de prueba </span><span class="c1">de forma
                coordinada con el PM.</span></li>
        <li class="c7 c30 c51 li-bullet-0"><span class="c1">El recorrido y manual de usuario se realizar&aacute; en los
                &uacute;ltimos sprints.</span></li>
    </ol>
    <p class="c6 c51 c157"><span class="c1"></span></p>
    <ol class="c3 lst-kix_d3i63clc3lgg-1" start="2">
        <li class="c7 c24 li-bullet-0">
            <h2 id="h.ja9xqids1cyt" style="display:inline"><span>Objetivos de las pruebas</span></h2>
        </li>
    </ol>
    <p class="c2"><span class="c62 c8 c19">Flujo del Cliente:</span></p>
    <ol class="c3 lst-kix_732m4c7tqfpy-0 start" start="1">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de Login.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de b&uacute;squeda de
                cat&aacute;logo.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de filtrado de cat&aacute;logo.</span>
        </li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad del agendado &nbsp;de la prueba de
                manejo.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de la subida de documentos para la
                solicitud de prueba de manejo.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de la subida de documentos para la
                compra de un auto.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de la transacci&oacute;n del pago para
                la prueba de manejo.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de la transacci&oacute;n de la compra de
                auto</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad del seguimiento de acciones del usuario
                (prueba de manejo o compras).</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad del sistema de Chat.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad del sistema de favoritos
                (wishlist).</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de la edici&oacute;n de datos en el
                perfil.</span></li>
    </ol>
    <p class="c2 c17"><span class="c1"></span></p>
    <p class="c2"><span class="c62 c8 c19">Flujo del Super Administrador:</span></p>
    <ol class="c3 lst-kix_2f59h085xe11-0 start" start="1">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de Login.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de b&uacute;squeda de usuarios.</span>
        </li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar las funcionalidad de filtrado de usuarios.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de la modificaci&oacute;n de datos de un
                grupo automotriz.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de la b&uacute;squeda de
                solicitudes.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad del filtrado de solicitudes.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar funcionalidad de la aprobaci&oacute;n/negaci&oacute;n de
                una solicitud.</span></li>
        <li class="c20 c76 li-bullet-0"><span class="c1">Probar la funcionalidad del registro de un grupo
                automotriz.</span></li>
        <li class="c20 c76 li-bullet-0"><span class="c1">Probar la funcionalidad del dashboard estad&iacute;stico.
            </span></li>
    </ol>
    <p class="c2"><span class="c62 c8 c19">Flujo del Grupo Automotriz:</span></p>
    <p class="c7 c66 c125"><span class="c1">Etapa 1:</span></p>
    <ol class="c3 lst-kix_iqtl5xa2cmxc-0 start" start="1">
        <li class="c25 c7 li-bullet-0"><span class="c1">Probar funcionalidad del Login.</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Probar funcionalidad para realizar una aplicaci&oacute;n.</span>
        </li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Probar funcionalidad del panel de seguimiento a una
                aplicaci&oacute;n.</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Probar funcionalidad de la modificaci&oacute;n de los datos del
                perfil.</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Probar funcionalidad de la eliminaci&oacute;n de una
                cuenta.</span></li>
    </ol>
    <p class="c2 c85"><span class="c1">Etapa 2:</span></p>
    <ol class="c3 lst-kix_9sstyjjxvcqu-0 start" start="1">
        <li class="c25 c7 li-bullet-0"><span class="c1">Probar funcionalidad de Login.</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Probar funcionalidad del registro de una agencia.</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Probar funcionalidad de la b&uacute;squeda de usuarios.</span>
        </li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Probar funcionalidad del filtrado de usuarios.</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">&nbsp;Probar funcionalidad para la modificaci&oacute;n de datos
                de una agencia.</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Probar funcionalidad del dashboard estad&iacute;stico.</span>
        </li>
    </ol>
    <p class="c6 c66"><span class="c1"></span></p>
    <p class="c2"><span class="c62 c8 c19">Flujo de la Agencia:</span></p>
    <ol class="c3 lst-kix_7h0jbu1x222k-0 start" start="1">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar funcionalidad de Login.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar funcionalidad de la b&uacute;squeda de usuarios.</span>
        </li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar funcionalidad del filtrado de usuarios.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar funcionalidad del registro de un gerente.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar funcionalidad para la modificaci&oacute;n de datos de un
                gerente.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar funcionalidad para la
                actualizaci&oacute;n/modificaci&oacute;n del cat&aacute;logo de autos.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar funcionalidad del dashboard estad&iacute;stico.</span>
        </li>
    </ol>
    <p class="c6 c66 c125"><span class="c1"></span></p>
    <p class="c2"><span class="c62 c8 c19">Flujo del Gerente:</span></p>
    <ol class="c3 lst-kix_7hnw7pp31c96-0 start" start="1">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar funcionalidad de Login.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar funcionalidad de la b&uacute;squeda de usuarios.</span>
        </li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar funcionalidad del filtrado de usuarios.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar funcionalidad del registro de un vendedor.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar funcionalidad para la modificaci&oacute;n de datos de un
                vendedor.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar funcionalidad para la
                actualizaci&oacute;n/modificaci&oacute;n del cat&aacute;logo de autos.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar funcionalidad del dashboard estad&iacute;stico.</span>
        </li>
    </ol>
    <p class="c6 c66"><span class="c62 c8 c19"></span></p>
    <p class="c6 c66"><span class="c62 c8 c19"></span></p>
    <p class="c2"><span class="c62 c8 c19">Flujo del Vendedor:</span></p>
    <ol class="c3 lst-kix_mg52369i75sn-0 start" start="1">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar funcionalidad del Login.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de b&uacute;squeda de
                cat&aacute;logo.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de filtrado de cat&aacute;logo.</span>
        </li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de la b&uacute;squeda de
                solicitudes.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad del filtrado de solicitudes.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar funcionalidad del manejo de una solicitud.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar funcionalidad del sistema de chat.</span></li>
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar funcionalidad del dashboard estad&iacute;stico.</span>
        </li>
    </ol>
    <h2 class="c7 c94 c103" id="h.1cjsyuq850k3"><span class="c47 c143"></span></h2>
    <ol class="c3 lst-kix_d3i63clc3lgg-1" start="3">
        <li class="c7 c24 li-bullet-0">
            <h2 id="h.j8zy2j5g5i1t" style="display:inline"><span>Alcance</span></h2>
        </li>
    </ol>
    <p class="c2"><span class="c62 c8 c19">Flujo del Cliente:</span></p>
    <ol class="c3 lst-kix_rg52xa75v2qv-0 start" start="1">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de Login.</span></li>
    </ol>
    <ul class="c3 lst-kix_34xw20osf7pl-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Acceso v&aacute;lido con Credenciales correctas de
                super-administrador.</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Acceso no autorizado con correo invalido/cuenta
                inexistente.</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Acceso no autorizado con contrase&ntilde;a incorrecta.</span>
        </li>
    </ul>
    <ol class="c3 lst-kix_rg52xa75v2qv-0" start="2">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de b&uacute;squeda de
                cat&aacute;logo.</span></li>
    </ol>
    <ul class="c3 lst-kix_pzlvm0ag2zpq-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Se hace una b&uacute;squeda de un auto dentro del
                cat&aacute;logo</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">El sistema muestra los resultados de los autos segun la
                b&uacute;squeda</span></li>
    </ul>
    <ol class="c3 lst-kix_rg52xa75v2qv-0" start="3">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de filtrado de cat&aacute;logo.</span>
        </li>
    </ol>
    <ul class="c3 lst-kix_kszrschy9h6a-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Dentro de la b&uacute;squeda de un auto del cat&aacute;logo se
                muestran los filtros disponibles para la b&uacute;squeda</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Se seleccionan los filtros deseados</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">El sistema muestra los resultados de los autos seg&uacute;n los
                filtros aplicados</span></li>
    </ul>
    <ol class="c3 lst-kix_rg52xa75v2qv-0" start="4">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad del agendado de la prueba de
                manejo.</span></li>
    </ol>
    <ul class="c3 lst-kix_d2dmeguqo78-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">El usuario cliente selecciona el auto de su preferencia para
                solicitar una prueba de manejo</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Para poder solicitar la prueba es necesario que llene un
                formulario y suba los documentos necesarios</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Una vez completado lo anterior su solicitud se confirma y
                autom&aacute;ticamente se le asigna un usuario vendedor que le dar&aacute; seguimiento a su
                solicitud</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">El usuario vendedor se pone en contacto con el cliente a
                trav&eacute;s del chat de la plataforma, en caso de que tenga dudas, adem&aacute;s puede ver el estatus
                de su solicitud en un apartado donde se listaran las solicitudes del cliente</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">El vendedor revisa los documentos de la solicitud, si
                est&aacute;n correctos se aprueban, de lo contrario el vendedor le tiene que notificar al cliente para
                que pueda volver a subir sus documentos correctamente</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Una vez que los documentos son aprobados por el vendedor, en
                caso de que el auto seleccionado se requiera pagar una cuota para la prueba de manejo, se hace la
                transacci&oacute;n necesaria </span></li>
        <li class="c25 c7 li-bullet-0"><span class="c8">Una vez completada la transacci&oacute;n el cliente agenda
            </span><span class="c8">su prueba</span><span class="c1">&nbsp;de manejo</span></li>
    </ul>
    <ol class="c3 lst-kix_rg52xa75v2qv-0" start="5">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de la subida de documentos para la
                solicitud de prueba de manejo.</span></li>
    </ol>
    <ul class="c3 lst-kix_piws44cnashc-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">El usuario cliente selecciona el auto de su preferencia para
                solicitar una prueba de manejo</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">El cliente llena el formulario con los datos necesarios y sube
                los documentos que se le piden</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">El vendedor revisa los documentos de la solicitud, si
                est&aacute;n correctos se aprueban, de lo contrario el vendedor le tiene que notificar al cliente para
                que pueda volver a subir sus documentos correctamente</span></li>
    </ul>
    <ol class="c3 lst-kix_rg52xa75v2qv-0" start="6">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de la subida de documentos para la
                compra de un auto.</span></li>
    </ol>
    <ul class="c3 lst-kix_8phg914ssidx-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">El usuario cliente selecciona un veh&iacute;culo y solicita
                comprarlo</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Para poder solicitar la comprar es necesario que llene un
                formulario y suba los documentos necesarios</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Despu&eacute;s de subirlos se le asignar&aacute; un vendedor
                quien revisar&aacute; sus documentos y le dar&aacute; seguimiento a su compra</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Una vez que complete esto el cliente puede ver el estatus de su
                solicitud en un apartado donde se listaran sus solicitudes</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">El vendedor al revisar los documentos si est&aacute;n correctos
                los aprueba y puede continuar con el proceso de compra, de lo contrario le tiene que notificar al
                usuario para que los vuelva a subir</span></li>
    </ul>
    <ol class="c3 lst-kix_rg52xa75v2qv-0" start="7">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de la transacci&oacute;n del pago para
                la prueba de manejo.</span></li>
    </ol>
    <ul class="c3 lst-kix_rzviu7jw11bm-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Una vez que los documentos de la prueba de manejo fueron
                aprobados, si el veh&iacute;culo necesita una cuota para realizar la prueba se le notifica al
                cliente</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">El cliente revisa el seguimiento de su solicitud y hace el
                pago</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Una vez que termina el pago el sistema le confirma de recibido
                el pago y se actualiza el seguimiento</span></li>
    </ul>
    <ol class="c3 lst-kix_rg52xa75v2qv-0" start="8">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de la transacci&oacute;n de la compra de
                auto</span></li>
    </ol>
    <ul class="c3 lst-kix_xnlyfuqgi6j3-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Una vez que los documentos de la compra fueron aprobados, se le
                notifica al cliente para pueda realizar el pago del veh&iacute;culo</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">El cliente revisa el seguimiento de su solicitud y hace el
                pago</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Una vez que termina el pago el sistema le confirma de recibido
                el pago y se actualiza el seguimiento</span></li>
    </ul>
    <ol class="c3 lst-kix_rg52xa75v2qv-0" start="9">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad del seguimiento de acciones del usuario
                (prueba de manejo o compras).</span></li>
    </ol>
    <ul class="c3 lst-kix_zfbk09w23seu-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Una vez que el cliente sube los documentos necesarios ya sea
                para la prueba de manejo o para la compra de un auto puede realizar el seguimiento de su
                solicitud</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">En el apartado indicado de seguimiento, puede ver en qu&eacute;
                fase va su solicitud</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Mientras el vendedor asignado a su solicitud la revisa y
                mientras va avanzando el proceso el vendedor va actualizando la etapa en la que se encuentra el
                cliente</span></li>
    </ul>
    <ol class="c3 lst-kix_rg52xa75v2qv-0" start="10">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad del sistema de Chat.</span></li>
    </ol>
    <ul class="c3 lst-kix_6bgajs6h3l6j-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Entrada a la vista de chats y contactos con acceso de
                cliente</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">El cliente revisa si tiene alg&uacute;n mensaje</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Selecciona una conversaci&oacute;n iniciada</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">El vendedor y el cliente pueden tener un medio de contacto
                directo</span></li>
    </ul>
    <ol class="c3 lst-kix_rg52xa75v2qv-0" start="11">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad del sistema de favoritos
                (wishlist).</span></li>
    </ol>
    <ul class="c3 lst-kix_443kk3whga57-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Se muestra el cat&aacute;logo de autos</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Si al cliente le interesa alg&uacute;n auto lo marca como
                favorito</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">En el apartado indicado el cliente puede revisar su lista de
                favoritos con los autos que marc&oacute; previamente </span></li>
    </ul>
    <ol class="c3 lst-kix_rg52xa75v2qv-0" start="12">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de la edici&oacute;n de datos en el
                perfil.</span></li>
    </ol>
    <ul class="c3 lst-kix_vwqv628w1cm9-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">El cliente puede acceder a los ajustes de su cuenta en el
                apartado indicado</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Dentro de los ajustes puede seleccionar la opci&oacute;n de
                modificar sus datos</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Al entrar a la opci&oacute;n modifica los datos necesarios y al
                final selecciona el bot&oacute;n de guardar cambios</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Los datos se actualizan tanto en la vista del cliente, como en
                la base de datos</span></li>
    </ul>
    <p class="c6 c66"><span class="c1"></span></p>
    <p class="c6 c66"><span class="c1"></span></p>
    <p class="c2"><span class="c62 c8 c19">Flujo del Super Administrador:</span></p>
    <ol class="c3 lst-kix_gcnxpnn6kj0u-0 start" start="1">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de Login.</span></li>
    </ol>
    <ul class="c3 lst-kix_wcxg857dis8q-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Acceso v&aacute;lido con Credenciales correctas de
                super-administrador</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Acceso no autorizado con correo invalido/cuenta
                inexistente</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Acceso no autorizado con contrase&ntilde;a incorrecta</span>
        </li>
    </ul>
    <ol class="c3 lst-kix_gcnxpnn6kj0u-0" start="2">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de b&uacute;squeda de usuarios.</span>
        </li>
    </ol>
    <ul class="c3 lst-kix_cj4e1u6rjkyy-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Se hace una b&uacute;squeda de un usuario dentro del
                cat&aacute;logo</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">El sistema muestra los resultados de los usuarios seg&uacute;n
                la b&uacute;squeda</span></li>
    </ul>
    <ol class="c3 lst-kix_gcnxpnn6kj0u-0" start="3">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar las funcionalidad de filtrado de usuarios.</span></li>
    </ol>
    <ul class="c3 lst-kix_px402vn9x8-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Dentro de la b&uacute;squeda de usuarios se muestran los filtros
                disponibles para la b&uacute;squeda</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Se seleccionan los filtros deseados</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">El sistema muestra los resultados de lo usuarios seg&uacute;n
                los filtros aplicados</span></li>
    </ul>
    <ol class="c3 lst-kix_gcnxpnn6kj0u-0" start="4">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de la modificaci&oacute;n de datos de un
                grupo automotriz.</span></li>
    </ol>
    <ul class="c3 lst-kix_mo3vsi1bdout-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Se accede a la p&aacute;gina de la cuenta del grupo automotriz
                con acceso de super-administrador</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Se efect&uacute;a un cambio de la informaci&oacute;n del grupo
                automotriz desde la p&aacute;gina de la cuenta.</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Se guardan los cambios de la cuenta del grupo automotriz.</span>
        </li>
    </ul>
    <ol class="c3 lst-kix_gcnxpnn6kj0u-0" start="5">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de la b&uacute;squeda de
                solicitudes.</span></li>
    </ol>
    <ul class="c3 lst-kix_vkx9pph5x7p6-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Se hace una b&uacute;squeda de una solicitud dentro del
                cat&aacute;logo</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">El sistema muestra los resultados de las solicitudes y sus
                estados</span></li>
    </ul>
    <ol class="c3 lst-kix_gcnxpnn6kj0u-0" start="6">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad del filtrado de solicitudes.</span></li>
    </ol>
    <ul class="c3 lst-kix_y2tifijecnbl-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Dentro de la b&uacute;squeda de solicitudes se muestran los
                filtros disponibles para la b&uacute;squeda</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Se seleccionan los filtros deseados</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">El sistema muestra los resultados de las solicitudes
                seg&uacute;n los filtros aplicados (aprobada/pendiente/denegada)</span></li>
    </ul>
    <ol class="c3 lst-kix_gcnxpnn6kj0u-0" start="7">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar funcionalidad de la aprobaci&oacute;n/negaci&oacute;n de
                una solicitud.</span></li>
    </ol>
    <ul class="c3 lst-kix_6y7yxgsemxkh-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Se elige una solicitud pendiente con acceso de
                super-administrador</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Se efect&uacute;a la aprobaci&oacute;n de una solicitud en
                espera</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Se efect&uacute;a la negaci&oacute;n de una solicitud en
                espera</span></li>
    </ul>
    <ol class="c3 lst-kix_gcnxpnn6kj0u-0" start="8">
        <li class="c20 c76 li-bullet-0"><span class="c1">Probar la funcionalidad del registro de un grupo
                automotriz.</span></li>
    </ol>
    <ul class="c3 lst-kix_chmh4a308mm1-0 start">
        <li class="c25 c76 li-bullet-0"><span class="c1">Se accede al landing-page de creaci&oacute;n de grupo
                automotriz.</span></li>
        <li class="c25 c76 li-bullet-0"><span class="c1">Creaci&oacute;n exitosa de un grupo automotriz</span></li>
        <li class="c25 c76 li-bullet-0"><span class="c1">Acceso exitoso a la cuenta del grupo automotriz</span></li>
    </ul>
    <ol class="c3 lst-kix_gcnxpnn6kj0u-0" start="9">
        <li class="c20 c76 li-bullet-0"><span class="c1">Probar la funcionalidad del dashboard estad&iacute;stico.
            </span></li>
    </ol>
    <ul class="c3 lst-kix_avq738omluz-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Acceso al dashboard con una cuenta de nivel valido muestra las
                estad&iacute;sticas y m&eacute;tricas de la plataforma</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Las estad&iacute;sticas son v&aacute;lidas y representativas de
                los datos dentro del sistema</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Las opciones y par&aacute;metros presentes dentro de la vista
                permiten ver estad&iacute;sticas particulares de acuerdo a la selecci&oacute;n de las mismas.</span>
        </li>
    </ul>
    <p class="c6 c66"><span class="c1"></span></p>
    <p class="c2"><span class="c62 c8 c19">Flujo del Vendedor:</span></p>
    <ol class="c3 lst-kix_mg52369i75sn-0" start="9">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar funcionalidad del Login.</span></li>
    </ol>
    <ul class="c3 lst-kix_hdfcogwop0vx-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Acceso v&aacute;lido con Credenciales correctas de
                vendedor</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Acceso no autorizado con correo invalido/cuenta
                inexistente</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Acceso no autorizado con contrase&ntilde;a incorrecta</span>
        </li>
    </ul>
    <ol class="c3 lst-kix_mg52369i75sn-0" start="10">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de b&uacute;squeda de
                cat&aacute;logo.</span></li>
    </ol>
    <ul class="c3 lst-kix_e5d5ipugdti2-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Se hace una b&uacute;squeda de un auto dentro del
                cat&aacute;logo</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">El sistema muestra los resultados de los autos segun la
                b&uacute;squeda</span></li>
    </ul>
    <ol class="c3 lst-kix_mg52369i75sn-0" start="11">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de filtrado de cat&aacute;logo.</span>
        </li>
    </ol>
    <ul class="c3 lst-kix_9ovnuv191t9a-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Dentro de la b&uacute;squeda de un auto del cat&aacute;logo se
                muestran los filtros disponibles para la b&uacute;squeda</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Se seleccionan los filtros deseados</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">El sistema muestra los resultados de los autos seg&uacute;n los
                filtros aplicados</span></li>
    </ul>
    <ol class="c3 lst-kix_mg52369i75sn-0" start="12">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad de la b&uacute;squeda de
                solicitudes.</span></li>
    </ol>
    <ul class="c3 lst-kix_yhyf0j2galop-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Se hace una b&uacute;squeda de una solicitud dentro del
                cat&aacute;logo</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">El sistema muestra los resultados de las solicitudes y sus
                estados</span></li>
    </ul>
    <ol class="c3 lst-kix_mg52369i75sn-0" start="13">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar la funcionalidad del filtrado de solicitudes.</span></li>
    </ol>
    <ul class="c3 lst-kix_ma8jl2wvcrl-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Dentro de la b&uacute;squeda de solicitudes se muestran los
                filtros disponibles para la b&uacute;squeda</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Se seleccionan los filtros deseados</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">El sistema muestra los resultados de las solicitudes
                seg&uacute;n los filtros aplicados (aprobada/pendiente/denegada)</span></li>
    </ul>
    <ol class="c3 lst-kix_mg52369i75sn-0" start="14">
        <li class="c7 c20 li-bullet-0"><span class="c8">Probar funcionalidad del manejo de una solicitud.</span></li>
    </ol>
    <ul class="c3 lst-kix_nzvnkv2irake-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Se elige una solicitud</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c8">Dentro de la vista de solicitud se modifica la etapa de
                proceso.</span></li>
    </ul>
    <ol class="c3 lst-kix_mg52369i75sn-0" start="15">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar funcionalidad del sistema de chat.</span></li>
    </ol>
    <ul class="c3 lst-kix_sxsbp83evw5r-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Entrada a la vista de chats y contactos con acceso de
                vendedor</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Selecci&oacute;n de una conversaci&oacute;n iniciada</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Creaci&oacute;n de una conversaci&oacute;n desde vista de
                contacto</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Enviar mensaje al cliente</span></li>
    </ul>
    <ol class="c3 lst-kix_mg52369i75sn-0" start="16">
        <li class="c7 c20 li-bullet-0"><span class="c1">Probar funcionalidad del dashboard estad&iacute;stico.</span>
        </li>
    </ol>
    <ul class="c3 lst-kix_87xx17fjt6sp-0 start">
        <li class="c25 c7 li-bullet-0"><span class="c1">Acceso al dashboard con una cuenta de nivel valido muestra las
                estad&iacute;sticas y m&eacute;tricas de la plataforma</span></li>
        <li class="c25 c7 li-bullet-0"><span class="c1">Las estad&iacute;sticas son v&aacute;lidas y representativas de
                los datos dentro del sistema</span></li>
        <li class="c7 c25 li-bullet-0"><span class="c1">Las opciones y par&aacute;metros presentes dentro de la vista
                permiten ver estad&iacute;sticas particulares de acuerdo a la selecci&oacute;n de las mismas.</span>
        </li>
    </ul>
    <p class="c7 c66"><span
            class="c1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>
    </p>
    <ol class="c3 lst-kix_d3i63clc3lgg-1" start="4">
        <li class="c7 c24 li-bullet-0">
            <h2 id="h.h904v6h0rrrr" style="display:inline"><span class="c16">Niveles de pruebas</span></h2>
        </li>
    </ol>
    <p class="c7 c66"><span class="c1">A continuaci&oacute;n se muestran el nivel de las pruebas que se
            realizar&aacute;n durante el desarrollo del proyecto, adem&aacute;s de detallar algunas de los
            m&eacute;todos que se utilizaran al igual que los responsables de dichas pruebas.</span></p>
    <p class="c6 c66"><span class="c1"></span></p>
    <p class="c7 c66 c89"><span class="c16">Pruebas Informales (Prueba Funcional)</span></p>
    <p class="c7 c66 c85"><span class="c8">El prop&oacute;sito de este tipo de pruebas es verificar r&aacute;pidamente
            el funcionamiento de los componentes del software. Las pruebas de este estilo no tienen ning&uacute;n tipo
            de entrega.</span></p>
    <ol class="c3 lst-kix_p4d0i57im8n6-0 start" start="1">
        <li class="c7 c60 li-bullet-0"><span class="c1">Alcance: Todas las secciones desarrolladas ser&aacute;n probadas
                mediante pruebas unitarias informales.</span></li>
        <li class="c7 c60 li-bullet-0"><span class="c1">Responsables: Los desarrolladores de software.</span></li>
        <li class="c7 c60 li-bullet-0"><span class="c1">Metodolog&iacute;a: Los desarrolladores responsables del
                componentes se encargaran de realizar pruebas de Input-Output para comprobar su correcto
                funcionamiento.</span></li>
        <li class="c7 c60 li-bullet-0"><span class="c1">Cada cuando: En cuanto se finalice, o se modifique alg&uacute;n
                componente.</span></li>
    </ol>
    <p class="c2 c17"><span class="c1"></span></p>
    <p class="c7 c66 c89"><span class="c47 c50">Prueba de Caja Negra (Prueba Funcional)</span></p>
    <p class="c7 c66 c85"><span class="c8">El prop&oacute;sito de las pruebas unitarias es probar cada uno de los
            componentes y funcionalidades &nbsp;que comprenden la aplicaci&oacute;n que se desarrollar&aacute;.</span>
    </p>
    <p class="c2 c17"><span class="c16"></span></p>
    <ol class="c3 lst-kix_xs41mtxr57df-0 start" start="1">
        <li class="c7 c60 li-bullet-0"><span class="c8">Alcanc</span><span class="c1">e: Todas las secciones
                desarrolladas ser&aacute;n probadas mediante pruebas de caja negra.</span></li>
        <li class="c7 c60 li-bullet-0"><span class="c1">Responsables: Los desarrolladores de software y los
                testers.</span></li>
        <li class="c7 c60 li-bullet-0"><span class="c1">Metodolog&iacute;a: Los desarrolladores probar&aacute;n
                componentes de la aplicaci&oacute;n sin tener conocimiento del c&oacute;digo detr&aacute;s de los mismos
                componentes, reportando errores en caso de encontrarlos. Espec&iacute;ficamente, el tipo de pruebas de
                caja negra que se realizar&aacute;n ser&aacute;n pruebas de tipo de casos de uso. Dentro de estas
                pruebas se realizar&aacute;n tres bater&iacute;as negativas y tres bater&iacute;as positivas que se
                deber&aacute;n cumplir cuando se realicen este tipo de pruebas.</span></li>
        <li class="c7 c60 li-bullet-0"><span class="c8">Cada cu&aacute;ndo: Al finalizar cada componente.</span></li>
    </ol>
    <h3 class="c7 c74 c103" id="h.6j2xwew2rmlu"><span class="c16"></span></h3>
    <h3 class="c7 c74" id="h.91fzm9dtgvmr"><span>Prueba de Caja Blanca</span><span class="c16">&nbsp;(Prueba
            Funcional)</span></h3>
    <p class="c33"><span class="c8">El prop&oacute;sito de este tipo de pruebas es encontrar la causa de alg&uacute;n
            tipo de falla que se </span><span class="c8">haya encontrado en otro tipo de pruebas. En espec&iacute;fico,
            las pruebas de caja blanca que se realizan son pruebas de cobertura, es decir, se probar&aacute;n los tres
            caminos m&aacute;s utilizados por los usuarios. </span><span class="c8">M&aacute;s a&uacute;n, se
            considerar&aacute; que los caminos seleccionados son apropiados si estos cubren un m&iacute;nimo de 80%
            &nbsp;de los caminos posibles. Este 80% debe regresar resultados de prueba positivos para as&iacute;
            justificar que el componente funciona de manera correcta. </span></p>
    <ol class="c3 lst-kix_wzt0u5vle4mu-0 start" start="1">
        <li class="c46 li-bullet-0"><span class="c1">Alcance: Cualquier componente de software que presente alguna falla
                dentro de alg&uacute;n otro tipo de prueba.</span></li>
        <li class="c46 li-bullet-0"><span class="c1">Responsables: Los desarrolladores de software y los testers.</span>
        </li>
        <li class="c46 li-bullet-0"><span class="c1">Metodolog&iacute;a: Los desarrolladores que se encargaron de crear
                los componentes en donde se encontraron los errores ser&aacute;n los encargados de realizar pruebas de
                caja blanca con el objetivo de encontrar que pedazo de c&oacute;digo es el que est&aacute; causando
                dicho error.</span></li>
        <li class="c46 li-bullet-0"><span class="c1">Cada cu&aacute;ndo: Al finalizar cada sprint.</span></li>
    </ol>
    <h3 class="c7 c74 c103 c89" id="h.7e2hupja93t3"><span class="c16"></span></h3>
    <h3 class="c7 c74" id="h.xhc6264rls1i"><span class="c16">Prueba de Integraci&oacute;n (Prueba Funcional)</span></h3>
    <p class="c33"><span class="c8">El prop&oacute;sito de las pruebas de integraci&oacute;n es comprobar el correcto
            funcionamiento de la aplicaci&oacute;n cuando todos los componentes son utilizados en conjunto. </span><span
            class="c1">Para efectos de este proyecto, debido a las restricciones de tiempo, este tipo de pruebas
            s&oacute;lo ser&aacute;n realizadas en los componentes cr&iacute;ticos de la aplicaci&oacute;n. </span></p>
    <ol class="c3 lst-kix_dgjxhhel0iia-0 start" start="1">
        <li class="c46 li-bullet-0"><span class="c1">Alcance: Componentes cr&iacute;ticos para el funcionamiento de la
                aplicaci&oacute;n</span></li>
        <li class="c46 li-bullet-0"><span class="c1">Responsables: Los responsables de cada c&eacute;lula de
                trabajo.</span></li>
        <li class="c46 li-bullet-0"><span class="c1">Metodolog&iacute;a: Los desarrolladores responsables de cada
                c&eacute;lula, al terminar m&aacute;s de un componente relacionado, empezaran a realizar pruebas e
                integraci&oacute;n. De la misma manera, al terminar el proyecto, se realizar&aacute;n &nbsp;nuevas
                pruebas de este estilo.</span></li>
        <li class="c46 li-bullet-0"><span class="c8">Cada cu&aacute;ndo: Al </span><span class="c8">terminarse
                pedazos</span><span class="c1">&nbsp;de software relacionados y al acabar todos los componentes de la
                aplicaci&oacute;n.</span></li>
    </ol>
    <p class="c92 c66 c17"><span class="c1"></span></p>
    <h3 class="c7 c74" id="h.j8epsprogp2p"><span class="c16">Prueba de Aceptaci&oacute;n (Prueba Funcional)</span></h3>
    <p class="c33"><span class="c1">El prop&oacute;sito de este tipo de pruebas es validar con el equipo de desarrollo y
            NDS si el sistema est&aacute; a la par con sus expectativas y cumple las funcionalidades que fueron
            discutidas en el documento SRS.</span></p>
    <ol class="c3 lst-kix_i0244pw02jv6-0 start" start="1">
        <li class="c46 li-bullet-0"><span class="c1">Alcance: Todos los aspectos del pedazo de software ser&aacute;n
                probados pruebas de validaci&oacute;n. Esto con el objetivo de revisar si aspectos de dise&ntilde;o y
                funcionalidad de la aplicaci&oacute;n est&aacute;n a la par de las expectativas de NDS.</span></li>
        <li class="c46 li-bullet-0"><span class="c1">Responsables: Rub&eacute;n Raya (NDS), los desarrolladores, los
                testers y el SCRUM master..</span></li>
        <li class="c46 li-bullet-0"><span class="c1">Metodolog&iacute;a: Los desarrolladores se reunir&aacute;n con
                Rub&eacute;n Raya y bajo su supervisi&oacute;n se encargar&aacute; de validar los aspectos importantes
                de la aplicaci&oacute;n desarrollada.</span></li>
        <li class="c46 li-bullet-0"><span class="c1">Cada cu&aacute;ndo:En cuanto se cumplan las pruebas de
                integraci&oacute;n.</span></li>
    </ol>
    <p class="c10"><span class="c1"></span></p>
    <h3 class="c7 c66 c94" id="h.qsyst13rz67j"><span>Prueba de Recorrido Est&aacute;tico (Validaci&oacute;n)</span></h3>
    <p class="c33"><span class="c1">El prop&oacute;sito de este tipo de pruebas es asegurar que el servicio, en
            t&eacute;rminos de funcionalidad y desempe&ntilde;o, act&uacute;e de manera satisfactoria.</span></p>
    <ol class="c3 lst-kix_rg98grvtj3pg-0 start" start="1">
        <li class="c46 li-bullet-0"><span class="c1">Alcance: Dado que se trata de una prueba de sistema, el software
                ser&aacute; probado en completud.</span></li>
        <li class="c46 li-bullet-0"><span class="c1">Responsables: Desarrolladores no pertenecientes al proyecto, los
                testers, el SCRUM master y Rub&eacute;n Raya (NDS). Un recorrido se considera aceptado una vez que sea
                aprobado por el equipo de desarrolladores y Rub&eacute;n Raya. Los responsables del proceso de
                validaci&oacute;n son los desarrolladores no pertenecientes al proyecto, Esteban Castillo y Ruben Raya.
                &nbsp;</span></li>
        <li class="c46 li-bullet-0"><span class="c1">Metodolog&iacute;a: Crear escenarios de acuerdo a las situaciones
                m&aacute;s usuales de los usuarios.</span></li>
        <li class="c46 li-bullet-0"><span class="c1">Cada cu&aacute;ndo: Al final del proyecto.</span></li>
    </ol>
    <h2 class="c7 c94 c103" id="h.gwsxrckj7v6b"><span class="c16"></span></h2>
    <ol class="c3 lst-kix_d3i63clc3lgg-1" start="5">
        <li class="c2 c94 c80 li-bullet-0">
            <h2 id="h.cwh2skhwocng" style="display:inline"><span>Criterios de aceptaci&oacute;n de pruebas</span></h2>
        </li>
    </ol>
    <h3 class="c7 c66 c94 c125 c142" id="h.j39ka7pd5nwf"><span class="c16">Pruebas Informales</span></h3>
    <p class="c84"><span class="c8 c152">Cada desarrollador</span><span class="c8">&nbsp;</span><span class="c1">tiene
            como responsabilidad realizar una prueba informal a cada componente que finalice. Ya que esta prueba no
            sigue una metodolog&iacute;a espec&iacute;fica, el desarrollador sabr&aacute; que el componente pas&oacute;
            la prueba si realiza de manera correcta su funcionalidad y trabaja de manera adecuada con otros componentes.
        </span></p>
    <h3 class="c7 c94" id="h.eydwveo9hoky"><span class="c78">&nbsp;</span></h3>
    <h3 class="c7 c94 c79" id="h.fsv2ynwal6n0"><span>Pruebas Unitarias </span><span class="c16">&nbsp;</span></h3>
    <ul class="c3 lst-kix_q48tat6aasri-0 start">
        <li class="c7 c15 li-bullet-0"><span class="c8 c19">Funcionalidad de Login:</span><span class="c1">&nbsp;Esta
                funcionalidad nunca debe fallar. Todas las pruebas deben proporcionar el usuario y la p&aacute;gina de
                inicio correctos, o bien enviar un mensaje de error indicando que el usuario no existe. Esto para cada
                tipo de usuario que permite la plataforma.</span></li>
        <li class="c7 c15 li-bullet-0"><span class="c8 c19">Funcionalidad de Registro:</span><span
                class="c1">&nbsp;Todas las pruebas deben de crear las credenciales ingresadas de forma correcta en la
                base de datos o bien enviar un mensaje de error indicando la raz&oacute;n por la cual las credenciales
                no son permitidas. Igualmente, el registro debe agregar la cuenta con los privilegios y permisos
                correspondientes a cada tipo de usuario.</span></li>
        <li class="c7 c15 li-bullet-0"><span class="c8 c19">Funcionalidad CRUD del Cat&aacute;logo:</span><span
                class="c1">&nbsp;Todas las pruebas deben permitir la subida, lectura, modificaci&oacute;n y
                eliminaci&oacute;n de elementos del cat&aacute;logo de autos. Esto debe de permitirse acorde a los
                permisos respectivos a cada tipo de cuenta, respetando los privilegios que conlleva cada una de ellas.
                Se debe de desplegar el mensaje de error correspondiente, si la informaci&oacute;n/datos por el usuario
                no es permitida/correcta.</span></li>
        <li class="c7 c15 li-bullet-0"><span class="c8 c19">Funcionalidad de B&uacute;squeda del Cat&aacute;logo:
            </span><span class="c1">Todas las pruebas deben permitir la b&uacute;squeda &nbsp;de los autos dentro del
                cat&aacute;logo con uso de lenguaje natural. Para todos los tipos de administradores que tienen acceso
                al cat&aacute;logo pueden hacer una b&uacute;squeda de los autos que pertenecen a su respectivo grupo
                automotriz o a su respectiva agencia, para los clientes pueden hacer una b&uacute;squeda de todos los
                autos de todas las agencia. Los resultados mostrados deben ser relacionados a las palabras ingresadas en
                la barra de b&uacute;squeda, si no hay autos relacionados con las palabras ingresadas en la
                b&uacute;squeda, no se mostrar&aacute;n resultados ya que no hay autos que coincidan. </span></li>
        <li class="c7 c15 li-bullet-0"><span class="c8 c19">Funcionalidad de Filtrado del Cat&aacute;logo</span><span
                class="c1">: Todas las pruebas deben permitir el filtrado de los autos dentro del cat&aacute;logo con
                los filtros previamente determinados. Para todos los tipos de administradores que tienen acceso al
                cat&aacute;logo pueden hacer un filtrado de la b&uacute;squeda de los autos que pertenecen a su
                respectivo grupo automotriz o a su respectiva agencia, para los clientes pueden hacer un filtrado de la
                b&uacute;squeda de todos los autos de todas las agencia. Los resultados mostrados deben ser seg&uacute;n
                los filtros relacionados, si no hay autos que cumplan con las restricciones de los filtros, no se
                mostrar&aacute;n resultados ya que no hay autos que coincidan. </span></li>
    </ul>
    <p class="c6 c37"><span class="c1"></span></p>
    <ul class="c3 lst-kix_q48tat6aasri-0">
        <li class="c7 c15 li-bullet-0"><span class="c8 c19">Funcionalidad de B&uacute;squeda de Usuarios: </span><span
                class="c1">Todas las pruebas deben permitir la b&uacute;squeda de otros usuarios con uso de lenguaje
                natural. Para todos los tipos de administradores que tienen acceso a la b&uacute;squeda de otros
                usuarios pueden hacer una b&uacute;squeda de los usuarios que pertenecen a su respectivo grupo
                automotriz o a su respectiva agencia. Los resultados mostrados deben ser relacionados a las palabras
                ingresadas en la barra de b&uacute;squeda, si no hay usuarios relacionados con las palabras ingresadas
                en la b&uacute;squeda, no se mostrar&aacute;n resultados ya que no hay usuarios que coincidan. </span>
        </li>
        <li class="c7 c15 li-bullet-0"><span class="c8 c19">Funcionalidad de Filtrado de usuarios</span><span
                class="c1">: Todas las pruebas deben permitir el filtrado de los usuarios con los filtros previamente
                determinados. Para todos los tipos de administradores que tienen acceso a la b&uacute;squeda de otros
                usuarios pueden hacer un filtrado de la b&uacute;squeda de los autos que pertenecen a su respectivo
                grupo automotriz o a su respectiva agencia. Los resultados mostrados deben ser seg&uacute;n los filtros
                relacionados, si no hay usuarios que cumplan con las restricciones de los filtros, no se
                mostrar&aacute;n resultados ya que no hay usuarios que coincidan. </span></li>
    </ul>
    <p class="c6 c37"><span class="c1"></span></p>
    <ul class="c3 lst-kix_q48tat6aasri-0">
        <li class="c7 c15 li-bullet-0"><span class="c62 c8 c19">Funcionalidad de Pago:</span></li>
    </ul>
    <p class="c7 c37"><span class="c1">Todas las pruebas deben permitir que el usuario pueda realizar el pago de un auto
            mediante cada uno de los diferentes m&eacute;todos de pago que ofrece la plataforma. Se deben de desplegar
            mensajes ya sea de &eacute;xito en la transacci&oacute;n o falla en la misma, indicando al usuario si hay
            una raz&oacute;n de su lado por la cual no fue posible efectuar el pago. </span></p>
    <ul class="c3 lst-kix_q48tat6aasri-0">
        <li class="c7 c15 li-bullet-0"><span class="c62 c8 c19">Funcionalidad de Chat:</span></li>
    </ul>
    <p class="c7 c37"><span class="c1">Todas las pruebas deben permitir que el usuario pueda seleccionar a otro usuario
            y comunicarse con este efectivamente mediante mensajes. Los mensajes enviados deben de ser visibles y
            mostrarse en la cuenta receptora, con la capacidad de mostrar un mensaje de error indicando al usuario la
            raz&oacute;n por la cual no se pudo enviar el mismo.</span></p>
    <ul class="c3 lst-kix_q48tat6aasri-0">
        <li class="c7 c15 li-bullet-0"><span class="c62 c8 c19">Funcionalidad de Favoritos (Wishlist):</span></li>
    </ul>
    <p class="c7 c37"><span class="c1">Todas las pruebas deben permitir que el usuario pueda marcar como
            &ldquo;favorito&rdquo; a todos los autos que desea, as&iacute; como visualizarlos correctamente en la
            secci&oacute;n de &ldquo;wishlist&rdquo;. Asimismo, el usuario siempre debe de ser capaz de eliminar a
            cualquier auto de dicha lista, donde los cambios deber&aacute;n reflejarse correctamente.</span></p>
    <ul class="c3 lst-kix_q48tat6aasri-0">
        <li class="c7 c15 li-bullet-0"><span class="c8 c19 c62">Funcionalidad Anal&iacute;tica:</span></li>
    </ul>
    <p class="c7 c37"><span class="c1">Todas las pruebas deben permitir que cada tipo de usuario pueda visualizar
            correctamente las estad&iacute;sticas e informaci&oacute;n adecuada para los permisos que le corresponden a
            dicha cuenta. Esta funcionalidad siempre deber&aacute; estar activa, y de haber un error en el lado del
            servidor, se deber&aacute; indicar con un mensaje respectivamente.</span></p>
    <p class="c6 c37"><span class="c1"></span></p>
    <h3 class="c7 c79 c94" id="h.kzej3b9e4wfe"><span>Prueba de Integraci&oacute;n</span></h3>
    <ul class="c3 lst-kix_u2d5nq9gvteo-0 start">
        <li class="c7 c30 li-bullet-0"><span class="c62 c8 c19">Manejo de Solicitudes: </span><span
                class="c8">Todas</span><span class="c1">&nbsp;</span><span class="c8">las pruebas deber&aacute;n
                permitir que el usuario en cuesti&oacute;n (Super-Admin y Vendedor) pueda modificar el estado/etapa de
                cualquier solicitud a su cargo. Asimismo, debe ser posible comentar acerca del estado de una solicitud
                as&iacute; informando al aplicante las acciones que debe realizar, o razones que justifican el estado de
                su solicitud. Finalmente, el usuario que maneja las solicitudes debe de poder negar o aceptar cualquier
                solicitud. Todo lo descrito anteriormente, debe siempre verse reflejado en la cuenta del usuario
                aplicante.</span></li>
        <li class="c7 c30 li-bullet-0"><span class="c62 c8 c19">Compra de un Auto:</span></li>
    </ul>
    <p class="c7 c125"><span class="c1">Todas las pruebas deber&aacute;n permitir que el cliente tenga la capacidad de
            comprar un auto exitosamente, y que este pase por las dos posibilidades principales en el proceso de compra,
            siendo la aceptaci&oacute;n o negaci&oacute;n de la solicitud. Para ello, el cliente debe ser capaz de
            seleccionar un auto junto con sus especificaciones, aplicar para la compra del mismo, subir la
            informaci&oacute;n y documentos necesarios, darle seguimiento a su solicitud, esperar la
            aceptaci&oacute;n/negaci&oacute;n de la misma, efectuar la compra por uno de los m&eacute;todos de pago
            disponible, continuar la comunicaci&oacute;n con el vendedor el tiempo que sea necesario para finalmente
            recibir su adquisici&oacute;n. </span></p>
    <ul class="c3 lst-kix_u2d5nq9gvteo-0">
        <li class="c7 c30 li-bullet-0"><span class="c8 c19">Agendado de la prueba de manejo: </span><span
                class="c1">Todas las pruebas deber&aacute;n permitir que el cliente tenga la capacidad de agendar una
                prueba de manejo exitosamente, y que este pase por las dos posibilidades principales en el proceso de
                agendado, siendo la aceptaci&oacute;n o negaci&oacute;n de la solicitud. Para ello, el cliente debe ser
                capaz de seleccionar un auto, solicitar una prueba de manejo para el mismo, subir la informaci&oacute;n
                y documentaci&oacute;n necesaria, darle seguimiento a la solicitud, y de ser aceptada seleccionar una
                fecha, lugar y hora disponible en el horario del vendedor. Asimismo, la comunicaci&oacute;n entre el
                cliente y el vendedor debe de ser posible en todo momento como parte del seguimiento de la prueba de
                manejo. </span></li>
    </ul>
    <h3 class="c7 c71 c103" id="h.92v4azusr6mg"><span class="c16"></span></h3>
    <h3 class="c7 c71" id="h.ns3vrtfyjguc"><span>Prueba de Validaci&oacute;n/Aceptaci&oacute;n</span></h3>
    <ul class="c3 lst-kix_3rm0szfqxvyi-0 start">
        <li class="c7 c30 li-bullet-0"><span class="c8">Los clientes y representantes de los mismos est&aacute;n
                satisfechos con la funcionalidad revisada as&iacute; como la experiencia del usuario (UI/UX) &nbsp;de la
                plataforma.</span></li>
    </ul>
    <h3 class="c7 c94 c79" id="h.7krppuwc58yf"><span>Pruebas Est&aacute;ticas de Recorrido</span></h3>
    <ul class="c3 lst-kix_5e4latf0qe1x-0 start">
        <li class="c7 c30 c110 li-bullet-0"><span class="c8">Es posible completar el flujo b&aacute;sico de la
                plataforma para cada uno de los tipos de usuario, desde el registro, login hasta cada una de sus
                acciones principales. </span></li>
    </ul>
    <p class="c6 c110"><span class="c1"></span></p>
    <ol class="c3 lst-kix_d3i63clc3lgg-1" start="6">
        <li class="c2 c94 c80 li-bullet-0">
            <h2 id="h.s6ntvdjxs5wr" style="display:inline"><span class="c16">Entregables de pruebas</span></h2>
        </li>
    </ol>
    <h2 class="c7 c94 c103 c104" id="h.ev54v0h5kuu0"><span class="c16"></span></h2><a
        id="t.bc86d7e36674b8ba87018d9096ba7e3ada76be7c"></a><a id="t.2"></a>
    <table class="c131 c104">
        <tr class="c13">
            <td class="c22" colspan="1" rowspan="1">
                <p class="c7"><span class="c18">No.</span></p>
            </td>
            <td class="c83" colspan="1" rowspan="1">
                <p class="c7"><span class="c18">Nombre de entregable</span></p>
            </td>
            <td class="c87" colspan="1" rowspan="1">
                <p class="c7"><span class="c18">Autor</span></p>
            </td>
            <td class="c70" colspan="1" rowspan="1">
                <p class="c7"><span class="c18">Reviewer</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c22" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">1.</span></p>
            </td>
            <td class="c83" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Plan de Pruebas</span></p>
            </td>
            <td class="c87" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Director de Pruebas</span></p>
            </td>
            <td class="c70" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Project Manager/Analista de Negocios</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c22" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">2.</span></p>
            </td>
            <td class="c83" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Revisi&oacute;n T&eacute;cnica Formal</span></p>
            </td>
            <td class="c87" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Director de Pruebas</span></p>
            </td>
            <td class="c70" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Project Manager/Analista de Negocios</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c22" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">3.</span></p>
            </td>
            <td class="c83" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Resultados de Pruebas Unitarias</span></p>
            </td>
            <td class="c87" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Equipo de Pruebas</span></p>
            </td>
            <td class="c70" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Project Manager</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c22" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">4.</span></p>
            </td>
            <td class="c83" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Resultados de Pruebas Integrales</span></p>
            </td>
            <td class="c87" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Equipo de Pruebas</span></p>
            </td>
            <td class="c70" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Project Manager</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c22" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">5.</span></p>
            </td>
            <td class="c83" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Resultados de Pruebas de Validaci&oacute;n</span></p>
            </td>
            <td class="c87" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Equipo de Pruebas</span></p>
            </td>
            <td class="c70" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Project Manager</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c22" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">6.</span></p>
            </td>
            <td class="c83" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Resultados de la Prueba de Sistema</span></p>
            </td>
            <td class="c87" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Equipo de Pruebas</span></p>
            </td>
            <td class="c70" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Project Manager</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c22" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">7.</span></p>
            </td>
            <td class="c83" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Reporte Diario/Semanal del Estatus</span></p>
            </td>
            <td class="c87" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Director de Pruebas/ Equipo de Pruebas</span></p>
            </td>
            <td class="c70" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Director de Pruebas/Project Manager</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c22" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">8.</span></p>
            </td>
            <td class="c83" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Reporte de Cierre</span></p>
            </td>
            <td class="c87" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Director de Pruebas</span></p>
            </td>
            <td class="c70" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Project Manager</span></p>
            </td>
        </tr>
    </table>
    <p class="c6"><span class="c18"></span></p>
    <ol class="c3 lst-kix_d3i63clc3lgg-1" start="7">
        <li class="c7 c24 li-bullet-0">
            <h2 id="h.vqt91vksszs0" style="display:inline"><span>Lista de hitos</span><span>&nbsp;</span></h2>
        </li>
    </ol>
    <p class="c7"><span class="c1">La lista de hitos es tentativa y puede cambiar por las siguientes razones</span></p>
    <ol class="c3 lst-kix_4ch1bnhitet1-0 start" start="1">
        <li class="c7 c80 c89 li-bullet-0"><span class="c1">Cualquier problema con la preparaci&oacute;n del entorno del
                Sistema</span></li>
        <li class="c7 c80 c89 li-bullet-0"><span class="c1">Cualquier cambio en el alcance o cosas agregadas al alcance
                del proyecto</span></li>
        <li class="c7 c80 c89 li-bullet-0"><span class="c8">Cualquier otra dependencia que afecte el esfuerzo y el
                tiempo</span></li>
    </ol>
    <p class="c6"><span class="c1"></span></p><a id="t.a8b42f7bd01255e5454370c0238be6d2b5e190d6"></a><a id="t.3"></a>
    <table class="c89 c131">
        <tr class="c13">
            <td class="c0" colspan="1" rowspan="1">
                <p class="c7"><span class="c18">No.</span></p>
            </td>
            <td class="c56" colspan="1" rowspan="1">
                <p class="c7"><span class="c18">Tipo de prueba</span></p>
            </td>
            <td class="c5" colspan="1" rowspan="1">
                <p class="c7"><span class="c18">Ejemplo de Prueba (SUT)</span></p>
            </td>
            <td class="c9" colspan="1" rowspan="1">
                <p class="c7"><span class="c18">Dependencia (DOC)</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c0" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">1</span></p>
            </td>
            <td class="c56" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Pruebas Unitarias</span></p>
            </td>
            <td class="c5" colspan="1" rowspan="1">
                <p class="c7"><span class="c47">Registro de la Plataforma: </span><span class="c1">Probar que el proceso
                        de registro funciona correctamente para cada tipo de usuario.</span></p>
            </td>
            <td class="c9" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">- Base de Datos Completada y conectada. </span></p>
                <p class="c7"><span class="c1">- API Completado y Funcional.</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c0" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">3</span></p>
            </td>
            <td class="c56" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Pruebas Unitarias</span></p>
                <p class="c6"><span class="c1"></span></p>
            </td>
            <td class="c5" colspan="1" rowspan="1">
                <p class="c7"><span class="c47">Login de la Plataforma: </span><span class="c1">Probar que el proceso de
                        Login funciona correctamente para cada tipo de usuario.</span></p>
            </td>
            <td class="c9" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">- Base de Datos Completada y conectada. </span></p>
                <p class="c7"><span class="c1">- API Completado y Funcional.</span></p>
                <p class="c7"><span class="c1">- Configuraci&oacute;n de Autenticaci&oacute;n y
                        Autorizaci&oacute;n</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c0" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">4</span></p>
            </td>
            <td class="c56" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Pruebas Unitarias</span></p>
                <p class="c6"><span class="c1"></span></p>
            </td>
            <td class="c5" colspan="1" rowspan="1">
                <p class="c7"><span class="c47">Modificaci&oacute;n del Cat&aacute;logo:</span><span
                        class="c1">&nbsp;Probar que los usuarios autorizados pueden subir, modificar y eliminar
                        elementos del cat&aacute;logo correctamente.</span></p>
            </td>
            <td class="c9" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">- Base de Datos Completada y conectada.</span></p>
                <p class="c7"><span class="c1">- API Completado y Funcional.</span></p>
                <p class="c7"><span class="c1">- Configuraci&oacute;n de privilegios completada. </span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c0" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">5</span></p>
            </td>
            <td class="c56" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Pruebas Unitarias</span></p>
                <p class="c6"><span class="c1"></span></p>
            </td>
            <td class="c5" colspan="1" rowspan="1">
                <p class="c7"><span class="c47">Funcionalidad de B&uacute;squeda:</span><span class="c1">&nbsp;Probar
                        que los diferentes tipos de usuarios pueden buscar correctamente la informaci&oacute;n que
                        desean mediante la barra de navegaci&oacute;n </span></p>
            </td>
            <td class="c9" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">- Base de Datos Completada y conectada. </span></p>
                <p class="c7"><span class="c1">- API Completado y Funcional.</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c0" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">6</span></p>
            </td>
            <td class="c56" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Pruebas Unitarias</span></p>
                <p class="c6"><span class="c1"></span></p>
            </td>
            <td class="c5" colspan="1" rowspan="1">
                <p class="c7"><span class="c47">Funcionalidad de Filtrado: </span><span class="c1">Probar que los
                        diferentes tipos de usuarios pueden filtrar correctamente la informaci&oacute;n que
                        desean.</span></p>
            </td>
            <td class="c9" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">- Base de Datos Completada y conectada. </span></p>
                <p class="c7"><span class="c1">- API Completado y Funcional.</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c0" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">7</span></p>
            </td>
            <td class="c56" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Pruebas Unitarias</span></p>
                <p class="c6"><span class="c1"></span></p>
            </td>
            <td class="c5" colspan="1" rowspan="1">
                <p class="c7"><span class="c47">Funcionalidad de Pago: </span><span class="c1">Probar el proceso de
                        pagos asegurando que los usuarios pueden completar el pago de un auto de manera f&aacute;cil y
                        segura.</span></p>
            </td>
            <td class="c9" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">- Integraci&oacute;n de la herramienta externa de Pago/Transacciones
                        (Stripe)</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c0" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">8</span></p>
            </td>
            <td class="c56" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Pruebas Unitarias</span></p>
                <p class="c6"><span class="c1"></span></p>
            </td>
            <td class="c5" colspan="1" rowspan="1">
                <p class="c7"><span class="c47">Funcionalidad de Chat: </span><span class="c1">Probar que los diferentes
                        tipos de usuario pueden comunicarse exitosamente entre s&iacute; mediante el Chat interno de la
                        plataforma.</span></p>
            </td>
            <td class="c9" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">- Base de Datos completada y conectada.</span></p>
                <p class="c7"><span class="c1">- Integraci&oacute;n de librer&iacute;a externa para desarrollo del Chat
                        (Socket IO).</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c0" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">9</span></p>
            </td>
            <td class="c56" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Pruebas Unitarias</span></p>
                <p class="c6"><span class="c1"></span></p>
            </td>
            <td class="c5" colspan="1" rowspan="1">
                <p class="c7"><span class="c47">Funcionalidad de Favoritos</span><span class="c1">: Probar que los
                        usuarios puedan seleccionar y guardar sus autos favoritos.</span></p>
            </td>
            <td class="c9" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">- Base de Datos Completada y conectada. </span></p>
                <p class="c7"><span class="c1">- API Completado y Funcional.</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c0" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">10</span></p>
            </td>
            <td class="c56" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Pruebas Unitarias</span></p>
                <p class="c6"><span class="c1"></span></p>
            </td>
            <td class="c5" colspan="1" rowspan="1">
                <p class="c7"><span class="c18">Funcionalidad de An&aacute;lisis de Documentos:</span></p>
                <p class="c7"><span class="c1">Probar que autom&aacute;ticamente se analiza correctamente la validez de
                        un documento.</span></p>
            </td>
            <td class="c9" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">- Integraci&oacute;n de servicio de AWS Textract</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c0" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">11</span></p>
            </td>
            <td class="c56" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Pruebas Unitarias</span></p>
                <p class="c17 c122"><span class="c1"></span></p>
            </td>
            <td class="c5" colspan="1" rowspan="1">
                <p class="c7"><span class="c47">Funcionalidad Anal&iacute;tica: </span><span class="c1">Probar que el
                        dashboard muestre la informaci&oacute;n estad&iacute;stica correcta y adecuada para cada tipo de
                        usuario.</span></p>
            </td>
            <td class="c9" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">- Base de Datos Completada y conectada. </span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c0" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">12</span></p>
            </td>
            <td class="c56" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Pruebas Integrales</span></p>
            </td>
            <td class="c5" colspan="1" rowspan="1">
                <p class="c7"><span class="c18">Manejo de Solicitudes:</span></p>
                <p class="c7"><span class="c1">Probar que la plataforma maneja correctamente y actualiza la
                        informaci&oacute;n referente a el estado de las solicitudes tanto de compra como de prueba de
                        manejo.</span></p>
            </td>
            <td class="c9" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">- Base de Datos Completada y Conectada. </span></p>
                <p class="c7"><span class="c1">- Interfaz de modificaci&oacute;n de solicitudes completada. </span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c0" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">13</span></p>
            </td>
            <td class="c56" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Pruebas Integrales</span></p>
            </td>
            <td class="c5" colspan="1" rowspan="1">
                <p class="c7"><span class="c47">Compra de un auto: </span><span class="c1">Probar que el proceso de
                        compra funciona en todos sus casos (tanto de aprobaci&oacute;n como negaci&oacute;n de la
                        solicitud).</span></p>
            </td>
            <td class="c9" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">- Conexi&oacute;n funcional entre estado de solicitud y cliente.</span>
                </p>
                <p class="c7"><span class="c1">- An&aacute;lisis de documentos completamente funcional.</span></p>
                <p class="c7"><span class="c1">- Sistema de Chat completamente funcional.</span></p>
                <p class="c7"><span class="c1">- Funcional completa del sistema de pagos.</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c0" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">14</span></p>
            </td>
            <td class="c56" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Pruebas Integrales</span></p>
            </td>
            <td class="c5" colspan="1" rowspan="1">
                <p class="c7"><span class="c47">Agendado de una prueba de manejo: </span><span class="c1">Probar que el
                        proceso de agendado de un prueba de manejo funciona en todos sus casos (aprobaci&oacute;n y
                        negaci&oacute;n de la solicitud).</span></p>
            </td>
            <td class="c9" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">- Conexi&oacute;n funcional entre estado de solicitud y cliente.</span>
                </p>
                <p class="c7"><span class="c1">- An&aacute;lisis de documentos completamente funcional.</span></p>
                <p class="c7"><span class="c1">- Sistema de Chat completamente funcional.</span></p>
                <p class="c7"><span class="c1">- Conexi&oacute;n funcional entre agenda del vendedor y el
                        cliente.</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c0" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">15</span></p>
            </td>
            <td class="c56" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Pruebas de Validaci&oacute;n/Aceptaci&oacute;n</span></p>
            </td>
            <td class="c5" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">El dise&ntilde;o (UI/UX) cumple con los est&aacute;ndares del cliente.
                    </span></p>
            </td>
            <td class="c9" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Interfaz de dise&ntilde;o completada.</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c0" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">16</span></p>
            </td>
            <td class="c56" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Pruebas Est&aacute;ticas de Recorrido</span></p>
            </td>
            <td class="c5" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Cada uno de los flujos para cada tipo de usuario se relacionan
                        correctamente entre s&iacute;, y cumplen con los est&aacute;ndares y funcionalidad solicitada
                        por el cliente.</span></p>
            </td>
            <td class="c9" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">- Conexi&oacute;n e integraci&oacute;n completa entre el front-end y
                        back-end.</span></p>
                <p class="c7"><span class="c1">- Configuraciones de seguridad completas.</span></p>
                <p class="c6"><span class="c1"></span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c0" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">17</span></p>
            </td>
            <td class="c56" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Manual de Usuario</span></p>
            </td>
            <td class="c5" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Se documenta el instructivo de uso para cada uno de los flujos de la
                        plataforma.</span></p>
            </td>
            <td class="c9" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">- Software completado y flujo completamente funcional</span></p>
            </td>
        </tr>
    </table>
    <p class="c6 c51"><span class="c121 c132"></span></p>
    <p class="c6 c51 c89"><span class="c121 c132"></span></p>
    <ol class="c3 lst-kix_d3i63clc3lgg-1" start="8">
        <li class="c7 c24 li-bullet-0">
            <h2 id="h.tttcgn6nmo2n" style="display:inline"><span>E</span><span>stimaci&oacute;n de esfuerzo de las
                    pruebas</span></h2>
        </li>
    </ol>
    <p class="c7 c138"><span class="c1">Pruebas Est&aacute;ticas</span></p><a
        id="t.1de78adc822e329353f5d2b478cfd0db52769ad3"></a><a id="t.4"></a>
    <table class="c114">
        <tr class="c13">
            <td class="c135" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Tipo de Prueba</span></p>
            </td>
            <td class="c141" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Horas</span></p>
            </td>
            <td class="c34" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">D&iacute;as</span></p>
            </td>
            <td class="c120" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Porcentaje del Proyecto</span></p>
            </td>
        </tr>
        <tr class="c98">
            <td class="c135" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">SRS</span></p>
            </td>
            <td class="c141" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">56 </span></p>
            </td>
            <td class="c34" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">7</span></p>
            </td>
            <td class="c120" colspan="1" rowspan="2">
                <p class="c4"><span class="c1">6.41%</span></p>
            </td>
        </tr>
        <tr class="c98">
            <td class="c135" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Plan de Pruebas</span></p>
            </td>
            <td class="c141" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">56</span></p>
            </td>
            <td class="c34" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">7 </span></p>
            </td>
        </tr>
    </table>
    <p class="c6 c138"><span class="c1"></span></p>
    <p class="c7 c138"><span class="c8">Pruebas Funcionales</span></p><a
        id="t.58acefe26023bb5ce6a5cee68e4cc83b83aa43d8"></a><a id="t.5"></a>
    <table class="c114">
        <tr class="c13">
            <td class="c54" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Tipo de Prueba</span></p>
            </td>
            <td class="c67" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Horas</span></p>
            </td>
            <td class="c40" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">D&iacute;as</span></p>
            </td>
            <td class="c113" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Porcentaje del Proyecto</span></p>
            </td>
        </tr>
        <tr class="c98">
            <td class="c54" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Pruebas Informales</span></p>
            </td>
            <td class="c67" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">N/A</span></p>
            </td>
            <td class="c40" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">N/A</span></p>
            </td>
            <td class="c113" colspan="1" rowspan="5">
                <p class="c4"><span class="c1">11.68%</span></p>
            </td>
        </tr>
        <tr class="c98">
            <td class="c54" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Pruebas de Integraci&oacute;n</span></p>
            </td>
            <td class="c67" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">28</span></p>
            </td>
            <td class="c40" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">3.5</span></p>
            </td>
        </tr>
        <tr class="c98">
            <td class="c54" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Pruebas de Caja Negra</span></p>
            </td>
            <td class="c67" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">56</span></p>
            </td>
            <td class="c40" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">7</span></p>
            </td>
        </tr>
        <tr class="c98">
            <td class="c54" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Pruebas de Caja Blanca</span></p>
                <p class="c4"><span class="c1">*porcentaje variable dependiendo de qu&eacute; componentes lo
                        necesiten</span></p>
            </td>
            <td class="c67" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">98</span></p>
            </td>
            <td class="c40" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">12.25</span></p>
            </td>
        </tr>
        <tr class="c98">
            <td class="c54" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">Prueba Pen-Testing </span></p>
            </td>
            <td class="c67" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">22</span></p>
            </td>
            <td class="c40" colspan="1" rowspan="1">
                <p class="c4"><span class="c1">2.75</span></p>
            </td>
        </tr>
    </table>
    <p class="c41"><span class="c8">La estimaci&oacute;n de esfuerzos anterior representa un 18.1% del total del
            proyecto.</span></p>
    <p class="c41 c77 c17"><span class="c42"></span></p>
    <ol class="c3 lst-kix_d3i63clc3lgg-0" start="3">
        <li class="c7 c94 c80 c89 li-bullet-0">
            <h1 id="h.rggsbldjdzgj" style="display:inline"><span class="c31">Proceso de gesti&oacute;n de pruebas</span>
            </h1>
        </li>
    </ol>
    <ol class="c3 lst-kix_d3i63clc3lgg-1 start" start="1">
        <li class="c7 c24 li-bullet-0">
            <h2 id="h.l5voq2cnpp4q" style="display:inline"><span class="c16">Proceso de ejecuci&oacute;n de
                    pruebas</span></h2>
        </li>
    </ol>
    <ol class="c3 lst-kix_lmcsya18g09n-0 start" start="1">
        <li class="c84 c60 li-bullet-0"><span class="c1">Aprobaci&oacute;n del plan de pruebas y funcionamiento del
                ambiente de pruebas en todos los dispositivos que ser&aacute;n utilizados.</span></li>
    </ol>
    <ol class="c3 lst-kix_lmcsya18g09n-1 start" start="1">
        <li class="c84 c66 c80 c79 li-bullet-0"><span class="c1">El ambiente de pruebas se comprueba por medio de una
                prueba informal que hagan de manera individual los desarrolladores. </span></li>
    </ol>
    <ol class="c3 lst-kix_lmcsya18g09n-0" start="2">
        <li class="c84 c60 li-bullet-0"><span class="c1">Siguiendo el cronograma del proyecto y el plan de pruebas, el
                project manager en conjunto con el l&iacute;der de pruebas asignar&aacute; a cada l&iacute;der sus
                respectivas pruebas.</span></li>
        <li class="c84 c60 li-bullet-0"><span class="c1">Conforme se finalicen componentes pero el cronograma no indique
                una prueba, los desarrolladores estar&aacute;n a cargo de las pruebas informales, y darles
                seguimiento.</span></li>
        <li class="c84 c60 li-bullet-0"><span class="c1">Cuando se indique la ejecuci&oacute;n de una prueba, cada
                l&iacute;der tiene la responsabilidad de asegurarse de delegar las pruebas a sus equipos y darles
                seguimiento. </span></li>
        <li class="c46 li-bullet-0"><span class="c1">Cada desarrollador encargado de una prueba tiene la responsabilidad
                de documentar su proceso, el resultado de dicha prueba, el seguimiento que se le dar&aacute; y la
                correcci&oacute;n de los errores. </span></li>
    </ol>
    <ol class="c3 lst-kix_lmcsya18g09n-1 start" start="1">
        <li class="c69 c66 li-bullet-0"><span class="c1">El desarrollador tiene la responsabilidad de hacer su proceso
                de QA e informar si se pasa o no la prueba.</span></li>
        <li class="c66 c69 li-bullet-0"><span class="c1">Primero se ejecutar&aacute;n las pruebas de caja negra y en
                caso de que alg&uacute;n componente falle dicha prueba, se aplicar&aacute; la prueba de caja blanca de
                cobertura en general y en alg&uacute;n componente cr&iacute;tico camino b&aacute;sico.</span></li>
        <li class="c69 c66 li-bullet-0"><span class="c1">Una vez que cada componente pase las pruebas unitarias, se
                ejecutar&aacute;n las pruebas de integraci&oacute;n.</span></li>
    </ol>
    <ol class="c3 lst-kix_lmcsya18g09n-0" start="6">
        <li class="c46 li-bullet-0"><span class="c1">El desarrollador tiene la responsabilidad de informar a sus
                respectivos l&iacute;deres acerca del resultado de las pruebas de sus componentes. </span></li>
        <li class="c46 li-bullet-0"><span class="c1">Si hay fallas, se le informar&aacute; a los l&iacute;deres y al
                project manager de acuerdo a la gravedad de ellas y se incluir&aacute;n capturas de pantalla y llenar
                los formularios propuestos, si es necesario.</span></li>
        <li class="c46 li-bullet-0"><span class="c1">Este proceso se repite hasta que todos los casos de prueba se
                ejecuten por completo y tengan un estado en el que ya sea que pasen o fallen.</span></li>
    </ol>
    <ol class="c3 lst-kix_lmcsya18g09n-1 start" start="1">
        <li class="c69 c66 li-bullet-0"><span class="c8">Durante el ciclo siguiente, se probar&aacute;n las pruebas
                falladas corregidas y los resultados se actualizar&aacute;n en el documento durante el ciclo hasta que
                todas las pruebas pasen. El proceso contin&uacute;a hasta que se llegue a un est&aacute;ndar comercial,
                promoviendo fiabilidad, f&aacute;cil acceso y alta estabilidad.</span></li>
    </ol>
    <p class="c6 c79"><span class="c1"></span></p>
    <ol class="c3 lst-kix_d3i63clc3lgg-1" start="2">
        <li class="c2 c94 c80 li-bullet-0">
            <h2 id="h.nsa8lxrnmxkd" style="display:inline"><span>Riesgos de prueba y factores de
                    mitigaci&oacute;n</span></h2>
        </li>
    </ol><a id="t.631e0a8bdeec5841d70663f7694b22eef0646943"></a><a id="t.6"></a>
    <table class="c131 c159">
        <tr class="c13">
            <td class="c0" colspan="1" rowspan="1">
                <p class="c7"><span class="c18">ID</span></p>
            </td>
            <td class="c117" colspan="1" rowspan="1">
                <p class="c7"><span class="c18">Riesgo</span></p>
            </td>
            <td class="c111" colspan="1" rowspan="1">
                <p class="c7"><span class="c18">Descripci&oacute;n</span></p>
            </td>
            <td class="c44" colspan="1" rowspan="1">
                <p class="c7"><span class="c18">Acciones de Mitigaci&oacute;n</span></p>
            </td>
            <td class="c105" colspan="1" rowspan="1">
                <p class="c7"><span class="c18">Probabilidad</span></p>
            </td>
            <td class="c73" colspan="1" rowspan="1">
                <p class="c7"><span class="c18">Impacto</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c0" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">R_01</span></p>
            </td>
            <td class="c117" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Latencia en el acceso al GitHub </span></p>
            </td>
            <td class="c111" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Al ser Github la plataforma en la que compartimos y organizamos nuestros
                        avances, si existe alg&uacute;n error en la plataforma o si nosotros cometemos alg&uacute;n
                        error, nuestro repositorio puede perder informaci&oacute;n o perderse por completo</span></p>
            </td>
            <td class="c44" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">- Regresar a la versi&oacute;n m&aacute;s estable dentro del historial de
                        versiones </span></p>
                <p class="c7"><span class="c1">- Utilizar la versi&oacute;n de alguien del equipo que no haya </span>
                </p>
            </td>
            <td class="c105" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Media</span></p>
            </td>
            <td class="c73" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Alta</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c0" colspan="1" rowspan="1">
                <p class="c7"><span class="c8">R_02</span></p>
            </td>
            <td class="c117" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Que no se d&eacute; el presupuesto necesario para el hosting de la
                        plataforma en la nube</span></p>
            </td>
            <td class="c111" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Los servicios de cloud son costosos pero garantizan seguridad y
                        escalabilidad, se debe de llegar a un acuerdo con el Tec para el uso de estos servicios</span>
                </p>
            </td>
            <td class="c44" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">- Contar con alternativas gratuitas de respaldo o cuentas con
                        &quot;trial&quot; del servicio con suficiente alcance de tiempo para la entrega del
                        proyecto.</span></p>
                <p class="c7"><span class="c1">- Uso del servidor</span></p>
            </td>
            <td class="c105" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Media</span></p>
            </td>
            <td class="c73" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Alta</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c0" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">R_ 03</span></p>
            </td>
            <td class="c117" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Inclusi&oacute;n de nuevos miembros al equipo</span></p>
            </td>
            <td class="c111" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Debido a la naturaleza del proyecto, de 4 equipos se formar&aacute;
                        s&oacute;lo un equipo, por lo que &nbsp;la integraci&oacute;n de las ideas y los integrantes
                        puede resultar retadora</span></p>
            </td>
            <td class="c44" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">- En cuanto sea detectado, restringir el acceso por completo al
                        individuo</span></p>
                <p class="c7"><span class="c1">- Contactar a las autoridades</span></p>
                <p class="c7"><span class="c1">- Contactar al equipo legal</span></p>
            </td>
            <td class="c105" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Media</span></p>
            </td>
            <td class="c73" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Alta</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c0" colspan="1" rowspan="1">
                <p class="c7"><span class="c8">R_04</span></p>
            </td>
            <td class="c117" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Divergencia entre los distintos ambientes de desarrollo </span></p>
            </td>
            <td class="c111" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Ya que se utilizar&aacute;n diferentes librer&iacute;as y dependencias,
                        si el sistema operativo del dispositivo de alg&uacute;n integrante no es compatible con dichos
                        componentes, el desarrollo de la aplicaci&oacute;n puede retrasarse y la productividad y
                        participaci&oacute;n del integrante puede verse afectada. </span></p>
            </td>
            <td class="c44" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">- Utilizar un docker o una m&aacute;quina virtual</span></p>
                <p class="c7"><span class="c1">- Estandarizar un ambiente de desarrollo</span></p>
            </td>
            <td class="c105" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Media</span></p>
            </td>
            <td class="c73" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Media</span></p>
            </td>
        </tr>
    </table>
    <p class="c6"><span class="c43"></span></p>
    <p class="c6"><span class="c1"></span></p>
    <p class="c6"><span class="c1"></span></p>
    <ol class="c3 lst-kix_d3i63clc3lgg-1" start="3">
        <li class="c2 c94 c80 li-bullet-0">
            <h2 id="h.5h8w5mqda6gh" style="display:inline"><span>Plan de comunicaciones y lista de equipos</span></h2>
        </li>
    </ol><a id="t.113000c59697455fb59036e97da4ef320a61d27c"></a><a id="t.7"></a>
    <table class="c114">
        <tr class="c13">
            <td class="c64" colspan="1" rowspan="1">
                <p class="c7"><span class="c18">Rol</span></p>
            </td>
            <td class="c75" colspan="1" rowspan="1">
                <p class="c7"><span class="c18">Descripci&oacute;n</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c64" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Project Manager </span></p>
            </td>
            <td class="c75" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">El miembro que est&aacute; a cargo de un equipo. Deben organizar y
                        planificar las tareas del equipo para que el proyecto tenga &eacute;xito, asegur&aacute;ndose de
                        que se entreguen en tiempo, forma y retroalimentadas. </span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c64" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">L&iacute;der de Pruebas</span></p>
            </td>
            <td class="c75" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Miembro del equipo que es responsable de participar y supervisar el
                        desarrollo de las pruebas. Debe de tener en cuenta todos los alcances y criterios de
                        validaci&oacute;n de cada prueba para asegurarse de que se cumplan en tiempo y forma. </span>
                </p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c64" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">L&iacute;der de Back-End</span></p>
            </td>
            <td class="c75" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Miembro del equipo que es responsable de participar y supervisar el
                        desarrollo del back-end. Debe coordinar con todos los equipos de desarrollo el avance y los
                        componentes del proyecto, asignar tareas, asegurarse de que se completen en tiempo y forma y
                        coordinarse con el project manager.</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c64" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">L&iacute;der de Front-End</span></p>
            </td>
            <td class="c75" colspan="1" rowspan="1">
                <p class="c7"><span class="c8">Miembro del equipo que es responsable de participar y supervisar el
                        desarrollo del front-end. Debe coordinar con todos los equipos de desarrollo, el avance y los
                        componentes del proyecto, asignar tareas, asegurarse de que se completen en tiempo y forma y
                        coordinarse con el project manager.</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c64" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">L&iacute;der de Base de Datos</span></p>
            </td>
            <td class="c75" colspan="1" rowspan="1">
                <p class="c7"><span class="c8">Miembro del equipo que es responsable de participar y supervisar el
                        desarrollo de la base de datos. Debe coordinar con todos los equipos de desarrollo, el avance y
                        los componentes del proyecto, asignar tareas, asegurarse de que se completen en tiempo y forma y
                        coordinarse con el project manager.</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c64" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">L&iacute;der de Seguridad</span></p>
            </td>
            <td class="c75" colspan="1" rowspan="1">
                <p class="c7"><span class="c8">Miembro del equipo que es responsable de participar y supervisar la
                        protecci&oacute;n de los diferentes aspectos del proyecto y la autenticaci&oacute;n de los
                        usuarios. Debe coordinar con todos los equipos de desarrollo, el avance y los componentes del
                        proyecto, asignar tareas, asegurarse de que se completen en tiempo y forma y coordinarse con el
                        project manager.</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c64" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">Equipo de Desarrollo</span></p>
            </td>
            <td class="c75" colspan="1" rowspan="1">
                <p class="c7"><span class="c1">C&eacute;lula de trabajo encargada de requerimientos espec&iacute;ficos,
                        compuesta de un miembro de back-end, uno de front-end, uno de base de datos, uno de seguridad,
                        de pruebas y un project manager.</span></p>
            </td>
        </tr>
    </table>
    <p class="c6"><span class="c1"></span></p>
    <h3 class="c7 c94" id="h.shiwdz2v0drx"><span>Expectativas del Rol </span></h3>
    <p class="c38 c61"><span class="c1">Es importante aclarar que dentro del proyecto presente, todos los involucrados
            en el desarrollo de la aplicaci&oacute;n cumpliran un rol como tester a pesar de las responsabilidades que
            tengan en otro rol. Por lo antes mencionado, por cada componente que sea finalizado por cualquier persona en
            el equipo de desarrollo se realizar&aacute; una prueba informal. De la misma manera, todo el equipo de
            desarrollo tiene como responsabilidad validar con el cliente los componentes de la aplicaci&oacute;n y el
            entregable final.</span></p>
    <p class="c38 c17 c61"><span class="c1"></span></p>
    <p class="c38 c61"><span class="c1">La siguiente lista define en t&eacute;rminos generales las expectativas
            relacionadas a los roles que est&aacute;n involucrados con el manejo, planeaci&oacute;n o ejecuci&oacute;n
            de la prueba para el proyecto. </span></p>
    <p class="c38 c61 c17"><span class="c1"></span></p>
    <h3 class="c7 c74" id="h.vajm4pu401qs"><span class="c149">Project Manag</span><span>er </span></h3>
    <p class="c7 c59"><span class="c8">R</span><span class="c1">evisa el contenido de</span><span class="c1">l plan de
            pruebas, la estrategia de las pueblas, los estimados, criterios de validaci&oacute;n con los equipos de
            trabajo, l&iacute;deres y los stakeholders. Recopila la retroalimentaci&oacute;n e informa a los
            dem&aacute;s. Tiene la responsabilidad de darle acompa&ntilde;amiento a las pruebas de caja blanca.</span>
    </p>
    <p class="c6 c59"><span class="c1"></span></p>
    <h3 class="c7 c74" id="h.cup1cc33x1cr"><span class="c16">L&iacute;der de Pruebas </span></h3>
    <p class="c38 c59"><span class="c1">Junto con el project manager, crea y revisa el contenido del plan de pruebas, la
            estrategia de las pueblas, los estimados y criterios de validaci&oacute;n coordinando la ejecuci&oacute;n
            con las actividades programadas en el cronograma del proyecto. Recibe retroalimentaci&oacute;n de los
            equipos de trabajo, l&iacute;deres y los stakeholders, se asegura que las pruebas se ejecuten en tiempo y
            forma y documenta el proceso y los resultados.</span></p>
    <p class="c6 c59"><span class="c1"></span></p>
    <h3 class="c7 c74" id="h.15iz1ry18o"><span class="c16">L&iacute;der de Back-End </span></h3>
    <p class="c38 c59"><span class="c8">Junto con el l&iacute;der de pruebas y el project manager, suma al contenido del
            plan de pruebas considerando las actividades programadas para el desarrollo del back-end, el avance del
            mismo y se asegura de la ejecuci&oacute;n de las pruebas de sus componentes y que la integraci&oacute;n con
            los otros equipos sea probada y documentada. Se le asignan pruebas, es parte y </span><span
            class="c8">delega</span><span class="c1">&nbsp;dichas pruebas y se asegura que las funcionalidades
            cr&iacute;ticas de su desarrollo sean consideradas como parte del plan de pruebas. Tiene un seguimiento de
            las pruebas informales que sus desarrolladores han ejecutado. </span></p>
    <p class="c6 c59"><span class="c1"></span></p>
    <p class="c7 c59"><span class="c8">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span
            class="c16">L&iacute;der de Front-End </span></p>
    <p class="c38 c59"><span class="c8">Junto con el l&iacute;der de pruebas y el project manager, suma al contenido del
            plan de pruebas considerando las actividades programadas para el desarrollo del front-end, el avance del
            mismo y se asegura de la ejecuci&oacute;n de las pruebas de sus componentes y que la integraci&oacute;n con
            los otros equipos sea probada y documentada. Se le asignan pruebas, es parte y </span><span
            class="c8">delega</span><span class="c1">&nbsp;dichas pruebas y se asegura que las funcionalidades
            cr&iacute;ticas de su desarrollo sean consideradas como parte del plan de pruebas. Tiene un seguimiento de
            las pruebas informales que sus desarrolladores han ejecutado. </span></p>
    <p class="c6 c59"><span class="c1"></span></p>
    <p class="c7 c59 c85"><span class="c16">L&iacute;der de Base de Datos </span></p>
    <p class="c38 c59"><span class="c8">Junto con el l&iacute;der de pruebas y el project manager, suma al contenido del
            plan de pruebas considerando las actividades programadas para el desarrollo de la base de datos, el avance
            de la misma y se asegura de la ejecuci&oacute;n de las pruebas de sus componentes y que la
            integraci&oacute;n con los otros equipos sea probada y documentada. Se le asignan pruebas, es parte y
        </span><span class="c8">delega</span><span class="c1">&nbsp;dichas pruebas y se asegura que las funcionalidades
            cr&iacute;ticas de su desarrollo sean consideradas como parte del plan de pruebas. Tiene un seguimiento de
            las pruebas informales que sus desarrolladores han ejecutado. </span></p>
    <p class="c6 c59"><span class="c1"></span></p>
    <p class="c7 c59 c85"><span class="c16">L&iacute;der de Seguridad </span></p>
    <p class="c7 c59"><span class="c8">Junto con el l&iacute;der de pruebas y el project manager, suma al contenido del
            plan de pruebas considerando las actividades programadas para la protecci&oacute;n de los diferentes
            aspectos del proyecto y la autenticaci&oacute;n de los usuarios, y se asegura de la ejecuci&oacute;n de las
            pruebas de sus componentes y que la integraci&oacute;n con los otros equipos sea probada y documentada. Se
            le asignan pruebas, es parte y </span><span class="c8">delega</span><span class="c1">&nbsp;dichas pruebas y
            se asegura que las funcionalidades cr&iacute;ticas de su desarrollo sean consideradas como parte del plan de
            pruebas. Tiene un seguimiento de las pruebas informales que sus desarrolladores han ejecutado.</span></p>
    <p class="c6 c59"><span class="c1"></span></p>
    <p class="c7 c59 c85"><span class="c16">Equipo de Desarrollo / Testers</span></p>
    <p class="c7 c59"><span class="c8">Junto con sus respectivos l&iacute;deres ejecutan las diferentes pruebas
            establecidas en el plan y se aseguran de que estas sean ejecutadas en el mismo ambiente siguiendo la
            metodolog&iacute;a. Proveen y dan seguimiento a la retroalimentaci&oacute;n y documentan el proceso y los
            resultados, as&iacute; garantizando un proceso de QA transparente. Informan a los l&iacute;deres si existe
            alg&uacute;n problema o si alg&uacute;n componente necesita ser corregido, se encargan de hacer las pruebas
            en tiempo y forma (de acuerdo al cronograma), llevan un seguimiento de sus pruebas informales y corrigen sus
            funcionalidades. Cada integrante del desarrollo tiene la responsabilidad de realizar sus pruebas asignadas
            de caja negra y junto con el SCRUM Master y el Project Manager realizar las pruebas de caja blanca. </span>
    </p>
    <p class="c6 c101"><span class="c1"></span></p>
    <h3 class="c7 c94" id="h.bpgnszel0u1j"><span class="c16">Cronograma de Actividades</span></h3>
    <p class="c66 c92"><span class="c123"><a class="c14"
                href="https://www.google.com/url?q=https://tec95061.monday.com/boards/4072044099/views/92404971&amp;sa=D&amp;source=editors&amp;ust=1678937540028783&amp;usg=AOvVaw1REvMm1lzWUhq5J_mqmRyB">Gantt
                (Monday.com)</a></span></p>
    <p class="c6 c126"><span class="c47 c106"></span></p>
    <ol class="c3 lst-kix_d3i63clc3lgg-0" start="4">
        <li class="c7 c94 c80 c89 li-bullet-0">
            <h1 id="h.6ngo7ertvrlx" style="display:inline"><span class="c86">Ambiente de pruebas</span></h1>
        </li>
    </ol>
    <ul class="c3 lst-kix_6tpu3jq5w4b9-0 start">
        <li class="c7 c28 c80 li-bullet-0"><span class="c1">El entorno de prueba consistir&aacute; en un entorno de
                Windows 11 como m&iacute;nimo, un n&uacute;cleo Intel i5 o equivalente; 8 GB de RAM.</span></li>
        <li class="c7 c28 c80 li-bullet-0"><span class="c1">Se utilizar&aacute;n los servicios de AWS, donde se busca
                alojar la aplicaci&oacute;n web y la base de datos. </span></li>
        <li class="c7 c28 c80 li-bullet-0"><span class="c1">Todos los testers trabajaran en la misma versi&oacute;n de
                la aplicaci&oacute;n y base de datos y tendr&aacute;n las mismas versiones del software utilizado
                (incluyendo las librer&iacute;as y dependencias).</span></li>
        <li class="c7 c28 c80 li-bullet-0"><span class="c8">En caso de ser necesario se usar&aacute; docker para poder
                ejecutar las pruebas y estandarizar el ambiente de trabajo.</span></li>
    </ul>
    <p class="c6 c28"><span class="c1 c93"></span></p>
    <ol class="c3 lst-kix_d3i63clc3lgg-0" start="5">
        <li class="c7 c94 c80 c89 li-bullet-0">
            <h1 id="h.e0bh1ws8hyem" style="display:inline"><span>Pruebas</span></h1>
        </li>
    </ol>
    <h1 class="c38 c94" id="h.1cv9qoiaynm6"><span class="c1">Esto se llenar&aacute; con la fase de despliegue de la
            unidad de formaci&oacute;n &ldquo;TC30005B&rdquo;. A continuaci&oacute;n, la propuesta de templates que se
            utilizar&aacute;n para als diferentes pruebas mencionadas.</span></h1>
    <p class="c41"><span class="c18">Template Recorrido</span></p>
    <p class="c41"><span class="c1">Nombre del Tester: </span></p>
    <p class="c41"><span class="c1">Nombre Moderador:</span></p><a
        id="t.5c3fd7b5b5c2964139b4da330dfb4dde61007c23"></a><a id="t.8"></a>
    <table class="c68">
        <tr class="c13">
            <td class="c128 c115" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">ID</span></p>
            </td>
            <td class="c109 c115" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Paso</span></p>
            </td>
            <td class="c52" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Descripci&oacute;n</span></p>
            </td>
            <td class="c115 c130" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Resultado Esperado</span></p>
            </td>
            <td class="c107 c115" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Resultado Actual</span></p>
            </td>
            <td class="c124 c115" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Observaciones</span></p>
            </td>
            <td class="c45" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Pasa o No Pasa</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c128" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c109" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c144" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c130" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c107" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c124" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c151" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
        </tr>
    </table>
    <p class="c41 c17"><span class="c18"></span></p>
    <p class="c41"><span class="c18">Template Caja Negra</span></p>
    <p class="c41"><span class="c1">Nombre del Tester:</span></p>
    <p class="c41"><span class="c1">Nombre de la Funci&oacute;n/Componente:</span></p><a
        id="t.a134dc50ad5257a23a6b5de875804a821412e18d"></a><a id="t.9"></a>
    <table class="c65">
        <tr class="c13">
            <td class="c97 c115" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">ID</span></p>
            </td>
            <td class="c115 c119" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Descripci&oacute;n</span></p>
            </td>
            <td class="c63" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Resultado Esperado</span></p>
            </td>
            <td class="c26" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Par&aacute;metro 1</span></p>
            </td>
            <td class="c12" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Par&aacute;metro 2</span></p>
            </td>
            <td class="c100" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Resultado Actual</span></p>
            </td>
            <td class="c81" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Observaciones</span></p>
            </td>
            <td class="c63" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Pasa o No Pasa</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c97" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c119" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c134" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c133" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c55" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c158" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c99" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c134" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
        </tr>
    </table>
    <p class="c17 c41"><span class="c18"></span></p>
    <p class="c41"><span class="c18">Template Caja Blanca</span></p>
    <p class="c41"><span class="c1">Nombre del Tester: </span></p>
    <p class="c41"><span class="c1">Nombre de la Funci&oacute;n/Componente:</span></p><a
        id="t.692b1d0e20634d52bcf95890f959936b1a99e397"></a><a id="t.10"></a>
    <table class="c58">
        <tr class="c13">
            <td class="c102" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">ID</span></p>
            </td>
            <td class="c52" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Descripci&oacute;n</span></p>
            </td>
            <td class="c96" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">L&iacute;nea de C&oacute;digo</span></p>
            </td>
            <td class="c116 c115" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Resultado Esperado</span></p>
            </td>
            <td class="c72" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Resultado Actual</span></p>
            </td>
            <td class="c96" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Observaciones</span></p>
            </td>
            <td class="c26" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Pasa o No Pasa</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c139" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c144" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c118" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c116" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c129" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c118" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c133" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
        </tr>
    </table>
    <p class="c41 c17"><span class="c18"></span></p>
    <p class="c41"><span class="c18">Template Integraci&oacute;n</span></p>
    <p class="c41"><span class="c1">Nombre del Tester:</span></p>
    <p class="c41"><span class="c1">Nombre &nbsp;del Supervisor:</span></p>
    <p class="c41"><span class="c1">Nombre de las Funciones/Componentes:</span></p><a
        id="t.71b7b10cbdb2b10d42cf8ef877c04333de3b7a5f"></a><a id="t.11"></a>
    <table class="c65">
        <tr class="c13">
            <td class="c27 c115" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">ID M&oacute;dulos</span></p>
            </td>
            <td class="c119 c115" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Descripci&oacute;n de la</span></p>
                <p class="c4"><span class="c18">Relaci&oacute;n</span></p>
            </td>
            <td class="c90 c115" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Resultado Esperado</span></p>
            </td>
            <td class="c39 c115" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Par&aacute;metro 1</span></p>
            </td>
            <td class="c39 c115" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Par&aacute;metro 2</span></p>
            </td>
            <td class="c48" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Resultado Actual</span></p>
            </td>
            <td class="c81" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Observaciones</span></p>
            </td>
            <td class="c63" colspan="1" rowspan="1">
                <p class="c4"><span class="c18">Pasa o No Pasa</span></p>
            </td>
        </tr>
        <tr class="c13">
            <td class="c27" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c119" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c90" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c39" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c39" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c137" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c99" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
            <td class="c134" colspan="1" rowspan="1">
                <p class="c4 c17"><span class="c18"></span></p>
            </td>
        </tr>
    </table>
    <p class="c41 c17"><span class="c18"></span></p>
    <p class="c41 c17"><span class="c18"></span></p>
    <ol class="c3 lst-kix_d3i63clc3lgg-0" start="6">
        <li class="c7 c94 c80 c89 li-bullet-0">
            <h1 id="h.j9dbb7pex1fz" style="display:inline"><span>Conclusiones</span></h1>
        </li>
    </ol>
    <p class="c38 c85"><span class="c1">En conclusi&oacute;n, la aplicaci&oacute;n de un plan de pruebas exhaustivo es
            esencial para el &eacute;xito del proyecto, sobre todo al tratarse de desarrollo de software. Esto ya que
            las pruebas continuas y sistematizadas &nbsp;permiten identificar as&iacute; como abordar posibles problemas
            emergentes antes de que se conviertan en riesgos &nbsp;mayores. Con acceso al documento del plan de pruebas,
            los miembros del equipo tendr&aacute;n una comprensi&oacute;n clara de los requisitos y expectativas del
            proyecto, que puede servir de gu&iacute;a para la toma de decisiones y la resoluci&oacute;n de
            problemas.</span></p>
    <p class="c38 c85"><span class="c1">El compromiso tanto del equipo de pruebas como de los desarrolladores, es
            crucial para la aplicaci&oacute;n eficaz de este plan de pruebas. La adhesi&oacute;n a los contenidos
            acordados del documento garantiza que todos est&eacute;n en la misma p&aacute;gina y trabajen por el mismo
            objetivo, as&iacute; facilitando un desarrollo fluido y el cumplimiento de los planes elaborados antes de la
            implantaci&oacute;n.</span></p>
    <p class="c38 c85"><span class="c1">Asimismo, el plan de pruebas puede ayudar al equipo a evaluar y mejorar el
            rendimiento general del proyecto. Mediante el seguimiento del progreso y la identificaci&oacute;n de
            &aacute;reas de mejora, el equipo puede perfeccionar el plan del proyecto, optimizar los recursos y mejorar
            la eficiencia general del proyecto. En t&eacute;rminos generales, la aplicaci&oacute;n de un plan de pruebas
            exhaustivo es esencial para el &eacute;xito de cualquier proyecto. Con pruebas continuas, directrices claras
            y el compromiso de los miembros del equipo, el proyecto puede entregarse a tiempo, dentro del presupuesto y
            con la calidad esperada.</span></p>
    <div>
        <p class="c17 c57"><span class="c42"></span></p>
    </div>
</body>

</html>