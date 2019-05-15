Table of contents

1.Introduction

  *Purpose

  *Scope

  *Definitions, acronyms, and abbreviations

  *References

  *Overview

2.Overrall description

  *Business Managment Process

  *Product perspective

    *Product Functions

  *User characteristics

  *Constrains

3.Specific requirements

  *Interface

  *Requirements

    *Functional requirements

    *Non functional requirements

    *User requirements

    *System requirements

4.Appendices

  *Elicitation process

Introducción 

Propósito 

El documento aquí realizado tiene como propósito principal definir todos y cada uno de los requerimientos para la implementación de una aplicación para los distintos bancos de la ciudad pero,  ¿para qué?, esta aplicación tiene el propósito de evitar largas filas o demasiada acumulación de gente en las diferentes sucursales del banco,permitiendo que desde la app móvil los clientes de dicho banco puedan  realizar trámites como: reposición de tarjetas,  apertura de cuentas, reportes de robo o extravio (su tarjeta nueva se le hará llegar a su domicilio), citas para obtención de créditos hipotecarios,etc.

En este documento analizaremos los requerimientos del cliente para el sistema a realizar y realizaremos un plan de acción para la creación de nuestra app.

Alcance

BancoMovil

-Desarrollaremos nuestra aplicación en el lenguaje java y podremos realizar los distintos tramites que se realizan en el banco ,con algunas excepciones.

-Desarrollaremos también un sistema para computadora ,que tendrán instaladas las pc’s de las sucursales donde se enviaran las peticiones de tramites que tienen los clientes,cabe destacar que en su base de datos obviamente ya se encontraran los datos de sus clientes con información  como nombre,dirección y numero de teléfono .


Referencias

https://www.banorte.com/wps/portal/banorte

https://www.banamex.com/

https://www.banregio.com/

https://www.bancomer.com/

https://www.hsbc.com.mx/

https://www.bancoppel.com/main/index.html

https://www.santander.com.mx/

Visión general

Con la realizacion  de nuestra app buscamos la reduccion de filas y acumulamiento de clientes en la sucursal ya que la mayoria son bancos pequenos, para solo hacer tramites que hay veces que son muy cortos y es inutil esperar tanto tiempo,asi se agilizara todo lo que tenga que ver con el banco, asi, beneficiando al banco como a los clientes.

Descripción general

BPM

PROCESO:

1.-selceccion de banco o bancos

2.-introduccion de los datos solicitados (usuario,contraseña,numero de cuenta,etc.)

3.-selccion de tramite (reporte,cita,etc)

4.-recepcion de la solicitud

5.-analisis de solicitud

6.-se envia la solicitud al gerente

7.-el gerente analiza la solicitud 

8.-el gerente envia los datos del cliente a buro de credito para su analisis

9.-el buro se encarga de notificar al gerente si es apto el cliente

10.-el gerente notifica al ejecutivo si es apto o no el cliente

11.-el ejecutivo hace la notificacion al cliente si su solicitud fue o no aceptada.

<img src="https://github.com/RequirementEngineering/ch-re-HelloWorld-163953AntonioCarrera/blob/master/BPM/BancoMovil.jpg">

<img src="https://github.com/RequirementEngineering/ch-re-HelloWorld-163953AntonioCarrera/blob/master/BPM/Bancos%20Disponibles.jpg">

<img src="https://github.com/RequirementEngineering/ch-re-HelloWorld-163953AntonioCarrera/blob/master/BPM/Datos%20a%20Ingresar.jpg">

<img src="https://github.com/RequirementEngineering/ch-re-HelloWorld-163953AntonioCarrera/blob/master/BPM/Tramites%20Disponibles.jpg">

<img src="https://github.com/RequirementEngineering/ch-re-HelloWorld-163953AntonioCarrera/blob/master/BPM/Analisis.jpg">


Perspectiva del Producto

Nuestro sistema facilitara la obtención de servicios y tramites de los distintos bancos, pudiendo realizar la mayoría de los tramites a través de nuestra app.

