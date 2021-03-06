# Biblioteca ECI
## Proyecto final de CVDS (Ciclos de Vida Del Desarrollo de Software). Periodo 2019-2
## Escuela Colombiana de Ingeniería Julio Garavito

### Integrantes

+  Juan Sebastián Frásica Galeano (Team developer)
+  Andrés Felipe Marcelo (Team developer)
+  Santiago Rubiano (Team developer)
+  David Vargas (Team developer)

### Profesor
+ Julián Velasco (Producto Owner)

## Descripción del producto

## Arquitectura y diseño detallado

### Modelo E-R (Entidad-Relación)
![ER](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/EntidadRelacion.png)

### Diagrama de paquetes
![Diagrama-de-clases-sprint-1-y-2](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/Diagrama_de_clases.png)

### Enlace de la aplicación en Heroku
http://ecibrary.herokuapp.com/

### Descripción de la arquitectura y tecnologías utilizadas
La aplicación está construida en 3 capas:

#### Capa de presentación
En esta capa se hizo uso de tecnologías como:
+  JSF (Java Server Faces)
+  Primefaces

#### Capa de aplicación
Aquí se usaron tecnologías:
+  Java
+  Google Guice (Un framework para inyección de dependencias)
+  Maven (Herramienta para gestión de dependencias)
+  Apache Shiro (Framework para autentiticación)

#### Capa de persistencia de datos
Se usó un motor de bases de datos **PostgreSQL** y la herramienta **myBatis**, la cual se encarga de la persistencia (mappea sentencias SQL y procedimientos almacenados con objetos a partir de ficheros XML o anotaciones).



### Manual de usuario:
Primero, cuando se ingrese al link http://ecibrary.herokuapp.com/ aparecerá la siguiente vista:
![Iniciar sesión](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/Manual%20de%20usuario/1.jpg)


Allí cualquier persona podrá iniciar sesión o podrá consultar los recursos disponibles.
Al hacer click en “Consultar recursos” se mostrarán los recursos disponibles. Sin embargo, esta vista es meramente informativa ya que no podrá realizar ninguna otra acción aparte de ver. Se muestra a continuación:

#### Vista consultar recursos (sin iniciar sesión):
![Sin iniciar sesion](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/Manual%20de%20usuario/2.jpg)

Por otra parte, al hacer click en Log In se redirigirá a otra vista, en donde se valida el inicio de sesión. 
![Login](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/Manual%20de%20usuario/3.jpg)

Algunas credenciales para iniciar sesión:
* Como administrador:
  *   Email: cvds@cvds.com
  *   Contraseña: 123   
* Como comunidad:
  *   Email: santiago.aponte@mail.escuelaing.edu.co
  *	Contraseña: invitado

    
#### Administrador:   
Al iniciar sesión como administrador se podrán realizar las siguientes tareas:
* Consultar todos los recursos.
* Modificar el estado de un recurso.
*	Registrar un nuevo recurso.
*	Ver reporte de ocupación.

![Admin](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/Manual%20de%20usuario/4.jpg)

Aquí se podrán ver todos los recursos en una tabla, donde se muestra información específica de cada uno.    


El administrador también puede modificar el estado de un recurso haciendo click en el engranaje que tiene cada recurso
![Modificar estado](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/Manual%20de%20usuario/5.jpg)   

Los 3 estados posibles del recurso son:
* Disponible
*	En mantenimiento
*	No disponible   

En la vista de registrar un nuevo recurso aparecerá lo siguiente:   
![Registrar recurso](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/Manual%20de%20usuario/6.jpg)   


En la vista de reporte de ocupación se muestran algunos gráficos y estadísticas del estado y uso de la biblioteca:
![Reporte](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/Manual%20de%20usuario/7.jpg)   


#### Comunidad:
Al iniciar sesión como comunidad se podrán realizar las siguientes tareas:
*	Consultar recursos disponibles.
*	Realizar una reserva.
*	Ver reservas.
*	Ver mis reservas.
*	Poder cancelar una reserva.

![Recursoss disponibles](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/Manual%20de%20usuario/8.jpg)     

   
   
Aquí solo se podrán ver los recursos disponibles, y se puede proceder a reservar determinado recurso al hacer click en el lápiz para editar


![Recursoss disponibles](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/Manual%20de%20usuario/9.jpg)   


Las reservas al recurso seleccionado se realizan mediante el calendario.   
Dichas reservas pueden ser normales o recurrentes.    
Las reservas recurrentes pueden ser diarias, semanales o mensuales.    

![calendario](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/Manual%20de%20usuario/10.jpg)  

![reservaDesdeCalendario](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/Manual%20de%20usuario/11.jpg)  

Cuando se realiza una reserva esta aparecerá en el calendario:

