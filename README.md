Novedades versi�n 5.1.0.9
--
**Versi�n 5.1.0.9**: Se actualiza el despachador de correos SMTP para permitir su configuraci�n mediante par�metros registrados en el panel de administraci�n. Estos par�metros determinan si los correos se env�an de forma as�ncrona (modo predeterminado y actual) y si se requiere emplear diversos ajustes personalizados seg�n las necesidades del cliente. De este modo, se garantiza una mayor flexibilidad y adaptabilidad del sistema para cumplir con los requisitos espec�ficos.

**Nota:** Se debe tener en cuenta que las contrase�as usadas para los servidores SMTP de **Gmail** y **Office** son contrase�as de aplicaciones, se deben crear directamente en las configuraciones de la cuenta.


Actualizaci�n ORM v5.1.0.9
--
S� actualmente ya cuenta con la versi�n instalada 5.1.0.8, debe seguir con los siguientes pasos para la actualizaci�n.

1. Descargar los siguientes componentes disponibles en el repositorio:
    * ORM.exe
    * Datos.sql

2. Reemplazar archivo ORM.exe en su carpeta instalada ORM.
![alt text](image-2.png)

3. Aplicar los objetos nivel de base de datos sobre el esquema ORM. Verificar su correcta aplicaci�n consultando la tabla OPT_CONFIGURATION:
![alt text](image-3.png)


4. Verificar aplicaci�n de par�metros desde el aplicativo.
![alt text](image.png)

    Los par�metros configurados por defecto al ser aplicados vienen configurados de la siguiete manera:
    ![alt text](image-1.png)


Despachando correo
--

![alt text](image-6.png)


Una vez realizado los pasos anteriores debe ir al m�dulo de **Consultas**  y configurar el servidor SMTP si a�n no lo ha programado, primero se debe abrir el despachardor y seleccionar la opci�n **Configurar servidor SMTP**
![alt text](image-16.png)

Una vez creada la contrase�a de aplicaciones seg�n su cliente de correos, se debe confiugrar con las credenciales.
![alt text](image-17.png)
Una vez configuradas dichas credenciales se puede continuar con los siguientes pasos.







1. Levantar el despachador de tareas, es de vital importancia que este se encuentre activo para realizar el despacho de tareas post. Para activalor se debe dar clic en la pesta�a superior llamada **Consultas programadas**.
![alt text](image-7.png)
* Se desplegara la siguiente pesta�a:
![alt text](image-8.png)
* Se debe abrir una consulta y abrir la pesta�a de **Consultas programadas** y se habilitara el bot�n de **Programar ejecuci�n**.
![alt text](image-9.png)
* Se debe seleccionar la periodicidad de la tarea post

![alt text](image-10.png)
* Luego dar clic en crear nueva tarea
![alt text](image-11.png)
* Seleccionar el tipo de tarea post:
![alt text](image-12.png)
* Para el caso de ejempo se va usar el tipo **Generar archivo y Enviar por correo**.
![alt text](image-13.png)
Se debe seleccionar el tipo de archivo a generar, la ruta en donde se va almacenar y los correos de origen y destino. Dar clic en aceptar.

* Dar clic en **Aceptar** 
![alt text](image-14.png)

* Visualizar la tarea programda desde la pesta�ana inferior **Ejecuci�nes programadas**
![alt text](image-15.png)



