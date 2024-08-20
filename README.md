# StarkLabsIndustryMD
Primeramente vamos a la Pagina de VirtualBox para descargar la ultima versión del instalador
![image](https://github.com/user-attachments/assets/9e9c5e42-a2d3-4388-a081-28958070c554)

Luego lo buscamos en el File Explorer de nuestra computadora para ejecutar la instalación
![image](https://github.com/user-attachments/assets/91825420-13d7-4765-822a-57392a6d6975)

Una vez abirto el Executable, procedemos a darle Next y demás acciones para culminar la instalación del Virtual Box
![image](https://github.com/user-attachments/assets/67cae6e7-47ba-4fa1-80aa-437a1e455326)

Acá podemos ver el Virtual Box instalado
![image](https://github.com/user-attachments/assets/889d3316-444f-409c-9b9b-fb6671312239)

Se crea la Maquina Virtual con Windows Server 2019
![image](https://github.com/user-attachments/assets/81ff3268-af9e-48ea-a493-6b7f878d1ca7)

Se le instala SQL Server 2022
![image](https://github.com/user-attachments/assets/85f9c3b8-f86b-4ff8-ace6-9ec76cf00847)

Se le instala Sharepoint Server 2019
![image](https://github.com/user-attachments/assets/59a3d167-93b1-4b23-98ee-37c6695c0bda)

Para hacer una Instalación Funcional debemos de crear un Usuario en ADDS para poder usarlo en la conexión de SharePoint con la Base de Datos SQL. Por lo tanto iniciamos la instalación de ADDS en el Server Manager.
![image](https://github.com/user-attachments/assets/5b029041-df2f-4500-91f9-437499e1418a)
![image](https://github.com/user-attachments/assets/7859171a-7180-4521-8486-5a0dfebeae89)

Instalación de ADDS completa
![image](https://github.com/user-attachments/assets/3a5cc917-570c-4f0d-adee-9fae73e59283)

Una vez instalado el ADDS tenemos que promover el servidor y además realizar una configuración para que todo quede funcional, para eso vamos al Server Manager a la esquina superior derecha a buscar la bandera con un triangulo amarillo y procedemos a darle “Promover este Servidor”
![image](https://github.com/user-attachments/assets/18c8645a-9d5f-4cfe-8a76-f74b775ea6e1)

Una vez se inicia el asistente le damos “crear un nuevo bosque” y seguidamente lo nombramos como deseemos en mi caso “proyecto.local”
![image](https://github.com/user-attachments/assets/34cbfff6-e1b5-444c-a7ad-9e9b8800c9e4)

En el siguiente paso solo creamos una contraseña segura
![image](https://github.com/user-attachments/assets/eaa7afd1-e34d-4fc7-a913-05dc9464aa99)

Le damos “Next”
![image](https://github.com/user-attachments/assets/9c2d3ec3-56cb-4154-851d-7a2a0bfb55d0)

En la siguiente ventana el mismo nos crea el NetBIOS Domain Name y le damos “Next”
![image](https://github.com/user-attachments/assets/15788fa1-578d-4ed6-9642-7caa83677c86)

Le damos “Next” en ambas ventanas
![image](https://github.com/user-attachments/assets/9b3565fd-4c2c-4d47-99a1-33149127a4ba)
![image](https://github.com/user-attachments/assets/e60d8add-deae-4895-a3bd-f13546425cff)
Seguidamente le damos “Install” en la siguiente ventana y luego el servidor se reiniciará automáticamente

Una vez que se esta en el Instalador de Sharepoint Server 2019, primero se utiliza la opción splash y al abrirse la ventana flotante usamos la opción “Install Software Prerequisites”
![image](https://github.com/user-attachments/assets/c93906ec-71f6-4d2e-8ec0-ddae5ccdfdc7)

Seguidamente se Completa la Instalación de los Prerequisites
![image](https://github.com/user-attachments/assets/62448747-e43f-4c95-803d-7af462e350c7)

Una vez mas accesamos a splash y cuando estamos en la ventana flotante le damos “Install Sharepoint Server”
![image](https://github.com/user-attachments/assets/0ee27d72-111d-44de-95e6-61883be1733e)

Buscamos el Enterprise Product Key en Internet
![image](https://github.com/user-attachments/assets/4f93931d-751a-444b-ac24-331f4f118d2a)

Le damos Install Now
![image](https://github.com/user-attachments/assets/8518909b-b0f3-42c7-9019-9bd13ad2b255)

Finaliza la Instalación y se Reinicia la Maquina
![image](https://github.com/user-attachments/assets/4e727f48-4a6e-4ed2-93f0-71ded6786eb8)

Se abre el Executable para continuar con la Instalación de SharePoint
![image](https://github.com/user-attachments/assets/cd76a0cf-606b-429d-b6a8-3a6a3b074b01)

Crear una nueva granja de servidores
![image](https://github.com/user-attachments/assets/97faf46e-4aba-4d39-beaf-24275e23dded)

Luego de eso agregamos el Servidor de la Base de Datos y aparte ponemos el usuario creado con el ADDS y su respectiva contraseña
![image](https://github.com/user-attachments/assets/91475005-d992-4368-82a2-c0d107127795)

Creamos otra contraseña para la granja
![image](https://github.com/user-attachments/assets/7123c93f-190c-41c2-98f0-4dc0f5541e1b)

Seguidamente seleccionamos Single-Server Farm
![image](https://github.com/user-attachments/assets/9209855a-2d0f-4547-8834-f271dd0198ee)

(Opcional) Podemos elegir un numero de puesto especifico o podemos dejar el predeterminado, en mi caso utilice el 30000
![image](https://github.com/user-attachments/assets/3e14b890-3971-4ae7-acee-44a7f880b48d)

Revisamos la configuración
![image](https://github.com/user-attachments/assets/9e11177b-665f-4658-a9e1-b62adf23531e)

La instalación se empieza a ejecutar automáticamente
![image](https://github.com/user-attachments/assets/0ba52825-ce69-4d5c-9c3c-19e0153e6a27)

Finaliza la instalación
![image](https://github.com/user-attachments/assets/7f4084ca-3c9f-4090-a400-7c9ba59304d0)

Listo ahora si tenemos nuestro SharePoint y procedemos a darle "Start Wizard"
![image](https://github.com/user-attachments/assets/2708091a-140b-41b9-9853-a9098ca103e2)

Luego seleccionamos nuestra propia cuenta ya creada y dejamos las opciones de la parte inferior a como vienen por predeterminado
![image](https://github.com/user-attachments/assets/e48ff189-b3bd-478c-8a6b-ecd871b8a047)




































