Minicore – Aplicación de Comisiones de Ventas
Descripción

Minicore es una aplicación web desarrollada con Flask y SQLAlchemy que permite calcular comisiones de ventas por usuario en un rango de fechas determinado.

La aplicación incluye:

Registro de usuarios y ventas (datos de prueba preconfigurados).

Cálculo de comisiones según tramos de ventas.

Interfaz web con formularios para filtrar ventas por fecha.

Generación dinámica de resultados con resumen de ventas y comisiones.

Esta aplicación está preparada para ser desplegada en servicios de backend dinámico, como Render, y no es compatible con plataformas de hosting estático como Netlify.

Tecnologías utilizadas

Python 3.11+

Flask (Framework web)

Flask-SQLAlchemy (ORM para base de datos)

SQLite (base de datos por defecto, configurable con DATABASE_URL)

Gunicorn (servidor WSGI para producción)

HTML, CSS (templates en Jinja2)

Instalación local

Clonar el repositorio:

git clone <URL_DEL_REPOSITORIO>
cd minicore


Crear un entorno virtual:

python -m venv venv
source venv/bin/activate   # Linux/macOS
venv\Scripts\activate      # Windows


Instalar dependencias:

pip install -r requirements.txt


Ejecutar la aplicación localmente:

python app.py


Abrir en el navegador:

http://127.0.0.1:5000/

Uso

Acceder a la página principal / para seleccionar un rango de fechas.

Ingresar fecha de inicio y fecha de fin en formato YYYY-MM-DD.

Enviar el formulario para ver el resumen de ventas y comisiones por usuario.

Configuración para despliegue en Render

Crear archivo Procfile en la raíz del proyecto:

web: gunicorn app:app --bind 0.0.0.0:$PORT


Asegurarse de tener requirements.txt actualizado:

Flask
Flask-SQLAlchemy
SQLAlchemy
gunicorn


Opciones de despliegue en Render:

Tipo de servicio: Servicio Web

Publish Directory: ./

Start Command: gunicorn app:app --bind 0.0.0.0:$PORT

Estructura del proyecto
/minicore
│
├─ app.py                # Archivo principal Flask
├─ requirements.txt      # Dependencias
├─ Procfile              # Comando para Render
├─ templates/            # Archivos HTML
│    ├─ formulario_busqueda.html
│    └─ comision.html
└─ static/               # CSS, JS, imágenes

Enlaces
Enlace al video explicativo:https://youtu.be/uU2WKMIOAJQ

Enlace de despliegue: https://minicoree-5.onrender.com

Enlace al repositorio:https://github.com/EnzoCortez/MIniCoreE.git

Autor 
Enzo Cortez

Render requiere que la app escuche en 0.0.0.0 y en el puerto definido por la variable $PORT.

No es compatible con Netlify directamente porque Flask requiere un backend dinámico.