•	Reposición de tarjetas

•	Apertura de cuentas

•	Reportes de robo o extravío (su tarjeta nueva se le hará llegar a su domicilio)

•	Citas para obtención de créditos hipotecarios

•	Etc.

Encontraremos información sobre:

•	Requisitos para cada uno de los tramites

•	Ubicación de la sucursal más cercana al domicilio

•	Números de teléfono para cualquier duda o aclaración

•	Correo electrónico

La aplicación será gratuita para cualquier sistema operativo

Funciones del Producto

	Las principales funciones del producto es minimizar el tiempo de espera y filas en las diferentes sucursales de los distintos bancos de la ciudad.

	Llevar un control para el banco de los tramites que se realizan a diario en sus distintas sucursales

Características del Usuario

Hay 5 tipos de usuarios

 Usuario  | Descripcion
 -------  | -------------
 Cliente      | El usuario realizara el trámite necesario desde la app instalada en su Smartphone o tableta.
 Ejecutivo    | El ejecutivo recibirá la notificación sobre el tramite solicitado por el cliente y lo realizara lo más pronto posible.
 Repartidor   | La función de este es repartir las tarjetas que soliciten por robo o extravio,este solo repartirá a las zonas cercanas                   a la sucursal donde fue expedida la misma.
 Gerente      | la funcion del gerente es checar movimientos y todo los tramites realizados ya sean diariamente,semanalmente o                           mensualmente segun lo requiera el banco.
 Buro         | La funcion del buro de credito es checar que el cliente no se encuentre en su base de datos con adeudo en alguna                         institucion bancaria,inmobiliaria etc,,en caso de que el cliente este o no este en buro,este le notificara al banco la                   investigacion sobre el cliente para decidir si es apto o no para los prestamos.
 
CASOS DE USO

<img src="https://github.com/RequirementEngineering/ch-re-HelloWorld-163953AntonioCarrera/blob/master/Use%20Case/bancomovil.png">

