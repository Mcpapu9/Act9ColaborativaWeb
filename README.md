# Vía Segura — Prototipo Front-End Navegable

Prototipo navegable de interfaz web desarrollado con HTML5 y CSS3 para el proyecto *Vía Segura*, enfocado en la prevención y reporte de incidentes comunitarios en León, Guanajuato.

---

## 1. Integrantes y Roles (Sección 4)

| Integrante | Rol | Responsabilidades |
| :--- | :--- | :--- |
| *Luis Ariel Granados Campos* | Lead Dev & DevOps | Configuración inicial del repositorio Git, estructura base, CSS modular y maquetado de vistas de acceso (index.html, registro.html). |
| *Javier Alejandro Sálazar Mártinez* | Front-End Developer | Maquetado de vistas internas, desarrollo de formularios y flujo de confirmación (inicio.html, reportar.html, confirmacion.html). |
| *Jesús Alberto Cortés García* | QA & Documentation | Documentación del proyecto, trazabilidad de requerimientos, auditoría de calidad de interfaz y manual de navegación. |

---

## 2. Trazabilidad: Requerimientos ----> Vistas Web

| ID Requerimiento | Descripción del Requerimiento (Act. 3) | Vista Web Implementada | Archivo HTML |
| :---: | :--- | :--- | :--- |
| *RF-01* | Inicio de sesión de usuarios registrados | Pantalla de Login | index.html |
| *RF-02* | Registro de nuevos usuarios en la plataforma | Pantalla de Registro | registro.html |
| *RF-03* | Panel principal y menú de opciones de seguridad | Dashboard / Inicio | inicio.html |
| *RF-04* | Formulario para reportar incidentes con datos clave | Formulario de Reporte | reportar.html |
| *RF-05* | Confirmación y generación de folio de reporte | Resumen de Confirmación | confirmacion.html |

---

## 3. Mapa de Navegación

El prototipo sigue una estructura navegable fluida sin dependencia de servidor backend:

```text
[ index.html ] (Login)  <--->  [ registro.html ] (Registro)
      |
      v
[ inicio.html ] (Dashboard principal)
      |
      +---> [ reportar.html ] (Formulario de reporte)
                  |
                  v
            [ confirmacion.html ] (Folio generado)
                  |
                  +---> Regresar a [ inicio.html ]
