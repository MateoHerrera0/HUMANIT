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
## 2.3. Requerimientos No Funcionales
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