Usuario  | Descripcion
 ----- | -------------
 Nombre | Banco Movil
 Autor | Marco Antonio Carrera Jaquez
 Fecha | 14/05/2019
 Descripcion |La aplicacion tendra las opciones necesarias para hacer tramites desde celular o tableta,asi como consulta de saldos
 Actores | cliente,ejecutivo,gerente,repartidor,buro de credito
 Condiciones Previas | Para la utilizacion de la app el cliente tiene que tenerla en su telefono y contar con cuenta en el banco obviamente
 Flujo | *Cliente.-Ingresa a la aplicacion e interactua para decidir que tramite desea, *Ejecutivo.- Recibe la solicitud de tramite para poder realizarla lo mas pronto bosible,*Buro.- checa el estatus del cliente,*Gerente.-Autoriza o no el credito o prestamo. *Repartidor.- reparte las tarjetas  
 Flujo alternativo | En el caso que se rechaze algun tramite el ejecutivo notificara al cliente
 Post-condiciones | Se guardaran todos los tramites en la base de datos del sistema
 
 CASO DE USO 1 
 
 <img src="https://github.com/RequirementEngineering/ch-re-HelloWorld-163953AntonioCarrera/blob/master/Use%20Case/Use%20case%201.png">
 
 Usuario  | Descripcion
 ----- | -------------
 Nombre | Cliente
 Autor | Marco Antonio Carrera Jaquez
 Fecha | 14/05/2019
 Descripcion | El cliente ingresara a la aplicacion e interactuara con los tramites a realizar o estados de cuenta etc,
 Actores | Cliente
 Condiciones Previas | Para la utilizacion de la app el cliente tiene que tenerla en su telefono y contar con cuenta en el banco obviamente
 Flujo | *El cliente entra a la aplicacion ,ingresa, si es la primera vez le pedira todos sus datos ,elige banco o bancos y listo ya no hay necesidad de reingresar ningun dato a menos que instale la aplicacion en un telefono distinto.cada vez qyue realize un tramite debera esperar la respuesta del banco via telefonica,sms o correo electronico.    

 CASO DE USO 2 
 
  <img src="https://github.com/RequirementEngineering/ch-re-HelloWorld-163953AntonioCarrera/blob/master/Use%20Case/use%20case%202.png">
  
   Usuario  | Descripcion
 ----- | -------------
 Nombre | Ejecutivo
 Autor | Marco Antonio Carrera Jaquez
 Fecha | 14/05/2019
 Descripcion |El ejecutivo ingresara al software bancario, revisara la peticion del usuario,revisara su base de datos,despues este enviara la peticion al  gerente.
 Actores | Ejecutivo,Gerente
 Flujo | *El ejecutivo ingresara al software bancario, revisara la peticion del usuario,revisara su base de datos,despues este enviara la peticion al  gerente.el ejecutivo esperara que el gerente autorize o no para dar aviso a el cliente el resultado de su peticion.
  
 CASO DE USO 3
 
  <img src="https://github.com/RequirementEngineering/ch-re-HelloWorld-163953AntonioCarrera/blob/master/Use%20Case/use%20case%203.png">
  
    
 Usuario  | Descripcion
 -----       | -------------
 Nombre      | Gerente
 Autor       | Marco Antonio Carrera Jaquez
 Fecha       | 14/05/2019
 Descripcion | El Gerente revisara las peticiones enviadas por el ejecutivo 
 Actores     | Ejecutivo,Gerente,Buro
 Flujo       | *El Gerente revisara las peticiones enviadas por el ejecutivo,y posteriormente enviara los datos al buro de credito para checar el status del cliente.
 
 CASO DE USO 4
 
  <img src="https://github.com/RequirementEngineering/ch-re-HelloWorld-163953AntonioCarrera/blob/master/Use%20Case/use%20case%204%20(1).png">
 
 Usuario  | Descripcion
 -----    | -------------
 Nombre | Buro de Credito
 Autor  | Marco Antonio Carrera Jaquez
 Fecha  | 14/05/2019
 Descripcion | El buro de credito checara el status del cliente para determinar si el cliente es apto o no para el tramite realizado(solo hipotecas o prestamos)
 Actores | Gerente,Buro
 Flujo | *El buro de credito checara el status del cliente para determinar si el cliente es apto o no para el tramite realizado(solo hipotecas o prestamos) ,posteriormente el buro informara al gerente correspondiete la decision.
 

Restricciones

•	El cliente deberá contar con correo electrónico

•	Ser cliente activo en cualquier banco

Suposiciones y Dependencias

•	La aplicación funcionara con cualquier sistema operativo móvil.

•	Dependera de una conexión wifi o de datos móviles para su funcionamiento.

•	Android 5.0 en adelante e ios 9 en adelante

Requerimientos Especificos


Interfaz

Interfaz de Usuario

Esta interfaz debe ser fácil de utilizar,los colores van ir variando dependiendo del banco de su preferencia,banorte (rojo y blanco),Bancomer(azul y blanco) y asi respectivamente.

	Al abrir nuestra aplicación nos permitirá seleccionar el/los banco(s) en los que el usuario ya es cliente

	En caso de ser mas de un banco al que esta inscrito,la aplicación le pedirá ingresar sus credenciales (correo y contraseña)

	En la parte superior aparecerá el logotipo del banco que se esta utilizando

	Parte superior izquierda se encontrara información sobre el banco,ubicaciones,teléfonos de contacto y correo electrónico de la empresa y también el perfil del usuario.

	Parte superior derecha vendrá el menú con los diferentes tramites que se pueden realizar en línea.

	Al final de haber realizado el tramite se mostrara un mensaje donde aparecerá el tramite realizado ,el tiempo en el que se habrá realizado su tramite,y dando las gracias por usar la aplicación móvil.

