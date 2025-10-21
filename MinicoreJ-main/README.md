Proyecto Comisiones

Autor: Enzo Cortez

Descripción

Este proyecto permite consultar y visualizar comisiones de ventas dentro de un rango de fechas definido por el usuario. Está desarrollado con Python Flask para el backend y HTML + Bootstrap 4 para el frontend, garantizando una interfaz amigable y responsiva.

El proyecto consta de dos vistas principales:

Formulario de búsqueda de comisiones: Permite ingresar fecha de inicio y fin para filtrar los registros.

Reporte de comisiones: Muestra en una tabla el nombre del vendedor, el total de ventas y la comisión correspondiente.

Tecnologías utilizadas

Python 3.x

Flask

HTML5 / CSS3

Bootstrap 4

Jinja2 (para renderizar las plantillas HTML con datos dinámicos)

Funcionamiento

Abrir la aplicación en el navegador.

En la página principal, ingresar el rango de fechas deseado.

Presionar el botón Buscar.

La aplicación mostrará una tabla con los resultados:

Nombre completo del vendedor

Total de ventas en el rango seleccionado

Comisión calculada

Estructura del proyecto
project-root/
│
├── templates/
│   ├── buscar_comisiones.html
│   └── reporte_comisiones.html
│
├── static/
│   └── (archivos CSS o JS opcionales)
│
├── app.py (archivo principal de Flask)
└── README.md

Despliegue

Enlace a la aplicación desplegada: [Agregar enlace aquí]

Video explicativo del funcionamiento: [Agregar enlace aquí]

Repositorio GitHub: [Agregar enlace aquí]

Instrucciones para ejecutar localmente

Clonar el repositorio:

git clone [Agregar enlace aquí]


Instalar dependencias:

pip install -r requirements.txt


Ejecutar la aplicación:

python app.py


Abrir el navegador y acceder a http://127.0.0.1:5000/

Autor

Enzo Cortez
