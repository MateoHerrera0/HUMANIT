<p align="center">
  <img src="../Logos/humanIT.005.png" width="300" title="hover text">
</p>
<hr/>

<h2 align="center"> Completa Digitalización del Proceso de Adquisición de un Vehículo 

<h2 align="center"> Software 
Requirements Specification

<h2 align="center"> Versión 2.0

| Date            | Version       | Description  |  
| -------------   |:-------------:| :----------- |
| 26/02/2023      | 0.1           | Creation of document SRS|                          
| 01/03/2023      | 0.2           | Doc in Markdown|      
|                 |               |              |      

<h2 align="center"> Authors
<h3 align="center"> Andreína Sanánez
<h3 align="center"> Karla Mondragón
<h3 align="center"> Mateo Herrera 
<h3 align="center"> Regina Rodríguez
<h3 align="center"> Salvador Milanés

<h1 align="center"> Software Requirements Specification

# Índice
1. [Introducción](#1-introducción)
        
    1.1. [Propósito](#11-propósito)

    1.2. [Enfoque y Alcance](#12-enfoque-y-alcances)

    1.3. [Objetivos SMART](#13-objetivos-smart)

2. [Requerimientos](#2-requerimientos)

    2.1. [Requerimientos Funcionales](#21-requerimientos-funcionales)

    2.2. [Requerimientos No Funcionales](#22-requerimientos-no-funcionales)

    2.3. [Restricciones](#23-restricciones)

3. [Arquitectura](#3-arquitectura) 

    3.1. [Diagrama de Arquitectura](#31-diagrama-de-arquitectura)
    
    3.2. [Technological Stack](#32-stack-tecnológico)

# 1. Introducción 
<p align="justify"> El objetivo de este documento es recopilar, analizar y brindar una visión profunda de la aplicación web para NDS Cognitive Labs, definiendo el problema y la solución en detalle. El documento también concentra las capacidades requeridas por todos los stakeholders y sus necesidades definiendo las características del producto.

<p align="justify"> Nuestra misión para este proyecto es hacer el proceso de compra de un auto de la forma más fácil y conveniente para el usuario haciéndolo completamente en línea.Esto planeamos lograrlo creando una plataforma confiable, transparente y de fácil acceso en la que los clientes puedan tomar decisiones informadas basadas en información confiable y recomendaciones profesionales. Nuestro compromiso con nuestros clientes es ofrecerles una gama variada de autos a través de agencias y grupos automotrices previamente verificadas en nuestra plataforma.

<p align="justify"> Con respecto a nuestra visión, buscamos transformar radicalmente el sector de ventas de autos. Con este proyecto queremos que la experiencia tradicional de la compra de autos cambie por completo y sea de una manera completamente digital y sin estrés. Estamos comprometidos a crear una comunidad confiable de vendedores y compradores donde las transacciones pueden ser completamente en línea, quitando los problemas e inconvenientes asociados a la compra tradicional de autos. 

## 1.1. Propósito
<p align="justify"> El propósito del documento es recopilar y analizar todas las ideas que han surgido para definir el sistema y sus requisitos con respecto a los usuarios que harán uso de la aplicación. 

<p align="justify"> En este proyecto en colaboración con NDS Cognitive Labs, se busca la completa digitalización del proceso de adquisición de vehículos nuevos y seminuevos. La problemática que se busca resolver es agilizar un proceso que se ha vuelto inconveniente y tedioso: la compra de un vehículo. Dicho proceso presenta múltiples inconvenientes desde que no todas las agencias tienen el catálogo completo de autos disponibles hasta la cercanía entre las agencias y el comprador. Nuestra propuesta busca:
<ul>
    <li> La completa transparencia en los procesos de compra 
    <li> Un diseño intuitivo y funcional
    <li> Un proceso de compra amigable y conveniente
    <li> La completa protección de datos de usuarios
</ul>

## 1.2. Enfoque y Alcances
<p align="justify"> Por medio de una aplicación web que fomente la convivencia entre diferentes agencias, grupos automotrices y marcas se espera que el usuario sea capaz de elegir un vehículo desde un amplio catálogo, encuentre planes de financiamiento que se adapten a sus necesidades y que cuente con una plataforma con diversas formas de pago. El usuario puede solicitar una prueba de manejo si así lo desea y comprar su vehículo en cualquier agencia disponible y puede comunicarse con una agencia (vendedor específico) por medio de un chat en tiempo real.

<p align="justify"> Nuestra aplicación busca habilitar permisos de usuarios y roles administrativos. La plataforma permitirá a usuarios administradores subir catálogos de autos y a sus clientes navegar los mismos. Los clientes también serán capaces de subir los documentos legales requeridos y toda la información solicitada estará encriptada y protegida. La plataforma tendrá una interfaz intuitiva para que los usuarios puedan buscar y filtrar autos de un catálogo, comparar opciones seleccionadas y ver sus especificaciones.

<p align="justify"> Lo que nos diferencia de la competencia es nuestra intención de crear un simulador Comparativo de autos, dar recomendaciones personalizadas con Machine Learning y la implementación de un "Wishlist" (Bookmark de autos preferidos). Algunos aspectos de la solución que nosotros como HumanIT Consulting no cubriremos son el mantenimiento de la aplicación, el servicio y patrocinio del almacenamiento en Cloud y la solución de quejas acerca de la manufactura o el estado de los automóviles.

## 1.3. Objetivos SMART
1. _Mejorar la experiencia del usuario:_ para fines de junio 2023, con el lanzamiento de la aplicación, buscamos reducir a la mitad, el tiempo que le toma a un usuario finalizar la compra de un automóvil en la plataforma acelerando el proceso de pago y mejorando la interfaz de usuario.
2. _Mejorar el servicio al cliente:_ para mediados de abril 2023, se busca implementar un chatbot que pueda ofrecer ayuda las 24 horas, los 7 días de la semana y reducir a la mitad los tiempos de respuesta a las consultas de los clientes. Esto mejorará el servicio al cliente en la plataforma.
3. _Aumentar las opciones de pago:_ para fines de mayo de 2023, se busca incluir una pasarela de pago que acepte más formas de pago para ampliar la cantidad de alternativas de pago disponibles para los clientes en la plataforma.
4. _Aumentar el posicionamiento en los motores de búsqueda:_ para fines de mayo de 2023, se utilizarán mejores prácticas de optimización de motores de búsqueda para aumentar el ranking de la plataforma.
5. _Mejorar la seguridad de la plataforma:_ para evitar violaciones de datos y garantizar la privacidad del consumidor, se agregara autenticación y la verificación de autorización y se incluirá el cifrado de datos para fines de abril de 2023. 
6. _Implemente análisis predictivos:_ uso de análisis predictivo para fines de junio de 2023 con el objetivo de estudiar los datos de los clientes y ofrecer sugerencias de automóviles individuales, lo que lleva a un aumento en la satisfacción del cliente.

## 1.4. Definiciones, Acrónimos y Abreviaciones
| Concepto   | Descripción       |  
| :---------:|:-------------     | 
| SQL        | Structured Query Language, lenguaje de programación para almacenar y procesar información en una base de datos relacional|                           
| API        | Application Programming Interface, conjunto de definiciones y protocolos que se usa para diseñar e integrar el software de las aplicaciones|      
| BD o DB    | Base de Datos o Database|   
| AWS        | Amazon Web Services, colección de servicios de computación en la nube pública que en conjunto forman una plataforma de computación en la nube, ofrecidas a través de Internet por Amazon.com|  

# 2. Requerimientos 
## 2.1. WBS
1. Versión 1: 
<table cellspacing="0" cellpadding="0">
        <thead>
            <tr>
                <th colspan="2">Project Definition</th>
                <th class="s2" dir="ltr" colspan="2">Project Development</th>
                <th class="s3" dir="ltr" colspan="2">Validation</th>
                <th class="s4" dir="ltr" colspan="2">Deployment</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>1. Scope<br> 1.1. Requirement Definition<br> 1.1.1. Functional<br> 1.1.2.
                    Non-Functional<br> 1.2. System Map<br> 1.3. Epics</td>
                <td>All</td>
                <td>1. Project Initialization <br> 1.1. Set up working env<br> 1.2. Install
                    Dependencies<br> 1.3. Configure Source Control<br><br><br></td>
                <td class="s7" dir="ltr"><br>K &amp; S<br>K &amp; S<br>K &amp; S<br><br><br></td>
                <td>1. Beta Testing<br> 1.1. Unit Test<br> 1.2. Integral Test<br> 1.3. White Box
                    Testing<br> 1.4. Black Box Testing<br> 1.5. General Pentesting Round</td>
                <td><br>K &amp; R &amp; S<br>K &amp; R &amp; S<br>K &amp; R &amp; S &amp; M<br>K
                    &amp; R<br>K &amp; M<br></td>
                <td>1. Feedback</td>
                <td>All</td>
            </tr>
            <tr>
                <td class="s5" dir="ltr">2. Design<br> 2.1. Tech Stack Definition<br> 2.2. Architecture Diagram<br> 2.3.
                    User Stories<br> 2.4. Process Diagram<br><br></td>
                <td class="s6" dir="ltr"><br><br><br><br><br><br><br>All<br></td>
                <td class="s11" dir="ltr">2. Backend<br> 2.1. Payment Implementation<br> 2.2. Design data structures<br>
                    2.3. API Creation<br> 2.3.1. End-points design<br> 2.3.2. Database Connection<br> 2.4. Hooks for
                    account creation <br> 2.5. Hooks for data visualisation<br> 2.6. Roles implementation <br> 2.6.1.
                    Hierarchy Implementation<br> 2.6.2. Access Restriction <br> 2.6.3. Principle of Least Privilege and
                    filtering<br> 2.7. Front-end Connection<br><br><br><br></td>
                <td class="s7" dir="ltr"><br>A &amp; S &amp; K<br>A &amp; S<br>A &amp; S &amp; M<br><br><br>A &amp;
                    S<br>A &amp; S<br>A &amp; S &amp; K &amp; M<br><br><br><br><br><br>A &amp; S &amp; K &amp;
                    R<br><br><br><br></td>
                <td></td>
                <td class="s12"></td>
                <td class="s10" dir="ltr">2. Debugging</td>
                <td class="s10" dir="ltr">All</td>
            </tr>
            <tr style="height: 20px">
                <td class="s5" dir="ltr">3. Documentation<br> 3.1. Budgeting<br> 3.2. SRS<br><br><br></td>
                <td class="s6" dir="ltr"><br>All<br>K<br><br><br></td>
                <td class="s7" dir="ltr">3. Frontend<br> 3.1. Wireframe design<br> 3.2. App Mock-up<br> 3.3. React
                    Implementation<br> 3.4. Views for roles<br> 3.5. Local Asset Sourcing </td>
                <td class="s7" dir="ltr"><br>R<br>R &amp; K<br>M&amp; K &amp; S &amp; R<br>R &amp; K &amp; S<br>R &amp;
                    K</td>
                <td></td>
                <td class="s12"></td>
                <td class="s10" dir="ltr">3. Cloud Deployment</td>
                <td class="s10" dir="ltr">M &amp; S</td>
            </tr>
            <tr style="height: 20px">
                <td class="s13"></td>
                <td class="s7" dir="ltr">4. Database<br> 4.1. Database Design<br> 4.1.1. Class Diagram<br> 4.1.2.
                    Entity-Relation Diagram<br> 4.2. Database Programming<br> 4.3. Database Implementation</td>
                <td class="s7" dir="ltr"><br>K &amp; R<br>K &amp; R &amp; M<br>K &amp; R &amp; M</td>
                <td></td>
                <td class="s12"></td>
                <td class="s10" dir="ltr">4. Product Deployment</td>
                <td class="s10" dir="ltr">R &amp; S</td>
            </tr>
            <tr style="height: 20px">
                <td class="s13"></td>
                <td class="s11" dir="ltr">5. Security <br> 5.1. Web Traffic Encryption <br> 5.2. User Credentials
                    Encryption<br> 5.3. Implementation of JWS Tokens<br> 5.4. Implementation of Google OAuth<br> 5.5.
                    Endpoint authorization and authentication<br> 5.6. Database data encryption<br> 5.7. Data Integrity
                    Protection<br> 5.8. Permision Restriction in Database<br> 5.9. Database Backup
                    Implementation<br><br><br><br><br><br></td>
                <td class="s7" dir="ltr"><br>A &amp; M<br>A &amp; M<br><br>A &amp; M<br><br>A &amp; M<br><br>A &amp;
                    M<br><br>A &amp; M<br><br>A &amp; M<br>A &amp; M<br><br>K &amp; A &amp; M<br><br><br><br><br><br>
                </td>
                <td></td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
        </tbody>
    </table>

## 2.2. Requerimientos Funcionales
1. Versión 1:
<table>
    <thead>
        <tr>
            <th class="s0" dir="ltr" colspan="7">REQUERIMIENTOS FUNCIONALES</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="s1" dir="ltr" colspan="7">Catálogo de Autos</td>
        </tr>
        <tr style="height: 20px">
            <td class="s5" dir="ltr">ID Req Funcional</td>
            <td class="s5" dir="ltr">ID Historia de Usuario Asociada</td>
            <td class="s5" dir="ltr">Concepto</td>
            <td class="s5" dir="ltr">Descripción</td>
            <td class="s5" dir="ltr">Criterios de validación</td>
            <td class="s5" dir="ltr">Nivel</td>
            <td class="s5" dir="ltr">Prioridad</td>
        </tr>
        <tr style="height: 20px">
            <td class="s5" dir="ltr" colspan="7">1.1 Creación del Catálogo</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[001]</td>
            <td class="s6" dir="ltr">US[001]</td>
            <td class="s6" dir="ltr">Registrar un auto</td>
            <td class="s6" dir="ltr">La plataforma le permite a un administrador con permisos correctos registrar un
                auto y sus características.</td>
            <td class="s6" dir="ltr">1. La aplicación me brinda la opción de registrar un nuevo automóvil
                directamente <br>2. La aplicación guarda la nueva información que estoy ingresando en el catálogo
            </td>
            <td class="s6" dir="ltr">1.1.1</td>
            <td class="s6" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[002]</td>
            <td class="s7" dir="ltr"></td>
            <td class="s6" dir="ltr">Asignar Metadatos</td>
            <td class="s6" dir="ltr">Guardar tiempo, fecha y usuario que lo subió.</td>
            <td class="s8"></td>
            <td class="s6" dir="ltr">1.1.2</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s5" dir="ltr" colspan="7">1.2 Modificación del Catálogo</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[003]</td>
            <td class="s6" dir="ltr">US[002]</td>
            <td class="s6" dir="ltr">Eliminar auto</td>
            <td class="s6" dir="ltr">La plataforma le permite a un usuario con permisos correctos eliminar un auto
                del catálogo.</td>
            <td class="s6" dir="ltr">1. La aplicación brinda una vista en la cuenta de administrador donde puede
                visualizar los autos de su catalogo y eliminarlo.<br>2. La aplicación debe de actualizar la base de
                datos correspondiente a la eliminación.<br>3. La aplicación debe de mostrar el catalogo actualizado.
            </td>
            <td class="s6" dir="ltr">1.2.1</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[004]</td>
            <td class="s6" dir="ltr">US[003]</td>
            <td class="s6" dir="ltr">Modificar auto</td>
            <td class="s6" dir="ltr">La plataforma le permite al usuario con permisos correctos modificar
                información de un auto existente.</td>
            <td class="s6" dir="ltr">1. La aplicación brinda una vista en la cuenta de administrador donde puede
                visualizar los autos de su catalogo y modificar los datos que lo describen. <br>2. La aplicación
                debe de actualizar la base de datos correspondiente a la eliminación. <br>3. La aplicación debe de
                mostrar el catalogo actualizado.</td>
            <td class="s6" dir="ltr">1.2.2</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s5" dir="ltr" colspan="7">1.3 Recuperación de Catálogo</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[005]</td>
            <td class="s6" dir="ltr">US[004]</td>
            <td class="s6" dir="ltr">Buscar Auto</td>
            <td class="s6" dir="ltr">La plataforma le permite al usuario ver el catalogo de autos, y navegar en el
                para elegir uno en particular.</td>
            <td class="s6" dir="ltr">1. La aplicación debe de contener una vista en la cuenta de gerente que
                contenga una barra de filtros que permita encontrar un carro en particular al seleccionar una
                combinación de los mismos.<br>2. La aplicación debe de acceder correcta y eficientemente a la base
                de datos para realizar la búsqueda, siendo exclusivamente los resultados del catalogo.</td>
            <td class="s6" dir="ltr">1.3.1</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[006]</td>
            <td class="s6" dir="ltr">US[004]</td>
            <td class="s6" dir="ltr">Filtrar catálogo (Wizard)</td>
            <td class="s6" dir="ltr">La plataforma le permite al usuario filtrar el catálogo de acuerdo a
                características seleccionadas</td>
            <td class="s6" dir="ltr">1. La aplicación debe de contener una vista en la cuenta de gerente que
                contenga un sistema de Wizard permita encontrar un carro en particular mediante la utilización de
                las recomendaciones de tags que sugiera el Wizard.<br>2. El Wizard debe de generar tags
                correctamente y acorde a la información que ingresa el usuario.<br>3. La aplicación debe de acceder
                correcta y eficientemente a la base de datos para realizar la búsqueda, siendo exclusivamente los
                resultados del catalogo.</td>
            <td class="s6" dir="ltr">1.3.2</td>
            <td class="s9" dir="ltr">S</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[007]</td>
            <td class="s6" dir="ltr">US[004]</td>
            <td class="s6" dir="ltr">Buscar Lenguaje Natural </td>
            <td class="s6" dir="ltr">La plataforma le permite al usuario buscar Autos con lenguaje natural.</td>
            <td class="s6" dir="ltr">1. La aplicacion contiene una barra de busqueda que permite escribir en
                lenguaje natural las especificaciones de un vehiculo.<br>2. La aplicación debe de acceder correcta y
                eficientemente a la base de datos para realizar la búsqueda, siendo exclusivamente los resultados
                del catalogo.</td>
            <td class="s6" dir="ltr">1.3.3</td>
            <td class="s9" dir="ltr">C</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr"></td>
            <td class="s6" dir="ltr">US[005]</td>
            <td class="s6" dir="ltr">Buscar Auto</td>
            <td class="s6" dir="ltr">La plataforma le permite al usuario ver el catalogo de autos, y navegar en el
                para elegir uno en particular.</td>
            <td class="s6" dir="ltr">1. La aplicación debe de contener una vista en la cuenta de cliente que
                contenga una sección de búsqueda que permita encontrar un vehiculo en particular eligiendo y
                combinando filtros.<br>2. La aplicación debe de acceder correcta y eficientemente a la base de datos
                para realizar la búsqueda.</td>
            <td class="s6" dir="ltr">1.3.4</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[008]</td>
            <td class="s6" dir="ltr">US[005]</td>
            <td class="s6" dir="ltr">Filtrar catálogo</td>
            <td class="s6" dir="ltr">La plataforma le permite al usuario filtrar el catálogo de acuerdo a
                características seleccionadas</td>
            <td class="s6" dir="ltr">1. La aplicación debe de contener una vista en de catálogo con un sistema
                Wizard que permita encontrar un carro en particular mediante la utilización de las recomendaciones
                de tags que sugiera el Wizard.<br>2. El Wizard debe de generar tags correctamente y acorde a la
                información que ingresa el usuario.<br>3. La aplicación debe de acceder correcta y eficientemente a
                la base de datos para realizar la búsqueda, siendo exclusivamente los resultados del catalogo.</td>
            <td class="s6" dir="ltr">1.3.5</td>
            <td class="s9" dir="ltr">S</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[009]</td>
            <td class="s6" dir="ltr">US[005]</td>
            <td class="s6" dir="ltr">Buscar Lenguaje Natural </td>
            <td class="s6" dir="ltr">La plataforma le permite al usuario buscar Autos con lenguaje natural.</td>
            <td class="s6" dir="ltr">1. La aplicacion contiene una barra de busqueda que permite escribir en
                lenguaje natural las especificaciones de un vehiculo.</td>
            <td class="s6" dir="ltr">1.3.6</td>
            <td class="s9" dir="ltr">C</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[010]</td>
            <td class="s6" dir="ltr">US[006]</td>
            <td class="s6" dir="ltr">Ingresar a homepage</td>
            <td class="s6" dir="ltr">La plataforma le permite al usuario entrar a la página de inicio sin necesidad
                de registrarse</td>
            <td class="s6" dir="ltr">1. La pagina raiz de la plataforma muestra autos en oferta y permite a los
                usuarios ver los productos y crear una cuenta.</td>
            <td class="s6" dir="ltr">1.3.7</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s1" dir="ltr" colspan="7">Venta de Autos</td>
        </tr>
        <tr style="height: 20px">
            <td class="s5" dir="ltr" colspan="7">2.1 Seleccionar Pago</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[011]</td>
            <td class="s6" dir="ltr">US[006]</td>
            <td class="s6" dir="ltr">Calcular precio final</td>
            <td class="s6" dir="ltr">La plataforma le permite al usuario calcular el precio que pagaría al finalizar
                todo el proceso dependiendo del financiamiento elegido.</td>
            <td class="s6" dir="ltr">1. Activar la vista del auto permite ver el precio final, asi como opciones de
                financiamiento y metodos de pago.</td>
            <td class="s6" dir="ltr">2.1.1</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[012]</td>
            <td class="s6" dir="ltr">US[007]</td>
            <td class="s6" dir="ltr">Seleccionar financiamiento</td>
            <td class="s6" dir="ltr">La plataforma le permite al usuario seleccionar el plan de financiamiento de su
                preferencia</td>
            <td class="s6" dir="ltr">1. A partir del perfil del usuarios y sus documentos, tengo la oportunidad de
                elegir un plan de financiamiento desde la interfaz.</td>
            <td class="s6" dir="ltr">2.1.2</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[013]</td>
            <td class="s6" dir="ltr">US[008]</td>
            <td class="s6" dir="ltr">Seleccionar método de pago</td>
            <td class="s6" dir="ltr">La plataforma le permite al usuario seleccionar un método de pago</td>
            <td class="s6" dir="ltr">1. Desde la interfaz de compra se pueden registrar metodos de pago nuevos o
                elegir uno ya registrado.<br>2. Es posible pagar con tarjetas guardadas o soluciones de pagos
                virtuales (transferencia SPEI/PayPal)</td>
            <td class="s6" dir="ltr">2.1.3</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s5" dir="ltr" colspan="7">2.2 Prueba de Manejo</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[014]</td>
            <td class="s6" dir="ltr">US[009]</td>
            <td class="s6" dir="ltr">Registrar documentos de prueba de manejo</td>
            <td class="s6" dir="ltr">La plataforma le permite al usuario subir documentos legales referentes a la
                prueba de manejo</td>
            <td class="s6" dir="ltr">1. La plataforma provee una interfaz para elegir documentos de la computadora
                del usuario y subirlos al sistema.<br>2. La plataforma notifica documentos han sido validados, y de
                no serlo es posible volver a subirlos</td>
            <td class="s6" dir="ltr">2.2.1</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[015]</td>
            <td class="s6" dir="ltr">US[010]</td>
            <td class="s6" dir="ltr">Solicitar prueba de manejo.</td>
            <td class="s6" dir="ltr">La plataforma le permite al usuario solicitar una prueba de manejo</td>
            <td class="s6" dir="ltr">1. Desde la seccion de vista del auto, es posible solicitar una prueba de
                manejo<br>2. Desde el perfil de usuario es posible ver el estado de la solicitud.</td>
            <td class="s6" dir="ltr">2.2.2</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s5" dir="ltr" colspan="7">2.3 Comprar el Auto</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[016]</td>
            <td class="s6" dir="ltr">US[011]</td>
            <td class="s6" dir="ltr">Validar documentacion</td>
            <td class="s6" dir="ltr">La plataforma le permite al usuario subir sus documentos, y al administrador
                revisar y validarlos.</td>
            <td class="s6" dir="ltr">1. El cliente sube sus documentos a la plataforma<br>2. El vendedor con quien
                el cliente tiene una relacion, desde su vista los revisa para checar si son validos o no<br>3. El
                vendedor despues de revisarlos los valida y le notifica al cliente</td>
            <td class="s6" dir="ltr">2.3.1</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[017]</td>
            <td class="s6" dir="ltr">US[012]</td>
            <td class="s6" dir="ltr">Registrar documentos de compra del auto</td>
            <td class="s6" dir="ltr">La plataforma le permite al usuario subir documentos legales referentes a la
                compra del auto</td>
            <td class="s6" dir="ltr">1. Desde la pagina de compra del auto es posible subir los documentos
                necesarios para autorizar el canjeo.</td>
            <td class="s6" dir="ltr">2.3.2</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[018]</td>
            <td class="s7" dir="ltr"></td>
            <td class="s6" dir="ltr">Registrar datos de compra</td>
            <td class="s6" dir="ltr">Guardar datos acerca de la compra (vendedor, estatus, etc)</td>
            <td class="s8"></td>
            <td class="s6" dir="ltr">2.3.3</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[019]</td>
            <td class="s6" dir="ltr">US[013]</td>
            <td class="s6" dir="ltr">Comprar auto</td>
            <td class="s6" dir="ltr">La plataforma le permite al usuario realizar el pago en línea</td>
            <td class="s6" dir="ltr">1. Despues de ser validados los documentos se puede realizar la compra del
                auto.</td>
            <td class="s6" dir="ltr">2.3.4</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[020]</td>
            <td class="s6" dir="ltr">US[014]</td>
            <td class="s6" dir="ltr">Seguimiento de la compra</td>
            <td class="s6" dir="ltr">La plataforma le permite al usuario dar seguimiento al estatus de su compra
            </td>
            <td class="s6" dir="ltr">1. Desde el perfil de usuario es posible ver el estado de las solicitudes y
                compras.</td>
            <td class="s6" dir="ltr">2.3.5</td>
            <td class="s9" dir="ltr">S</td>
        </tr>
        <tr style="height: 20px">
            <td class="s5" dir="ltr" colspan="7">2.4 Revisión de documentación por el Vendedor</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[021]</td>
            <td class="s6" dir="ltr">US[015]</td>
            <td class="s6" dir="ltr">Validar solicitud de compra</td>
            <td class="s6" dir="ltr">La plataforma le permite al vendedor validar la solicitud de un cliente.</td>
            <td class="s6" dir="ltr">1. Despues de ser validados los documentos del cliente se puede validar la
                solicitud de compra.</td>
            <td class="s6" dir="ltr">2.4.1</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[022]</td>
            <td class="s6" dir="ltr">US[016]</td>
            <td class="s6" dir="ltr">Validar documentación</td>
            <td class="s6" dir="ltr">La plataforma le da opción al vendedor de validar los documentos del cliente
            </td>
            <td class="s6" dir="ltr">1. Se requiere validar los documentos del cliente previo a validar sus
                solicitudes de compra.</td>
            <td class="s6" dir="ltr">2.4.2</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s5" dir="ltr" colspan="7">2.5 Modificar precios finales y planes de financiamiento</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[023]</td>
            <td class="s6" dir="ltr">US[017]</td>
            <td class="s6" dir="ltr">Modificación de los precios y planes de financiamiento</td>
            <td class="s6" dir="ltr">La plataforma le permite al vendedor modificar los precios finales y los planes
                de financiamiento.</td>
            <td class="s6" dir="ltr">1. Los precios de los autos son subidos junto con el catálogo de la
                agencia<br>2. Si mi agencia me pide modificar los precios a través de mi vista lo puedo hacer<br>3.
                Si con el cliente llego a un acuerdo diferente del precio que esta marcado en la plataforma lo puedo
                modificar</td>
            <td class="s6" dir="ltr">2.5.1</td>
            <td class="s9" dir="ltr">S</td>
        </tr>
        <tr style="height: 20px">
            <td class="s1" dir="ltr" colspan="7">Cuentas</td>
        </tr>
        <tr style="height: 20px">
            <td class="s5" dir="ltr" colspan="7">3.1 Creación de cuentas</td>
        </tr>
        <tr style="height: 20px">
            <td class="s10" dir="ltr">REQ_FUN[024]</td>
            <td class="s8"></td>
            <td class="s6" dir="ltr">Crear cuenta de “super-administrador”</td>
            <td class="s6" dir="ltr">El super administrador cuenta con todos los privilegios dentro de la aplicación
                web y además puede dar de alta a las agencias y/o grupos automotrices</td>
            <td class="s7" dir="ltr"></td>
            <td class="s6" dir="ltr">3.1.1</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s10" dir="ltr">REQ_FUN[025]</td>
            <td class="s6" dir="ltr">US[018]</td>
            <td class="s6" dir="ltr">Crear cuenta de agencia (nivel alto)</td>
            <td class="s6" dir="ltr">El “super-administrador” puede dar de alta cuentas de las agencias o grupos
                automotrices que hayan sido autorizados</td>
            <td class="s6" dir="ltr">1. La aplicación brinda una sección con el formulario adecuado para crear una
                cuenta correspondiente a una agencia. <br>2. La aplicación almacena correctamente los datos de la
                cuenta de agencia. </td>
            <td class="s6" dir="ltr">3.1.2</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[026]</td>
            <td class="s6" dir="ltr">US[019]</td>
            <td class="s6" dir="ltr">Registrar documentos de validación de agencia</td>
            <td class="s6" dir="ltr">La plataforma le permite a la agencia registrar sus documentos legales de
                registro</td>
            <td class="s6" dir="ltr">1. Como agencia quiero hacer mi solicitud dentro de la plataforma<br>2. Lleno
                los datos necesarios y subo los documentos correspondientes<br>3. Mis documentos son validados del
                otro lado por un agente.</td>
            <td class="s6" dir="ltr">3.1.3</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[027]</td>
            <td class="s6" dir="ltr">US[020]</td>
            <td class="s6" dir="ltr">Validar documentos de validación de agencia</td>
            <td class="s6" dir="ltr">La plataforma le permite al super administrador observar y validar documentos
                de registro, además de proporcionarles información si se rechaza</td>
            <td class="s6" dir="ltr">1. La agencia sube sus documentos para solicitar estar dentro de la
                plataforma<br>2. El super-administrador los revisa y puede validarlos o rechazarlos</td>
            <td class="s6" dir="ltr">3.1.4</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[028]</td>
            <td class="s6" dir="ltr">US[021]</td>
            <td class="s6" dir="ltr">Crear cuenta de gerente (nivel medio)</td>
            <td class="s6" dir="ltr">Las agencias puede dar de alta a las cuentas de los gerentes de su agencia</td>
            <td class="s6" dir="ltr">1. La aplicación brinda una sección con el formulario adecuado para crear una
                cuenta correspondiente a un gerente. <br>2. La aplicación almacena correctamente los datos de la
                cuenta de agencia. </td>
            <td class="s6" dir="ltr">3.1.5</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[029]</td>
            <td class="s6" dir="ltr">US[022]</td>
            <td class="s6" dir="ltr">Crear cuenta de ventas (nivel bajo)</td>
            <td class="s6" dir="ltr">Los gerentes puede dar de alta a las cuentas de los vendedores de su agencia
            </td>
            <td class="s6" dir="ltr">1. La aplicación brinda una sección con el formulario adecuado para crear una
                cuenta correspondiente a un vendedor. <br>2. La aplicación almacena correctamente los datos de la
                cuenta de vendedor.</td>
            <td class="s6" dir="ltr">3.1.6</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[030]</td>
            <td class="s6" dir="ltr">US[023]</td>
            <td class="s6" dir="ltr">Crear cuenta de cliente</td>
            <td class="s6" dir="ltr">Los usuarios pueden registrarse y crear una cuenta en la aplicación web</td>
            <td class="s6" dir="ltr">1. La aplicación brinda una sección con el formulario adecuado para crear una
                cuenta correspondiente a un cliente. <br>2. La aplicación almacena correctamente los datos de la
                cuenta de cliente.</td>
            <td class="s6" dir="ltr">3.1.7</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[031]</td>
            <td class="s6" dir="ltr">US[024]</td>
            <td class="s6" dir="ltr">Modificar datos personales</td>
            <td class="s6" dir="ltr">Los clientes pueden cambiar sus datos personales como su nombre, correo,
                dirección, entre otros.</td>
            <td class="s6" dir="ltr">1. La aplicación brinda una sección de &quot;modificación de datos&quot; en la
                que el usuario puede editar sus datos personales de su perfil.<br>2. La aplicación debe de
                actualizar correctamente los datos modificados por el usuario.</td>
            <td class="s6" dir="ltr">3.2.1</td>
            <td class="s9" dir="ltr">S</td>
        </tr>
        <tr style="height: 20px">
            <td class="s5" dir="ltr" colspan="7">3.3 Eliminación de cuentas</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[032]</td>
            <td class="s6" dir="ltr">US[025]</td>
            <td class="s6" dir="ltr">Eliminar cuenta de agencia (nivel alto)</td>
            <td class="s6" dir="ltr">El súper administrador puede eliminar las cuentas de las agencias o grupos
                automotrices</td>
            <td class="s6" dir="ltr">1. La aplicación brinda una vista en la cuenta de administrador donde puede
                visualizar las cuentas a su cargo y eliminarlas.<br>2. La aplicación debe de actualizar la base de
                datos correspondiente a la eliminación.</td>
            <td class="s6" dir="ltr">3.3.1</td>
            <td class="s9" dir="ltr">S</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[033]</td>
            <td class="s6" dir="ltr">US[026]</td>
            <td class="s6" dir="ltr">Eliminar cuenta de gerente (nivel medio)</td>
            <td class="s6" dir="ltr">Las agencias pueden eliminar las cuentas de los gerentes de su agencia</td>
            <td class="s6" dir="ltr">1. La aplicación brinda una vista en la cuenta de agencia donde puede
                visualizar las cuentas de gerente a su cargo y eliminarlas.<br>2. La aplicación debe de actualizar
                la base de datos correspondiente a la eliminación.</td>
            <td class="s6" dir="ltr">3.3.2</td>
            <td class="s9" dir="ltr">S</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[034]</td>
            <td class="s6" dir="ltr">US[027]</td>
            <td class="s6" dir="ltr">Eliminar cuenta ventas (nivel bajo)</td>
            <td class="s6" dir="ltr">Los gerentes pueden eliminar las cuentas de los vendedores de su agencia</td>
            <td class="s6" dir="ltr">1. La aplicación brinda una vista en la cuenta de gerente donde puede
                visualizar las cuentas de vendedores a su cargo y eliminarlas.<br>2. La aplicación debe de
                actualizar la base de datos correspondiente a la eliminación, y eliminar las relaciones que existan
                del vendedor con clientes, buscando crear una nueva relacion cliente&#39;vendedor de la misma
                agencia..</td>
            <td class="s6" dir="ltr">3.3.3</td>
            <td class="s9" dir="ltr">S</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[035]</td>
            <td class="s6" dir="ltr">US[028]</td>
            <td class="s6" dir="ltr">Eliminar cuenta de cliente</td>
            <td class="s6" dir="ltr">El cliente puede eliminar su propia cuenta</td>
            <td class="s6" dir="ltr">1. La aplicación brinda una vista en la donde el cliente tiene la opción de
                eliminar su propia cuenta.<br>2. La aplicación debe de verificar con un &quot;pop-up&quot; que el
                usuario realmente desea eliminar su cuenta.<br>3. La aplicación debe de actualizar la base de datos
                correspondiente a la eliminación y sus respectivas relaciones con los vendedores.</td>
            <td class="s6" dir="ltr">3.3.4</td>
            <td class="s9" dir="ltr">S</td>
        </tr>
        <tr style="height: 20px">
            <td class="s1" dir="ltr" colspan="7"></td>
        </tr>
        <tr style="height: 20px">
            <td class="s5" dir="ltr" colspan="7">4.2 Diálogo con Agente por Chat</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[036]</td>
            <td class="s6" dir="ltr">US[029]</td>
            <td class="s6" dir="ltr">Iniciar conversación con un agente</td>
            <td class="s6" dir="ltr">El usuario solicita el inicio de una conversación con un agente.</td>
            <td class="s6" dir="ltr">1. Desde la plataforma es posible instanciar una solicitud de chat con un
                agente.<br>2. Si hay agentes disponibles, es posible tener un dialogo en tiempo real<br>3. Si no
                existe, se crea una relacion entre el cliente y el vendedor para permanecer en contacto en el
                futuro.</td>
            <td class="s6" dir="ltr">4.2.1</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[037]</td>
            <td class="s6" dir="ltr">US[030]</td>
            <td class="s6" dir="ltr">Negociación de Precio</td>
            <td class="s6" dir="ltr">Al usuario se le permite negociar el precio final con el vendedor por medio del
                chat.</td>
            <td class="s6" dir="ltr">1. El cliente solicita hablar con un agente despues de seleccionar el auto de
                su interés<br>2. El cliente puede comenzar una convesación y negociar un precio diferente al marcado
                en la plataforma, de no tener una relacion con el vendedor, se genera una para futuras
                interacciones.</td>
            <td class="s6" dir="ltr">4.2.2</td>
            <td class="s9" dir="ltr">C</td>
        </tr>
        <tr style="height: 20px">
            <td class="s1" dir="ltr" colspan="7">Admins</td>
        </tr>
        <tr style="height: 20px">
            <td class="s5" dir="ltr" colspan="7">5.1 Estadisticas y metricas</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[038]</td>
            <td class="s6" dir="ltr">US[031]</td>
            <td class="s6" dir="ltr">Recuperar estadisticas de usuarios</td>
            <td class="s6" dir="ltr">La plataforma le permite al usuario observar estadísticas correspondientes a su
                rol</td>
            <td class="s6" dir="ltr">1. Hay una seccion en la plataforma para administradores, donde es posible ver
                estadisticas de las ventas y consultas en la plataforma.</td>
            <td class="s6" dir="ltr">5.1.1</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s5" dir="ltr" colspan="7">5.2 Búsqueda de Admins</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[039]</td>
            <td class="s6" dir="ltr">US[032]</td>
            <td class="s6" dir="ltr">Buscar usuarios</td>
            <td class="s6" dir="ltr">La plataforma le permite a los admins buscar usuarios a su cargo</td>
            <td class="s9 softmerge" dir="ltr">
                <div class="softmerge-inner" style="width:339px;left:-1px">1. Desde la plataforma, un administrador
                    tiene un endpoint para ver los usuarios a su cargo.</div>
            </td>
            <td class="s6" dir="ltr">5.2.1</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[040]</td>
            <td class="s6" dir="ltr">US[033]</td>
            <td class="s6" dir="ltr">Filtrar usuarios</td>
            <td class="s6" dir="ltr">La plataforma le permite a los admins filtrar usuarios</td>
            <td class="s6" dir="ltr">1. Desde la plataforma, un administrador puede filtrar su búsqueda de usuarios
            </td>
            <td class="s6" dir="ltr">5.2.2</td>
            <td class="s9" dir="ltr">S</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[041]</td>
            <td class="s6" dir="ltr">US[034]</td>
            <td class="s6" dir="ltr">Busqueda con tags</td>
            <td class="s6" dir="ltr">La plataforma le permite a los admins usar tags para encontrar usuarios</td>
            <td class="s6" dir="ltr">1. Desde la plataforma, un administrador puede realizar una busqueda tipo
                wizard con tags</td>
            <td class="s6" dir="ltr">5.2.3</td>
            <td class="s9" dir="ltr">C</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[042]</td>
            <td class="s6" dir="ltr">US[035]</td>
            <td class="s6" dir="ltr">Ver lista de todos los clientes</td>
            <td class="s6" dir="ltr">La plataforma muestra una lista de todos los clientes registrados, la seleccion
                permite ver mas informacion de un cliente particular.</td>
            <td class="s6" dir="ltr">1. La plataforma tiene una seccion apartada para ver los clientes interesados
                en sus productos.</td>
            <td class="s6" dir="ltr">5.2.4</td>
            <td class="s9" dir="ltr">S</td>
        </tr>
        <tr style="height: 20px">
            <td class="s5" dir="ltr" colspan="7">5.3 Diálogo con Cliente por Chat</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[043]</td>
            <td class="s6" dir="ltr">US[036]</td>
            <td class="s6" dir="ltr">Ver fila de Clientes en espera</td>
            <td class="s6" dir="ltr">La plataforma muestra el Queue de clientes en espera, a la que puede
                suscribirse el agente.</td>
            <td class="s6" dir="ltr">1. Un vendedor puede ver el queue de clientes en espera</td>
            <td class="s6" dir="ltr">5.3.1</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[044]</td>
            <td class="s6" dir="ltr">US[037]</td>
            <td class="s6" dir="ltr">Iniciar conversación con Cliente</td>
            <td class="s6" dir="ltr">El sistema asigna el primer Cliente del Queue al Agente y se instancía una
                conversación.</td>
            <td class="s11" dir="ltr">1. Un vendedor puede entrar en el queue de clientes en espera para un chat, y
                se crea una nueva instancia de relacion entre el vendedor y el cliente.</td>
            <td class="s6" dir="ltr">5.3.2</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[045]</td>
            <td class="s7" dir="ltr"></td>
            <td class="s6" dir="ltr">Instanciar nueva relación</td>
            <td class="s6" dir="ltr">La plataforma guarda el identificador de usuario y agente para interacciones
                futuras</td>
            <td class="s7"></td>
            <td class="s6" dir="ltr">5.3.3</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s1" dir="ltr" colspan="7">Seguridad</td>
        </tr>
        <tr style="height: 20px">
            <td class="s5" dir="ltr" colspan="7">6.1 Seguridad de la Interfaz</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[046]</td>
            <td class="s7" dir="ltr"></td>
            <td class="s6" dir="ltr">Sanitizar las entradas</td>
            <td class="s6" dir="ltr">Sanitizar la información ingresada a la plataforma por externos, antes de
                pasarla a otro proceso.</td>
            <td class="s7"></td>
            <td class="s6" dir="ltr">6.1.1</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s5" dir="ltr" colspan="7">6.2 Seguridad de la Base de Datos</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[047]</td>
            <td class="s7" dir="ltr"></td>
            <td class="s6" dir="ltr">Encriptar credenciales de las cuentas</td>
            <td class="s6" dir="ltr">Almacenar las credenciales (usuario y contraseña) de los usuarios de la
                plataforma de forma encriptada.</td>
            <td class="s12"></td>
            <td class="s6" dir="ltr">6.2.1</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[048]</td>
            <td class="s7" dir="ltr"></td>
            <td class="s6" dir="ltr">Encriptar archivos subidos</td>
            <td class="s6" dir="ltr">Almacenar a los archivos subidos a la plataforma de forma encriptada.</td>
            <td class="s7"></td>
            <td class="s6" dir="ltr">6.2.2</td>
            <td class="s9" dir="ltr">M</td>
        </tr>
        <tr style="height: 20px">
            <td class="s5" dir="ltr" colspan="7">6.3 Disposiciones Generales</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_FUN[049]</td>
            <td class="s6" dir="ltr">US[038]</td>
            <td class="s6" dir="ltr">Registrar acciones de los usuarios.</td>
            <td class="s6" dir="ltr">Mantener una bitácora de las acciones de los usuarios en el sistema. (e.j.
                inicio de sesión, cierre de sesión, subida, descarga).</td>
            <td class="s6" dir="ltr">1. La plataforma tiene una seccion para usuarios con permisos de
                super-administrador para ver y modificar acciones de los usuarios.</td>
            <td class="s6" dir="ltr">6.3.1</td>
            <td class="s9" dir="ltr">S</td>
        </tr>
    </tbody>
</table>

## 2.3. Requerimientos No Funcionales
1. Versión 1
<table>
    <thead>
    </thead>
    <tbody>
        <tr style="height: 20px">
            <td class="s13" dir="ltr" colspan="7">REQUERIMIENTOS NO FUNCIONALES</td>
        </tr>
        <tr style="height: 20px">
            <td class="s1" dir="ltr" colspan="7">Catálogo de Autos</td>
        </tr>
        <tr style="height: 20px">
            <td class="s5" dir="ltr">ID Req Funcional</td>
            <td class="s5" dir="ltr">ID Historia de Usuario Asociada</td>
            <td class="s5" dir="ltr">Concepto</td>
            <td class="s5" dir="ltr">Descripción</td>
            <td class="s5" dir="ltr">Criterios de validación</td>
            <td class="s5" dir="ltr">Nivel</td>
            <td class="s5" dir="ltr">Prioridad</td>
        </tr>
        <tr style="height: 20px">
            <td class="s5" dir="ltr" colspan="7">1.1 Recuperación de Catálogo</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_NOFUN[001]</td>
            <td class="s6" dir="ltr">US_NF[001]</td>
            <td class="s6" dir="ltr">Comparar Autos</td>
            <td class="s6" dir="ltr">La plataforma le permite al usuario comparar dos Autos del catálogo</td>
            <td class="s6" dir="ltr">1. Desde la busqueda de autos, es posible hacer una comparacionentre un auto y
                otro, mostrando similitudes y diferencias, asi como caracteristicas en que uno es mejor que otro.
            </td>
            <td class="s6" dir="ltr">1.1.1</td>
            <td class="s9" dir="ltr">C</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_NOFUN[002]</td>
            <td class="s6" dir="ltr">US_NF[002]</td>
            <td class="s6" dir="ltr">Lista de deseos (wishlist)</td>
            <td class="s6" dir="ltr">La plataforma le permite al usuario seleccionar Autos que le hayan gustado y
                guardarlos (bookmark)</td>
            <td class="s6" dir="ltr">1. El usuario puede apartar un auto en su lista de deseos para despues
                consultarla en su perfil. <br>2. Los autos apartados tambien generan sugerencias de productos
                similares.</td>
            <td class="s6" dir="ltr">1.1.2</td>
            <td class="s9" dir="ltr">C</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_NOFUN[003]</td>
            <td class="s6" dir="ltr">US_NF[003]</td>
            <td class="s6" dir="ltr">Recomendar autos</td>
            <td class="s6" dir="ltr">En base al wishlist y la actividad del usuario, usando machine learning, la
                plataforma recomendará autos al usuario</td>
            <td class="s6" dir="ltr">1. La plataforma muestra autos similares a los que el usuario ha consultado en
                el buscador</td>
            <td class="s6" dir="ltr">1.1.3</td>
            <td class="s9" dir="ltr">C</td>
        </tr>
        <tr style="height: 20px">
            <td class="s1" dir="ltr" colspan="7">Venta</td>
        </tr>
        <tr style="height: 20px">
            <td class="s5" dir="ltr" colspan="7">2.1 Cotización</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_NOFUN[004]</td>
            <td class="s6" dir="ltr">US_NF[004]</td>
            <td class="s6" dir="ltr">Comprar auto con precio final</td>
            <td class="s6" dir="ltr">La plataforma permite al cliente hacer una compra con el precio mostrado en la
                vista del producto (one-click-transaction)</td>
            <td class="s11" dir="ltr">1. La plataforma hace un cálculo del precio final de un auto con las
                especificaciones de la agencia</td>
            <td class="s6" dir="ltr">2.1.1</td>
            <td class="s9" dir="ltr">C</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_NOFUN[005]</td>
            <td class="s7" dir="ltr"></td>
            <td class="s6" dir="ltr">Proceso de venta &quot;transparente&quot;</td>
            <td class="s6" dir="ltr">El cliente al solicitar o realizar una cotización del auto de su interés se le
                mostrará el precio final del auto</td>
            <td class="s7"></td>
            <td class="s6" dir="ltr">2.1.2</td>
            <td class="s9" dir="ltr">S</td>
        </tr>
        <tr style="height: 20px">
            <td class="s1" dir="ltr" colspan="7">Recepción de documentos</td>
        </tr>
        <tr style="height: 20px">
            <td class="s5" dir="ltr" colspan="7">3.1 Procesamientos de documentos</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_NOFUN[006]</td>
            <td class="s7" dir="ltr"></td>
            <td class="s6" dir="ltr">Procesamientos de documentos con OCR</td>
            <td class="s6" dir="ltr">La plataforma al recibir los documentos es capaz de identificar los caracteres
                dentro del archivo y procesarlos como texto</td>
            <td class="s7"></td>
            <td class="s6" dir="ltr">3.1.1</td>
            <td class="s9" dir="ltr">C</td>
        </tr>
        <tr style="height: 20px">
            <td class="s1" dir="ltr" colspan="7">Diseño de aplicación web</td>
        </tr>
        <tr style="height: 20px">
            <td class="s5" dir="ltr" colspan="7">4.1 Interface</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_NOFUN[007]</td>
            <td class="s6" dir="ltr">US_NF[005]</td>
            <td class="s6" dir="ltr">Screen-size adaptable para tablet y celular</td>
            <td class="s6" dir="ltr">La aplicación web se puede adaptar a distintos dispositivos con la finalidad de
                tener la mejor experiencia visual</td>
            <td class="s11" dir="ltr">1. La plataforma es responsiva y se puede adaptar a diferentes tamaños</td>
            <td class="s6" dir="ltr">4.1.1</td>
            <td class="s9" dir="ltr">S</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_NOFUN[008]</td>
            <td class="s7" dir="ltr"></td>
            <td class="s6" dir="ltr">Interfaz y experiencia de la aplicación web</td>
            <td class="s6" dir="ltr">La aplicación web es sencilla de usar y está pensada en torno al usuario (UX)
            </td>
            <td class="s12"></td>
            <td class="s6" dir="ltr">4.1.2</td>
            <td class="s9" dir="ltr">S</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_NOFUN[009]</td>
            <td class="s7" dir="ltr"></td>
            <td class="s6" dir="ltr">Diseño visual de la aplicación web (UI)</td>
            <td class="s6" dir="ltr">La aplicación web está diseñada para que sea visualmente lo más sencilla pero
                con un diseño gráfico pensado específicamente para este servicio</td>
            <td class="s12"></td>
            <td class="s6" dir="ltr">4.1.3</td>
            <td class="s9" dir="ltr">S</td>
        </tr>
        <tr style="height: 20px">
            <td class="s6" dir="ltr">REQ_NOFUN[010]</td>
            <td class="s7" dir="ltr"></td>
            <td class="s6" dir="ltr">Proceso de venta &quot;transparente&quot;</td>
            <td class="s6" dir="ltr">El cliente al solicitar o realizar una cotización del auto de su interés se le
                mostrará el precio final del auto</td>
            <td class="s14"></td>
            <td class="s6" dir="ltr">4.1.4</td>
            <td class="s9" dir="ltr">S</td>
        </tr>
    <tbody>
</table>

## 2.4. Restricciones

# 3. Arquitectura
## 3.1. Diagrama de Arquitectura
1. Versión 1: https://github.com/MateoHerrera0/HUMANIT/blob/main/Documentaci%C3%B3n/Architecture%20Diagram.drawio.png
<div align="center">
    <img src="Architecture Diagram.drawio.png" width="500" title="hover text">
</div> 
  
Componentes:

1. Route53: Servicio de DNS proporcionado por AWS.
2. AWS Shield: Servicio de protección ante ataques DDoS proporcionado por AWS.
3. WAF: Firewall de aplicaciones web de AWS. Contiene preconfiguraciones de reglas que protegen ante los top 10 riesgos de seguridad según OWASP.
4. CloudFront. Servicio de CDN (cloud distribution network) proporcionado por AWS. Hace uso de edge locations (caches) para generar conexiones más rápidas. CloudFront también encripta la comunicación entre el servidor y cliente.
5. Elastic Load Balancer: Servicio de AWS que automáticamente distribuye el tráfico entrante a diferentes destinos (EC2). Si una instancia de EC2 tiene mucho tráfico, este servicio automáticamente redirige a usuarios entrantes a otras instancias para generar un mejor desempeño de la aplicación.
6. Auto Scaling Group: Servicio de AWS que permite la creación automática de nuevas instancias de EC2 si se requiere en relación al tráfico entrante, y las destruye cuando no se necesiten. Esto ayuda a la escalabilidad del sistema.
7. Web Server (EC2): Máquina virtual EC2  encargada del despliegue del front-end.
8. App Server (EC2): Máquina virtual EC2 encargada del despliegue del back-end.
9. Elasticache: Caché de base de datos proporcionada por AWS. Queries de información frecuentemente utilizadas suceden dentro del caché, ayudando al rendimiento de la aplicación.
10. mySQL: Base de datos relacional.
11. MongoDB: Base de datos no relacional.
12. Rekognition (Opcional): Servicio de computer vision de AWS capaz de detectar contenido inapropiado, texto y biométricos en imágenes y videos.
13. Textract (Opcional):  Servicio de OCR proporcionado por AWS  capaz de extraer texto de documentos.
14. S3 Bucket for media: Bucket para almacenamiento de documentos e imágenes de la aplicación web
15. S3 Bucket for ECD & DB backup: Bucket para almacenamiento de copias de seguridad de instancias EC2 y bases de datos.
16. CloudWatch: Servicio de monitor cloud de AWS.
17. IAM: Servicios de autorización y autenticación configurables dentro de AWS.
  
  
## 3.2. Stack Tecnológico
1. Software Development IDE

_Visual Studio Code:_
* Gratuito - Open Source.
* Los programadores cuentan con conocimiento y experiencia previa.
* Compatible con diversos OS.
* Gran compatibilidad con extensiones/plugins de herramientas externas.
* Intuitivo de utilizar.

2. Database

_MySQL Community Edition (Almacenamiento de Cuentas):_
* Gratuito - GPL Licence.
* Los programadores cuentan con conocimiento y experiencia previa.
* Compatible con diversos OS - compatible con Windows. 
* Cuenta con capas de seguridad.
* Estructura relacional -  bueno para almacenar relaciones como aquellas en los diferentes tipos de cuentas definidas para la plataforma.
* Cuenta con una buena comunidad, documentación y material de consulta para su utilización.

_MongoDB (Almacenamiento de catálogo e información de la compra):_
* Gratuito.
* Los programadores cuentan con conocimiento y experiencia previa.
* Compatible con diversos OS - compatible con Windows. 
* Fácil instalación e implementación. 
* Altamente flexible y escalable.
* Tolera grandes volúmenes de datos.
* Estructura no relacional - bueno para manejar muchas read-write operations como lo son búsquedas, filtrado e información referente a la compra del auto.
* Cuenta con una buena comunidad, documentación y material de consulta para su utilización.

3. Dev. Environments

_NodeJS (Application Layer):_
* Gratuito - Open Source.
* Los programadores cuentan con conocimiento y experiencia previa.
* Compatibilidad cross-platform - gran compatibilidad con React.
* Facilita el desarrollo del backend en JavaScript.
* Particularmente rápido y escalable al estar construido sobre Chrome V8 Engine.
* Cuenta con una buena comunidad, documentación y material de consulta para su utilización.

4. Frameworks

_Express:_
* Gratuito - Open Source.
* Framework derivado de NodeJS y por ende compatible.
* Los programadores cuentan con conocimiento y experiencia previa.
* Provee un conjunto de herramientas que facilitan la creación del backend/API con NodeJS.
* Cuenta con una buena comunidad, documentación y material de consulta para su utilización.

5. Front-end Development Libraries

_React (JavaScript):_
* Gratuito - Open Source
* Los programadores cuentan con conocimiento y experiencia previa.
* Permite programación por componentes haciendo fácil reutilización y mantenimiento de código para la implementación de la funcionalidad y renderizado del front-end.
* Utiliza virtual DOM lo cual aumenta su rendimiento al permitir que cierta información se maneje y esté disponible “client-side”.
* Cuenta con una buena comunidad, documentación y material de consulta para su utilización.

6. Cascading Style Libraries

_Bootstrap:_
* Gratuito.
* Los programadores cuentan con conocimiento y experiencia previa.
* Opera en base a un “Grid System” con elementos pre-desarrollados que ahorran tiempo y esfuerzo al momento de realizar el estilo.
* A comparación de otras opciones que dan más libertad, con Bootstrap es sumamente rápido el desarrollo del UI.
* Cuenta con una buena comunidad, documentación y material de consulta para su utilización.

7. Cloud Service

_AWS - Academy Trial:_
* Se cuenta con 100 USD de crédito por cada integrante (2,000 USD).
* Los programadores cuentan con conocimiento y experiencia previa.
* Altamente escalable y confiable.
* Ofrece un amplio rango de herramientas y servicios.
* Proporciona un alto nivel de seguridad necesaria para la documentación legal y otra información confidencial manejada en la compra de un auto.

8. Payment Gateway Integration

_Stripe:_
* Comisión de 2.9% + 30 centavos por cada transacción.
* API fácil y rápida de utilizar/integrar con otra plataforma.
* Soporta una amplia variedad de monedas y métodos de pago.
* Proporciona un sistema seguro de pago.
* Cuenta con servicio al cliente 24/7 ya sea vía teléfono, email o live chat.
* Cuenta con una buena comunidad, documentación y material de consulta para su utilización.

9. Source Control

_GitHub:_
* Gratuito.
* Todos los programadores han utilizado y conocen extensamente la herramienta.
* Permite repositorios ilimitados - lo cual da versatilidad a la organización que se tome para la realización del proyecto.
* Permite administrar de forma sencilla y organizada controlar la colaboración, actualizaciones y cambios que se realicen al proyecto por parte de todos los miembros del equipo.
* Cuenta con una buena comunidad, documentación y material de consulta para su utilización.

10. Browsers
* Firefox
* Chrome
* Safari
* Edge

11. Operating Systems
* Windows 

  
### Diagrama del Tech Stack
A continuación se encuentra la visualización gráfica del Tech Stack de la solución. <br>
Link al diagrama: https://www.figma.com/file/yLADWuGigqfuYnZxik1LG7/Tech-Stack-Diagram-(Copy)?node-id=0%3A1&t=aLeCQBq4z7graTVD-1
<p align="center">
  <img src="TechStackChart.png" width="600" title="hover text">
</p>