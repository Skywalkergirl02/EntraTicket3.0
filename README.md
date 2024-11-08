# EntraTicket 3.0

## Descripción

**EntraTicket 3.0** es un sistema de gestión de entradas para shows y eventos. El sistema permite a los usuarios visualizar eventos disponibles, seleccionar localidades, comprar entradas y generar un código QR para el acceso al evento. Está diseñado para ser utilizado tanto en dispositivos móviles como en escritorio, ofreciendo una experiencia de usuario sencilla y eficiente. 

Este proyecto es una aplicación web desarrollada en **ASP.NET Core** con acceso a base de datos utilizando **ADO.NET**. El sistema está preparado para integrarse con métodos de autenticación JWT y cuenta con diversas funcionalidades, tales como la generación de códigos QR para las entradas y la autenticación de usuarios.

## Características Principales

- **Visualización de eventos**: Los usuarios pueden explorar los eventos disponibles y ver detalles como la fecha, hora y lugar.
- **Selección de localidades**: Permite elegir entre diferentes tipos de localidades para cada evento.
- **Compra de entradas**: Los usuarios pueden comprar entradas a través de una interfaz amigable.
- **Generación de códigos QR**: Después de una compra exitosa, se genera un código QR que será utilizado para acceder al evento.
- **Autenticación JWT**: Utiliza **JSON Web Tokens (JWT)** para la autenticación segura de usuarios.
- **Gestión de métodos de pago**: El sistema permite gestionar los métodos de pago para realizar compras.

## Tecnologías Utilizadas

- **ASP.NET Core 8**: Framework principal para el desarrollo de la aplicación.
- **ADO.NET**: Mecanismo para el acceso a datos desde una base de datos SQL Server.
- **SQL Server**: Base de datos relacional utilizada para almacenar los eventos, usuarios y transacciones.
- **QRCoder**: Librería para la generación de códigos QR al completar una compra.
- **JWT (JSON Web Tokens)**: Para la autenticación segura de usuarios.
- **Swagger**: Documentación de API para pruebas y desarrollo.

## Requisitos

### Herramientas Necesarias

- .NET 8 SDK
- SQL Server (local o en la nube)
- Visual Studio o Visual Studio Code


### Configuración de la Base de Datos

El sistema utiliza una base de datos SQL Server. Antes de correr el proyecto, asegurate de que tu base de datos esté configurada y que las cadenas de conexión en el archivo `appsettings.json` apunten a la base de datos correcta.

```json
{
  "ConnectionStrings": {
    "DefaultConnection": "Server=your-server;Database=EntraTicketDB;User Id=your-username;Password=your-password;"
  }
}
