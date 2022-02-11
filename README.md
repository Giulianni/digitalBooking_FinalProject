# digitalBooking_FinalProject
Final team project on the Certified Tech Developer career by Digital House. 

# ![]()![logo_1](https://s3.amazonaws.com/digitalbooking.equipo3c3/DocTecnica/logo_1.png)   [Digital Booking](http://digitalbooking.one), _sentite como en tu hogar_

*Digital Booking es una empresa de alquiler de casas, departamentos, habitaciones privadas y alojamientos en general, para toda persona que desee viajar y sentirse como en su hogar*. En busca de un despegue comercial de impacto, la empresa se propuso lanzar su página web de reservas online disponible 24/7.

El objetivo del equipo de desarrollo es ofrecer una página amigable, accesible y tolerante a todo tipo de usuarix. ¿Qué significa esto? Que la página se pueda usar tranquilx, apuradx, sin ganas de leer tanto, con una mascota pasando por el teclado o como sea. *La usabilidad y la tolerancia a fallos hacen del buscador de alojamientos y el motor de reservas de Digital Booking, la mejor opción para viajar y sentirte siempre como en tu hogar*. :palm_tree: :sunrise: :relaxed:

---

## Metodología de trabajo

### Metodología Scrum
Respetando todas los eventos, tiempos y roles. 
En esta practica contamos con la presencia de TLs, PO y Scrum Master mientras que en el equipo rotamos los roles de (Front End, Back End, BBDD, QA e Analista de Infraestructura). 
 
#### Asignación de roles
Al inicio rotamos entre todas las áreas cada integrante, y después cada uno se dedicó más al área que más le motivaba. 

## Duración del proyecto 

- 8 Semanas. 
- 4 Sprints. 

## Herramientas de desarrollo

### Gestión del Proyecto

Para el **desarrollo** de este proyecto, el equipo de desarrollo basó su interacción en tres **herramientas** principales: 

* GitLab: herramienta para el desarrollo de software colaborativo basada en Git, que funge de gestor 
  de repositorios y servicio de control de versiones.
* Discord: servicio de mensajería instantánea que funciona por servidores. El equipo cuenta con un 
  servidor propio en el que se crearon canales de texto para:
  * Áreas del proyecto:
    * Infraestructura
    * Bases de datos
    * Back end
    * Front end
    * Testing
  * Recursos útiles para el proyecto: información sobre páginas del mismo nicho 
    y recursos relativos al stack tecnológico utilizado.
  * Eventos de scrum:
    * Dailies: resumen de las actividades diarias de cada integrante.
    * Retros: recopilación de las acciones acordadas en cada Retrospectiva.
    * Product-Owner: tareas del sprint y aclaraciones de la PO. 
    * ppt: desarrollo y puesta en común de las presentaciones para cada sprint.
* Servicios de videollamadas como Zoom y Meet: reuniones virtuales de equipo para co-working, 
  resolución de conflictos y eventos de Scrum.

### Desarrollo del proyecto:
* IDEs: 
  * Visual Studio Code
  * IntelliJ Idea
  * MySQL Workbench
* Sistema de control de versiones:
  * Git
* Simulación / Virtualización: 
  * Hibernate-h2 (Bases de datos en Backend)

## Stack tecnológico del proyecto
* Front end: 
  * HTML + CSS
  * Javascript
  * React
    * Dependencias: 
      * React Router
      * Fortawesome
      * React Google Maps API
      * Axios
      * Rc-Rate
      * React burguer menu
      * React Datepicker
      * React Image Gallery
      * Styled components
  * Node + NPM
* Back end:
  * Java
  * Spring
  * Hibernate
* Base de datos: 
  * MySQL
  * MySQL Workbench
  * RDS
* Infraestructura:
  * Diagrams.net
  * AWS (Redes, EC2, RDS, S3)
  * Ubuntu 
  * Apache
  * MobaXTerm
  * Java SDK
  * Npm
  * Gitlab
  * Git
* Testing
  * Postmant
  * JEST
  * JUnit + Mockito


### DOCUMENTACIÓN TÉCNICA -------------------------------------------------------