Interfaz de la Empresa

	Ejecutivos: Las solicitudes para los distintos tramites,se enviaran obviamente a las bases de datos del banco al cual pertenece el cliente,ahí el ejecutivo visualizara cada tramite solicitado por el cliente y asi podrá realizarlo,cabe destacar  que los tramites se agruparan de acuerdo a el tipo de tramite,es decir ,un grupo de robo o extravio,otro grupo de solicitud de crédito hipotecario,etc.

	Gerente: El gerente tendrá en su computadora el mismo software que los ejecutivos asi podrá visualizar que tramites son los que tienen mayor demanda para el banco y que tan rápido sus ejecutivos trabajan en estos mismos.

Restricciones de Memoria

	Para los smartphones o tabletas deberán contar con minimo 2gb de ram

	Para las pc’s de los bancos deberán contar con minimo 1.5gb de ram


Atributos del sistema de software

Disponibilidad

	El sistema estará disponible 24/7 e incluso los días inhábiles 

	En dado caso que el sistema se caiga o la aplicación falle y tenga que reiniciarse ,el usuario no tendrá que reingresar o rellenar los campos que ya haya llenado ya que la aplicación tendrá funcion de autoguardarse cada vez que el cliente complete un campo o alguna sección.

Seguridad

	Para empezar se contaran con políticas de acceso yclasificacion de la información.

	Al ser una empresa bancaria tendremos una firma electrónica

	Toda información proporcionada por el usuario será cifrada para protegerla de personas malintencionadas.
Mantenimiento

	A este sistema se le dara mantenimiento dos veces por semana,con un software programado para ello.


Proceso de Elicitacion

El proceso de elititacion se realizo a travez de una entrevista con un ejecutivo del banco.

el ejecutivo comenta que dia a dia se llenan las salas de espera por motivos de tramites que se tienen que hacer directo en el banco.

"Necesitamos primeramente un sitema que permita realizar diversos tramites desde la aplicacion para telefono o tablet.

Necesitamos obviamente que el cliente cuente con correo electronico y sea cliente de nuestro banco.

Necesito tener un sistema para nuestras computadoras donde se reciban las peticiones de tramite de nuestros clientes.

El sistema debe enviarme una alerta para saber que se necesita realizar un tramite 

El sistema deve dividir los tramites, es decir:

-solicitudes de prestamo

-citas

-solicitud de hipoteca

-reposicion de tarjetas

-reporte de robo o extravio ,etc.

Tambien se necesita que lleve un contador para saber cuales tramites son los que mas se realizan en nuestra sucursales y al final de la semana nos de un reporte de todos los tramites realizados"

REQUERIMIENTOS FUNCIONALES

Cliente:

-Inicio de sesión.

-Tramites que se desean realizar

-Consultas de saldos

-Consultas de numeros telefonicos y ubicaciones de los distintos bancos

Empresa:

-Inicio de sesión.

-Sistema para ejecutivos donde llegaran y se almacenaran los tramites pedidos por el cliente

-Base de datos donde se almacenaran todos y cada uno de los tramites ya concretados y los que aun estan en revision.

REQUERIMIENTOS NO FUNCIONALES

-Estabilidad en almacenamiento y procesamiento

-La seguridad tanto para el cliente como para los ejecutivos en cuestion a proteccion de los datos al momentos del ingreso en usuario y contrasena para evitar el acceso a gente que no debe.

-Mantenimiento del software y nuestra aplicacion ,esta estara programada para darle mantenimento automaticamente.

BPM

PROCESO:

1.-selceccion de banco o bancos

2.-introduccion de los datos solicitados (usuario,contraseña,numero de cuenta,etc.)

3.-selccion de tramite (reporte,cita,etc)

4.-recepcion de la solicitud

5.-analisis de solicitud

6.-se envia la solicitud al gerente

7.-el gerente analiza la solicitud 

8.-el gerente envia los datos del cliente a buro de credito para su analisis

9.-el buro se encarga de notificar al gerente si es apto el cliente

10.-el gerente notifica al ejecutivo si es apto o no el cliente

11.-el ejecutivo hace la notificacion al cliente si su solicitud fue o no aceptada.
