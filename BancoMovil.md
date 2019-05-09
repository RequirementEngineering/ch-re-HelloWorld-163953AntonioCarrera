Introducción 

Propósito 

El documento aquí realizado tiene como propósito principal definir todos y cada uno de los requerimientos para la implementación de una aplicación para los distintos bancos de la ciudad pero,  ¿para qué?, esta aplicación tiene el propósito de evitar largas filas o demasiada acumulación de gente en las diferentes sucursales del banco,permitiendo que desde la app móvil los clientes de dicho banco puedan  realizar trámites como: reposición de tarjetas,  apertura de cuentas, reportes de robo o extravio (su tarjeta nueva se le hará llegar a su domicilio), citas para obtención de créditos hipotecarios,etc.

En este documento analizaremos los requerimientos del cliente para el sistema a realizar y realizaremos un plan de acción para la creación de nuestra app.

Alcance

BancoMovil

-Desarrollaremos nuestra aplicación en el lenguaje java y podremos realizar los distintos tramites que se realizan en el banco ,con algunas excepciones.

-Desarrollaremos también un sistema para computadora ,que tendrán instaladas las pc’s de las sucursales donde se enviaran las peticiones de tramites que tienen los clientes,cabe destacar que en su base de datos obviamente ya se encontraran los datos de sus clientes con información  como nombre,dirección y numero de teléfono .

-Por ultimo se desarrollara un software mas pequeño para el banco ,que consistirá en un altas bajas y cambios en cuestión a las tarjetas que expide,asi el banco llevara un control de sus tarjetas y sabra cuando necesitaría pedir mas para evitar la falta de tarjetas.

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


1.	Cliente: El usuario realizara el trámite necesario desde la app instalada en su Smartphone o tableta.

2.	Ejecutivo: El ejecutivo recibirá la notificación sobre el tramite solicitado por el cliente y lo realizara lo más pronto posible.

3.	Repartidor: La función de este es repartir las tarjetas que soliciten por robo o extravio,este solo repartirá a las zonas cercanas a la sucursal donde fue expedida la misma.

4.  Gerente:la funcion del gerente es checar movimientos y todo los tramites realizados ya sean diariamente,semanalmente o mensualmente segun lo requiera el banco.

5.  Buro de Credito.La funcion del buro de credito es checar que el cliente no se encuentre en su base de datos con adeudo en alguna institucion bancaria,inmobiliaria etc,,en caso de que el cliente este o no este en buro,este le notificara al banco la investigacion sobre el cliente para decidir si es apto o no para los prestamos.

<img src="https://raw.githubusercontent.com/RequirementEngineering/ch-re-HelloWorld-163953AntonioCarrera/master/Use%20Case/bancomovil.png">

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