## Adaptaciones de diseño por sprint
* [SPRINT 1](https://www.figma.com/file/ZDCQvG8wHRGPN3kgvkNivl/SPRINT-1---CTD-GRUPO-3?node-id=488%3A13568)

* [SPRINT 2](https://www.figma.com/file/AZp4KUpzUweuuICV0IRout/SPRINT-2---CTD---grupo-3?node-id=1063%3A10094)

* [SPRINT 3](https://www.figma.com/file/CjiGUTGd20ihpneX0ldOtM/SPRINT-3--CTD--GRUPO-3?node-id=1063%3A10094)

* [SPRINT 4](https://www.figma.com/file/FbozqgyyqaLnv0T51dE1sB/SPRINT-4---CTD-GRUPO-3?node-id=2104%3A17987)


## Recomendaciones para sumarse al ambiente de desarrollo

* Trabajar en una branch independiente hasta hacer funcional la nueva feature. Antes de hacer un merge, ejecutar un fetch de la rama a la que se va mergear. Incorporar los cambios si no se hicieron automáticamente, ejecutar el proyecto y realizar pruebas de integración. Una vez que la rama está funcional y los bugs que no se pudieron reportar se solucionaron, mergear a la rama troncal
* Determinar las "definition of done" en la planning.
* Si pasa un día sin poder resolver un problema.

## Base de datos

![Base_de_datos](https://s3.amazonaws.com/digitalbooking.equipo3c3/DocTecnica/Base_de_datos.png)

## Componentes y diagramas de la aplicación

![Flowchart_Template__2_](https://s3.amazonaws.com/digitalbooking.equipo3c3/DocTecnica/Flowchart_Template__2_.jpg)

## Backend

### Requerimientos

1) Java 11
2) Maven
3) MySQL
4) Workbench

### Instalación

Para la instalación de Java, Maven, MySQL y Workbench se recomienda la siguiente documentación:

- [Instalación Java 11](https://www.oracle.com/java/technologies/downloads/#java11)
- [Instalación Maven](https://maven.apache.org/download.cgi).
- [Instalación MySQL](https://dev.mysql.com/doc/refman/8.0/en/general-installation-issues.html)
- [Instalación WORKBENCH](https://dev.mysql.com/downloads/workbench/)

### Previo a usarlo - MySQL && WORKBENCH

1) Bajar los archivos de la rama **main** corriendo los siguientes comandos en la terminal de tu computadora:

```plaintext
git init
git remote add origin https://github.com/Giulianni/digitalBooking_FinalProject.git 
git pull origin main
```

2) La misma descargará una carpeta: Base de datos con dos scripts con extensión sql, donde:

- DigitalBooking_DataBase.sql --> Un script vacío que crea la base de datos y en el cuál levantaremos las entidades desde JAVA.
- Estructura_BaseDeDatos_DigitalBooking.sql --> Un script que contiene la estructura final de la base de datos. Con Reverse Engineer se obtiene el diagrama DER que se buscará crear posteriormente a través de Hibernate.

3) Si todo salió bien, entrar al WORKBENCH y a su conexión por defecto (recordar el usuario y contraseña configurados al instalar MySQL). Abrir el script **DigitalBooking_DataBase.sql**. Correr los comandos:

```plaintext
CREATE SCHEMA IF NOT EXISTS `DigitalBooking_DB1` DEFAULT CHARACTER SET utf8 ;
USE `DigitalBooking_DB1` ;
```

4) Actualizar la sección de **schemas**. Ahora debería verse en dicha sección la base de datos **DigitalBooking_DB1**, aunque sin ninguna tabla creada.

### Primer uso - JAVA

1) Bajar esta rama del repositorio. Si estas trabajando en una carpeta nueva, correr los siguientes comandos en la teminal de tu computadora:

```plaintext
git init
git remote add origin https://github.com/Giulianni/digitalBooking_FinalProject.git 
git pull origin main
```

2) Deberías tener esta estructura de carpetas

```plaintext
DigitalBookingBackEnd
│   README.md
│   mvnw
│   mvnw.cmd
│   pom.xml
└───src
```

3) En el archivo application.properties del path `/src/resources/application.properties` tener en cuenta de los siguientes campos:

- spring.datasource.url --> hace referencia a la URL donde esta el servicio de tu mysql y el nombre de la base de datos. Tener en cuenta el puerto donde esta corriendo la base de datos en su conexión local y el nombre de la base de datos configurada en el archivo DigitalBooking_DataBase.sql, por ejemplo:

```plaintext
spring.datasource.url=jdbc:mysql://localhost:3306/DigitalBooking_DB1
```

- spring.datasource.username && spring.datasource.password --> hace referencia al usuario y contraseña mediante la cual se establece la conexión a la base de datos (recordar la contraseña configurada al instalar MySQL).

```plaintext
spring.datasource.username=
spring.datasource.password=
```

4) Una vez configurado el application.properties, correr el proyecto ejecutando los siguientes comandos en la terminal (posicionándose en la carpeta del proyecto):

```plaintext
cd DigitalBookingBackEnd
mvn clean package
```

5) Luego de correr el comando `mvn clean package` la estructura de carpetas debería ser:

```plaintext
DigitalBookingBackEnd
│   README.md
│   mvnw
│   mvnw.cmd
│   pom.xml
└───src
└───target
```

6) Ahora, mediante los siguientes comandos debería ya estar corriendose el proyecto en el puerto configurado por defecto (el puerto 8086):

```plaintext
cd target
java -jar DigitalBooking.jar
```

7) Si todo salió bien, entrar al WORKBENCH y a su conexión por defecto. Al actualizar la sección de **schemas**, la misma ahora debería contener las tablas correspondientes creadas en JAVA.

### Documentación

Una vez corriendo el proyecto, se puede acceder a la url <http://localhost:8086/swagger-ui.html> y ver la documentación.

## Infraestructura

### Actual

