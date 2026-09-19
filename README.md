# Home & About

Proyecto web desarrollado con Django para crear una pequeña landing page o sitio personal con dos secciones principales: inicio y acerca de. El objetivo del proyecto es ofrecer una base sólida para una presentación profesional, con una estructura simple, mantenible y fácil de ampliar.

## Descripción general

Este trabajo consiste en la construcción de un sitio web básico con un diseño minimalista y una organización modular propia de Django. La aplicación incluye:

- Página principal con contenido de bienvenida
- Página de información personal o institucional
- Plantilla base reutilizable para mantener una estructura visual consistente
- Rutas organizadas por app para una mejor escalabilidad

La arquitectura del proyecto está diseñada para crecer en futuras etapas, permitiendo agregar nuevas páginas, secciones, estilos y contenido sin romper la base actual.

## Objetivos del proyecto

- Construir una base funcional para un sitio personal o profesional
- Aprender y aplicar patrones de Django para la creación de vistas y rutas
- Implementar templates reutilizables mediante herencia
- Organizar el proyecto de forma ordenada y profesional

## Tecnologías utilizadas

- Python
- Django
- SQLite3
- HTML
- Jinja/Django Templates

## Estructura del proyecto

```text
home-about/
├── djago_base/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
│   └── asgi.py
├── pages/
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── tests.py
│   ├── urls.py
│   ├── views.py
│   └── migrations/
├── templates/
│   ├── _base.html
│   ├── home.html
│   └── about.html
├── db.sqlite3
├── manage.py
├── requirements.txt
└── README.md
```

## Funcionalidades implementadas

### Página de inicio
Se define una vista basada en `TemplateView` para renderizar la página principal.

### Página de acerca de
Se crea una segunda vista que permite mostrar contenido adicional sobre la persona, empresa o proyecto.

### Arquitectura de rutas
El proyecto separa la definición de URLs en la app `pages`, y luego incluye esas rutas en la configuración principal de Django.

### Plantilla base
Se utiliza una plantilla base en `templates/_base.html` para mantener una estructura común para todas las páginas, facilitando la reutilización y una apariencia uniforme.

## Configuración del entorno

### Requisitos

- Python 3.10 o superior
- pip
- Virtual environment recomendado

### Instalación

1. Clona el repositorio.
2. Navega al directorio del proyecto.
3. Crea un entorno virtual:

```bash
python -m venv venv
```

4. Activa el entorno virtual:

- Windows:

```bash
venv\Scripts\activate
```

- macOS/Linux:

```bash
source venv/bin/activate
```

5. Instala las dependencias:

```bash
pip install -r requirements.txt
```

## Ejecución del proyecto

Desde la raíz del proyecto, ejecuta:

```bash
python manage.py runserver
```

Luego abre en el navegador:

- http://127.0.0.1:8000/
- http://127.0.0.1:8000/about/

## Rutas principales

| Ruta | Descripción |
|------|-------------|
| `/` | Página principal |
| `/about/` | Sección de información general |
| `/admin/` | Panel administrativo de Django |

## Estado del proyecto

Este es un proyecto en etapa inicial pero con una base funcional y bien organizada para continuar desarrollando una web personal o comercial. La estructura actual permite avanzar fácilmente con nuevas vistas, contenido dinámico y un diseño más profesional.

## Siguiente evolución recomendada

- Agregar estilos personalizados con CSS
- Incorporar diseño responsivo
- Añadir más secciones como servicios, portafolio, contacto o blog
- Integrar contenido dinámico desde bases de datos
- Mejorar la experiencia visual con componentes y layout más elaborados

## Nota

Este README refleja el estado actual del proyecto y su enfoque inicial de desarrollo con Django. La intención es servir como base documental para futuras mejoras y expansión del sitio.
