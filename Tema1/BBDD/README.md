
Función UPDATE:
```function updateUser($id, $nuevoNombre) {
    $conn = dbConnect();
    $update = "UPDATE users SET nombre = ? WHERE id = ?";
    $stmt = $conn->prepare($update);
    $stmt->bind_param("si", $nuevoNombre, $id);
    $stmt->execute()
```
Podemos comprobar que ha funcionado revisandolo desde la base de datos, ahora en vez de Alex, hay un usuario llamado Luca.
<img src="1.png">

Función DELETE:

 ```function deleteUser($id) {
    $conn = dbConnect();
    $delete = "DELETE FROM users WHERE id = ?";
    $stmt = $conn->prepare($delete);
    $stmt->bind_param("i", $id);
    $stmt->execute()```
