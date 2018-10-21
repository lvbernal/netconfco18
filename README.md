# AWS Lambda y .NET Core.

Instrucciones para el workshop "Desarrollo de funciones AWS Lambda con .NET Core", presentado en la [.NET Conf CO v2018](http://co.netconf.global/es), entre el 8 y el 10 de noviembre de 2018.

__Speakers__:
* Manuel Zapata
    * [@ManuelZapata](http://twitter.com/manuelzapata)
    * http://manuelzapata.co
* Leonardo Vargas
    * [@lvbernal](http://twitter.com/lvbernal)
    * http://lvbernal.com

__Requisitos__:
* [Visual Studio 2017](https://visualstudio.microsoft.com/downloads)
* [AWS Toolkit for Visual Studio 2017](https://marketplace.visualstudio.com/items?itemName=AmazonWebServices.AWSToolkitforVisualStudio2017)
* [Cuenta de Amazon Web Services](https://aws.amazon.com/)

# Introducción

En la primera parte del workshop aprenderá a crear y desplegar una función lambda desarrollada con .NET Core. Y en la segunda aprenderá a crear otra lambda que recibe el resultado de la primera desde una cola o _queue_ y lo envía a un servicio externo.

# Primera parte

Cree una lambda que cuente las palabras de una cadena de texto. Utilice [Postman](https://www.getpostman.com/), [Insomnia](https://insomnia.rest/) u otro cliente REST para consumir la función.

# Segunda parte

Cree una cola de AWS y modifique la primer lambda para que envíe los resultados hacia esa cola. Luego cree una segunda lambda que lea la cola y envíe el resultado a un canal de Slack.