# SIWEBA — Documentación del proyecto

## 1. Información General del Proyecto

### Nombre del proyecto
Diseño e implementación de un sistema web para el monitoreo de estaciones meteorológicas basadas en Arduino.

### Breve descripción
La solución consiste en el desarrollo de una plataforma web que permite integrar estaciones meteorológicas de usuarios e instituciones en una red colaborativa. En esta plataforma, los datos generados (temperatura, humedad, presión atmosférica, etc.) pueden ser compartidos y consultados de manera accesible y en tiempo real. El sistema se compone de dos subsistemas interconectados: una estación meteorológica de hardware basada en Arduino y una plataforma web de software desarrollada en Django para almacenar, validar y visualizar los datos.

### Objetivo general
Crear una estación meteorológica funcional con Arduino y una plataforma web para almacenar y consultar libremente los datos que esta recolecta.

### Estado actual
En desarrollo de una primera versión funcional que corresponderá a un prototipo mínimo viable, el cual estará enfocado en la recolección, almacenamiento, visualización y consulta de datos meteorológicos.

### Versión o Sprint actual
Sprint II: seguimiento, evaluación y adaptación.

---

## 2. Equipo de Trabajo

- **Mentor:** Mtro. Juan José López Cisneros.
- **Project Leader:** Primitivo Oyoque Vargas
- **Integrantes del equipo:**
    - Casandra Jazmín Rodríguez Flores 
    - Primitivo Oyoque Vargas

---

## 3. Estructura del Proyecto

### Repositorios del proyecto

La documentación de este repositorio corresponde al proyecto SIWEBA en conjunto, que se organiza en tres repositorios independientes:

- [documentacion](https://github.com/SIWEBA/documentacion): documentación general, de gestión y de los sprints.
- [django-backend](https://github.com/SIWEBA/django-backend): API, lógica del servidor y documentación técnica del backend.
- [django-frontend](https://github.com/SIWEBA/django-frontend): aplicación web y panel de visualización.

Al clonar los tres repositorios dentro de una misma carpeta de trabajo, la estructura general es:

```text
SIWEBA/
├── django-backend/      # API y lógica del servidor desarrolladas con Django
│   ├── config/          # Configuración general, rutas y despliegue de Django
│   ├── estaciones/      # Aplicación para gestionar estaciones meteorológicas
│   ├── usuarios/        # Aplicación para gestionar usuarios
│   └── docs/            # Documentación técnica del backend
├── django-frontend/     # Aplicación web desarrollada con Django
│   ├── config/          # Configuración general y rutas del frontend
│   └── dashboard/       # Vistas, modelos, migraciones y plantillas del panel
└── documentacion/       # Documentación general, técnica y de gestión del proyecto
    ├── capitulos/       # Capítulos de la documentación
    ├── design-baseline/ # Referencias y recursos del diseño, incluidos modelos 3D
    ├── docs/            # Documentación técnica
    ├── evidence/        # Evidencias del proyecto
    ├── project-management/ # Acta, roles, riesgos, cronograma y desglose del trabajo
    ├── sprints/         # Documentación organizada por sprint
    └── src/             # Recursos de la documentación, como logotipos
```

En ambos proyectos Django, `manage.py` permite ejecutar tareas administrativas y las carpetas `migrations/` de sus aplicaciones contienen los cambios versionados del esquema de datos. El backend y el frontend se mantienen en repositorios independientes.

---

## 4. Instrucciones para consultar o reproducir el proyecto

Este repositorio reúne la documentación del proyecto completo. Para consultar el código, visita los repositorios de backend y frontend indicados arriba o la [organización SIWEBA en GitHub](https://github.com/orgs/SIWEBA/repositories).

Para consultar la documentación en PDF:
1. Asegúrate de tener LuaLaTeX instalado en tu sistema.
2. Abre una terminal y navega hasta el directorio de esta documentación.
3. Ejecuta el comando `lualatex main.tex` para compilar el documento.
4. Abre el archivo PDF generado para visualizar la documentación.