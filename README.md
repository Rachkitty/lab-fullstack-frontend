# Laboratorio Integral: Arquitectura Fullstack (Node.js + Consumo Dual)

Este proyecto es una práctica de laboratorio completa para la asignatura de Programación FrontEnd / Desarrollo Web Avanzado. Consiste en la construcción de una API REST CRUD en Node.js y Express, la cual es consumida de forma simultánea por dos clientes frontend independientes (Cliente imperativo vs. Cliente reactivo).

---

## Arquitectura del Proyecto

El espacio de trabajo está diseñado bajo el principio de desacoplamiento cliente-servidor, donde ambos frontends consumen de forma unificada los mismos endpoints HTTP en `http://localhost:3000/api/tareas`.

```text
lab-fullstack-frontend/
├── backend-api/          # Servidor Node.js + Express (Puerto 3000)
├── frontend-bootstrap/   # Cliente 1: HTML5 + Bootstrap 5 + Vanilla JS (Live Server)
└── frontend-react/       # Cliente 2: SPA React 18+ + Vite + Bootstrap (Puerto 5173)
