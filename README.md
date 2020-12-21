# 20487D_MOD01_LAK_BlueYonder.Flights
# Module 1: Overview of Service and Cloud Technologies
# Lab: Exploring the Work Environment

JOSE VICENTE TEJERO - 20/12/2020

RESUMEN
Creating an ASP.NET Core Project

Creating a Simple Entity Framework Model
Create a new POCO entity
Create a new DbContext class

Creating a Web API Class
reate a new class for the web API
Create an action and use the Entity Framework context

Deploying the Web Application to Azure
Create an Azure Web App and an SQL database
Deploy the web application to the Azure Web App
Test the web API

PROBLEMAS
En el ejercicio 4, task 3, no he podido insertar un registro en la BD con el comando:

$postParams = "{'origin': 'Germany',
    'destination': 'France',
    'flightNumber': 'GF7625',
    'departureTime': '0001-01-01T00:00:00'}"
Invoke-WebRequest -Uri http://flightsmod1labjvtc.azurewebsites.net/api/flights -ContentType "application/json" -Method POST -Body $postParams


Como dice el enunciado, he introducido: [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12

Y tampoco funciona. Damos de alta los registros en la BD.
Por lo demás, todo bien, se llega a la base de datos desde el browser pero no muestra registros.

20487D_MOD01_LAK

\# Module 1: Overview of Service and Cloud Technologies

\# Lab: Exploring the Work Environment

**Exercise 1: Creating an ASP.NET Core Project**

**Task 1: Create a new ASP.NET Core project**

 

 

![img](clip_image002.png)

### Exercise 2: Creating a Simple Entity Framework Model

#### Task 1: Create a new POCO entity

 

 

![img](clip_image004.png)

 

 

 

 

 

![img](clip_image006.png)

 

 

### Exercise 4: Deploying the Web Application to Azure

#### Task 1: Create an Azure Web App and an SQL database

![img](clip_image008.png)

![img](clip_image010.png)

 

![img](clip_image012.png)

 

Task 2: Deploy the web application to the Azure Web App

 

![img](clip_image014.png)

 

![img](clip_image016.png)

 

Al ejecutar:

$postParams = "{'origin': 'Germany',

  'destination': 'France',

  'flightNumber': 'GF7625',

  'departureTime': '0001-01-01T00:00:00'}"

Invoke-WebRequest -Uri http://flightsmod1labjvtc.azurewebsites.net/api/flights -ContentType "application/json" -Method POST -Body $postParams

![img](clip_image018.png)

 

![img](clip_image020.png)

![img](clip_image022.png)

Como el comando Invoque no funciona, añadimos los registros directamente en la base de datos.

![img](clip_image024.png)

Comprobamos que funciona correctamente.

![img](clip_image026.png)

 

![img](clip_image028.png)

 

