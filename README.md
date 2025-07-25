

Este proyecto incluye un backend desarrollado en Python para la gestión de una base de datos relacional y un frontend en ReactJS.



## 📦 Backend

El backend de este proyecto está construido con **Python** y utiliza **FastAPI** para exponer servicios web.

### 🔧 Requisitos

Antes de ejecutar el backend, asegúrate de tener **Python 3.13** instalado y docker desktop.


### ⚙️ Configuración

Debes crear un archivo `.env` dentro del directorio `Back-End` con la siguiente información de conexión a tu base de datos:

```env
DB_HOST=mysql
DB_PORT=3306
DB_NAME=MarloyCoffee
DB_USER=admin
DB_PASS=admin123
MYSQL_ROOT_PASSWORD=admin123
MYSQL_DATABASE=MarloyCoffee
MYSQL_USER=admin
MYSQL_PASSWORD=admin123
```

Modifica los valores según tu configuración local.

### 🚀 Ejecución

Para ejecutar el servidor del backend, navega al directorio del backend y corre el siguiente comando:

docker compose up 

para construir tu contenedor de docker que conendra la api y el backend, luego estando en la carpeta de frontend ejecutamos el comando npm run dev para ver la pagina web

### 📡 Rutas de la API

Todas las rutas de la API estarán disponibles bajo el prefijo:

```
/api/ruta
```

Por ejemplo:  
http://localhost:8082/api/clientes
---

## 🧠 Nota

Asegúrate de tener corriendo tu servidor de base de datos y de que los datos del `.env` coincidan con tu configuración para evitar errores de conexión.
