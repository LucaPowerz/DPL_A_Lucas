# Guía para crear un sitio web en InfinityFree

Guía paso a paso para crear un sitio web en InfinityFree, cargar archivos con FileZilla y configurar una base de datos.

## Requisitos necesarios

- Contar con una dirección de correo válida.
- Tener instalado el programa FileZilla.
- Tener acceso a un navegador web.

## Crear una cuenta en InfinityFree

1. Visita la página de [InfinityFree](https://www.infinityfree.net/).
2. Haz clic en “Sign Up” o “Register” para crear tu cuenta.
3. Llena el formulario de registro con tu correo y una contraseña.
4. Confirma tu cuenta mediante el correo de verificación.
5. Ingresa a tu cuenta de InfinityFree.

## Crear un sitio web

1. En el panel de InfinityFree, selecciona “Create Account” o “New Account”.
2. Elige entre un dominio gratuito de InfinityFree o usa un dominio propio.
3. Completa la configuración del sitio.
4. Guarda la información de acceso FTP (servidor, usuario y contraseña) que te proporcionan en el panel.

## Configurar FileZilla

1. Abre FileZilla y selecciona `Archivo` -> `Gestor de sitios` o usa `Ctrl + S`.
2. Haz clic en "Nuevo sitio", y nómbralo (por ejemplo, "InfinityFree").
3. Completa la configuración con los datos FTP proporcionados:
   - **Host**: el servidor FTP de InfinityFree.
   - **Puerto**: 21
   - **Protocolo**: FTP
   - **Cifrado**: FTP explícito sobre TLS si está disponible.
   - **Método de acceso**: Normal.
   - **Usuario** y **Contraseña**: Datos de tu cuenta FTP.
4. Haz clic en “Conectar”.

## Subir archivos al servidor

1. Al conectar con tu servidor FTP en FileZilla, verás dos secciones: a la izquierda, tus archivos locales; a la derecha, los del servidor.
2. Dirígete a la carpeta donde tienes los archivos de tu sitio.
3. Arrastra los archivos desde el panel izquierdo al derecho para subirlos.

## Crear una base de datos en InfinityFree

1. En el panel de InfinityFree, busca “MySQL Databases”.
2. Crea una base de datos con:
   - Nombre para la base de datos.
   - Usuario y contraseña para la base de datos.
3. Guarda la información de la base de datos (nombre, usuario, contraseña y servidor MySQL).

## Conectar la aplicación a la base de datos

1. En tu proyecto, abre el archivo de configuración de conexión a la base de datos.
2. Completa los datos de conexión:
   - **Servidor**: servidor MySQL proporcionado (`sqlXXX.epizy.com`).
   - **Usuario**: Usuario de la base de datos.
   - **Contraseña**: Contraseña de la base de datos.
   - **Nombre de la base de datos**: Nombre asignado a la base.
3. Guarda los cambios.

## Probar el sitio

1. En el navegador, ingresa la URL de tu dominio (por ejemplo, `http://tudominio.epizy.com`).
2. Revisa que todo funcione correctamente, incluyendo la conexión a la base de datos.