* Diseño de insfraestructura en AWS conteniendo principales servicios para estructuras de red, servidores, almacenamiento externo, bases de datos y seguridad.
* Implementación de instancias comprendidas en free-tier:
  * EC2: t2.micro, vpc, key privada, security groups correspondientes para acceso publico y privado, instalación de web server, instalación de paquetes y scripts necesarios para la ejecución de la aplicación Java y React.
  * RDS: Base de datos MySQL, SGs correspndientes, tablas y relaciones, conexión a EC2, conexión a instancia desde Workbench.
  * S3: Almacenamiento externo de imagenes de productos, generación de urls e inserción en la base de datos de las imagenes a los productos correspondientes.
* Deploy de la aplicación en EC2: Deploy manual. Configuración de servidor(puertos, permisos, enrutamientos). Script spring.service para la ejecución automática del jar conteniendo el back end. Deploy manual de front.
* Generación de Ip elastica asociada a instancia ec2 y asociación de ip a un dominio para una url amigable.

### Visión para escalar la infraestructura

#### Acceso a la WEB

[Digital Booking](http://digitalbooking.one/)

#### Requerimientos

1) Diagramar infraestructura para AWS:

- Red interna
- Web/App servers
- Almacenamiento externo
- Base de datos
- Security groups

#### Acceso al diagrama de la estructura en "Diagrams.net"

- [Digital Booking AWS](https://drive.google.com/file/d/1o-OgsRSYSK4tl9_tP9dSR905KugvxR2H/view?usp=sharing)

#### Infraestructura explained

 1) Selección de la región **us-east-1**
 2) Creación de una Red privada **VPC**
 3) Creación de un **Internet Gateway** para que sea posible y controlado el acceso de internet dentro de la VPC
 4) Selección de dos **Availability Zones** que son lo que simulan al Data Center.
 5) Desarrollo de **subredes** para la instancia de nuestros servicios con escope a nivel de Availability zones:
    - **Public subnet** - Load balancer que puede estar presente en mas de una AZ y distribuirá al tráfico ingresante en multiples maquinas EC2. - NAT: Para posibles traficos de salida.
    - **Private subnet** - En estos niveles ubicaremos al Web Server (para deploy del Front de nuestra aplicación), Application Server (para el deploy del back de nuestra aplicación). Estos servidores serán instancias de EC2 que permiten autoescalado. EBS es el servicio de AWS para los discos. - En el tercer nivel ubicamos a la BBDD relacionar, que en el caso de AWS es el servicio RDS.
 6) Utilización de un **External storage** que en este caso será la utilización de un Bucket S3.
 7) Utilización de **CloudFront** que es un servicio que proporciona una API que permite distribuir contenido con baja latencia y alta velocidad (CDN) en la transferencia de datos gracias a que entrega las solicitudes mediante una red de ubicaciones de borde internacional. Esto será utilizado para distribuir el contenido del S3. Aquí los **Edge Locations** actuarán cómo un caché.
 8) **Route53** es el servicio de **DNS** de AWS que mapeará nuestro dominio a la **dirección IP del balanceador**.
 9) Definición de **Route Table** a modo de ejemplo con principales accesos.
10) Diseño de 4 posibles **Security groups**:
11) Ubicación de Amazon **CloudWatch**, herramienta que nos permitirá monitorear nuestra infraestructura de manera gráfica.

#### Documentos oficiales

Para más información:

- [Regiones y Availability zones](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-regions-availability-zones.html)
- [VPC](https://aws.amazon.com/es/vpc/faqs/)
- [Internet gateway](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Internet_Gateway.html)
- [Interacción Web Server, Application Server y DDBB](https://stackoverflow.com/questions/936197/what-is-the-difference-between-application-server-and-web-server)
- [Load balancer](https://aws.amazon.com/es/elasticloadbalancing/faqs/?nc=sn&loc=5)
- [NAT](https://docs.aws.amazon.com/es_es/vpc/latest/userguide/vpc-nat-gateway.html)
- [S3](https://aws.amazon.com/es/s3/?nc1=h_ls)
- [Route53](https://aws.amazon.com/es/route53/faqs/http)
- [CloudFront](https://aws.amazon.com/es/cloudfront/faqs/#Caching)
- [Security groups en AWS](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_SecurityGroups.html)
- [CloudWatch](https://aws.amazon.com/es/cloudwatch/)
- [Lambda](https://aws.amazon.com/es/lambda/)

#### Imagen

![DigitalBooking_InfraAWS](https://s3.amazonaws.com/digitalbooking.equipo3c3/DocTecnica/DigitalBooking_infra.png)

## Testing y calidad

En el siguiente link encontraremos el acceso al reporte final de testing del proyecto:

[https://docs.google.com/spreadsheets/d/1l4KSzrt84fLPdeqttkbJ6JbMTkq-9h8zJA2Z9kXP-ao/edit?usp=sharing](https://docs.google.com/document/d/e/2PACX-1vRovoXqXBUurRyThvBC80T-80wvXlmJdDzPeS4Y5fhmXQvYTMlrbXZjcTEWUgWNl9FutTOGPBJMaWIk/pub)

## 