![menuReservas](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/Manual%20de%20usuario/16.JPG)  

Y si se quieren realizar otras reservas a la misma hora solo permitirá cuando no se solapen, en caso contrario mostrará algo así:   
![menuReservas](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/Manual%20de%20usuario/17.JPG)  
Sin embargo, los horarios que no se solapen sí se podrán reservar:
![menuReservas](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/Manual%20de%20usuario/18.JPG)  





Al momento de ver mis reservas el usuario puede ver lo siguiente:   
![reservassss](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/Manual%20de%20usuario/12.JPG)  




#### Reservas canceladas:

![reservasCanceladas](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/Manual%20de%20usuario/13.JPG)  

#### Reservas en curso:

![reservasEnCurso](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/Manual%20de%20usuario/14.JPG)  

#### Reservas pasadas:
![reservasPasadas](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/Manual%20de%20usuario/15.JPG)    

Finalmente, si un usuario accede a una página no autorizada (Por ejemplo, un usuario logeado como comunidad trata de ingresar a la página del administrador) le aparecerá el error HTTP 401 (No autorizado) de manera personalizada:

![noAutorizado](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/Manual%20de%20usuario/19.JPG)   

Y también se tiene control de ello para páginas que no existen, donde aparece el error HTTP 404 (No encontrado):

![404](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/Manual%20de%20usuario/20.JPG)   



### Integración continua
[![CircleCI](https://circleci.com/gh/CVDS-ECI/ECI-Biblioteca.svg?style=svg)](https://circleci.com/gh/CVDS-ECI/ECI-Biblioteca)

### Calidad del código
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/64ad0e4484824d6ab2794f5535063e6f)](https://www.codacy.com/manual/sebastianfrasic/ECI-Biblioteca?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=CVDS-ECI/ECI-Biblioteca&amp;utm_campaign=Badge_Grade)

### Cubrimiento de pruebas
Mediante el plugin de Jacoco se realizó el porcentaje de cubrimiento de pruebas unitarias del proyecto:

![cubrumiento](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/Manual%20de%20usuario/21.JPG)   

## Descripción del proceso
Se trabajó mediante la metodología ágil Scrum. Durante todo el proceso se hicieron 3 sprints. Cada uno con una duración de 2 semanas.

## Descripción sprint 1

Burndown chart and backlog

+ Burndown chart: https://tree.taiga.io/project/sebastianfrasic-gestion-de-recursos-biblioteca/taskboard/sprint-1-15837

En este sprint se completaron casi todos los objetivos por realizar. Cada integrante del equipo cumplió con sus deberes en el tiempo adecuado y con una calidad óptima. La página de incio de sesión sirve correctamente y se puede realizar ciertas funciones dependiendo del usuario que inicie sesión. Faltó arreglar detalles como cambiar las vistas cuando se logea la comunidad y consultar un recurso. 

![Burndown chart and backlog sprint 1](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/BURNDOWN%20CHART%20AND%20BACKLOG%20SPRINT%201.png)

## Descripción sprint 2

Burndown chart and backlog

+ Burndown chart: https://tree.taiga.io/project/sebastianfrasic-gestion-de-recursos-biblioteca/taskboard/sprint-2-8608

En este sprint quedaron varias tareas abiertas/pendientes por hacer debido a que hubo problemas con el tiempo que cada integrante tuvo para realizar. Además de que tocó hacer una refactorización de la parte de UX y la mayoría de Front, en lo cual un integrante estuvo bastante desapegado con el trabajo que se tenía que hacer.
Las tareas que quedaron incompletas fueron las de reservar un recurso y la de ver el calendario con las reservas.
Acá también se corrigieron algunos issues del sprint 1.
![Burndown chart and backlog sprint 2](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/BURNDOWN%20CHART%20AND%20BACKLOG%20SPRINT%202.png)


## Descripción sprint 3

Burndown chart and backlog

+ Burndown chart: https://tree.taiga.io/project/sebastianfrasic-gestion-de-recursos-biblioteca/taskboard/sprint-3-5679

Finalmente, en este último sprint se completaron todas las tareas pendientes del segundo sprint, y se realizó correctamente el resto de tareas asignadas para este sprint.
Lo único que no se pudo hacer como lo pedían en el requisito fue lo de filtrar los reportes de ocupación y generar el archivo Excel.

Podría decirse que se cumplieron con todas las tareas solcitadas, y que el proyecto está en un excelente estado en cuanto a funcionalidad y calidad.

![Burndown chart and backlog sprint 3](https://github.com/CVDS-ECI/ECI-Biblioteca/blob/master/img/BURNDOWN%20CHART%20AND%20BACKLOG%20SPRINT%203.PNG)




