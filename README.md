# 🔗 API REST Productos - Spring Boot

## 📖 Descripción

Aplicación desarrollada con **Spring Boot** que implementa una **API REST CRUD** para la gestión de productos.
La API utiliza `@RestController` y `ResponseEntity` para manejar solicitudes HTTP y devolver respuestas en formato **JSON** con los códigos de estado correctos.

---

## ⚙️ Tecnologías

* Java 17
* Spring Boot 3
* Spring Web
* Maven

---

## 🏗️ Estructura

```text
apiproductos/
 ├── controller/
 ├── service/
 ├── model/
 └── ApiProductosApplication.java
```

---

## 🚀 Ejecución

```bash
mvn clean install
mvn spring-boot:run
```

Abrir:

```text
http://localhost:8080/api/productos
```

---

## 🧪 Endpoints

| Método | URL                 | Descripción         | Código      |
| ------ | ------------------- | ------------------- | ----------- |
| GET    | /api/productos      | Listar productos    | 200 OK      |
| GET    | /api/productos/{id} | Obtener por ID      | 200 / 404   |
| POST   | /api/productos      | Crear producto      | 201 Created |
| PUT    | /api/productos/{id} | Actualizar producto | 200 / 404   |
| DELETE | /api/productos/{id} | Eliminar producto   | 204 / 404   |

---

## 📌 Ejemplo JSON

```json
{
  "nombre": "Laptop",
  "descripcion": "16GB RAM",
  "precio": 2500
}
```

---

## ✔ Validación

La API cumple con:

* CRUD completo funcional
* Uso correcto de métodos HTTP
* Respuestas en JSON
* Manejo de códigos HTTP (200, 201, 204, 404)
* Manejo global de errores

---

## 📸 Pruebas


Se validó usando Postman:

* GET → lista de productos<img width="1628" height="1008" alt="image" src="https://github.com/user-attachments/assets/c93b4324-973c-4d88-bce6-b36db8cc1b25" />
<img width="812" height="739" alt="image" src="https://github.com/user-attachments/assets/df6845a2-d77a-4df9-9fc6-d06c6ef170d1" />
* POST → creación<img width="1239" height="881" alt="image" src="https://github.com/user-attachments/assets/d3235c7c-7f55-4a0d-a381-c38b8020127c" />

* PUT → actualización<img width="1567" height="975" alt="image" src="https://github.com/user-attachments/assets/8ecf1abe-dc41-4c42-ada6-ec8c3164d8d0" />

* DELETE → eliminación

