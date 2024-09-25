## Pasos para redireccionar en paginas PHP

#1. Creamos un archivo php con la estructura de un html, seguido escribimos <a> y inyectamos dentro el href seguido de un = con la direccion a la que haremos la unión:

ejemplo:
<a href="ejemplo.php?name=alex">ejemplo</a>

#2. Creamos un archivo llamado ejemplo.php donde podremos mostrar los datos que receivimos por medio del get al hacer print_r($_GET) y para redirigir a otras paginamos podemos poner header("location: ejemplo2.php") y para mandar el parametro header("location: ejemplo.php?name=".$_GET['name'];

#3. Por ultimo creamos el archivo ejemplo2.php para mostrar los datos recividos con el print del paso anterior
