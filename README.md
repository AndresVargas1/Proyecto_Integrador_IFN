# 🌱 Inventario Forestal Nacional (IFN) – Proyecto Integrador

![React](https://img.shields.io/badge/Frontend-React-blue)
![Django|DFR](https://img.shields.io/badge/Backend-Django|DFR-green)
![Postgres](https://img.shields.io/badge/DB-Postgres-blueviolet)
![MongoDB](https://img.shields.io/badge/DB-MongoDB-brightgreen)
![Vercel](https://img.shields.io/badge/Deploy-Vercel-black)
![Render](https://img.shields.io/badge/Deploy-Render-lightgrey)

Desarrollo de software para el Inventario Forestal Nacional (IFN) en Colombia.  
Proyecto integrador de Ingeniería de Sistemas (semestre V – 2025).  
El software digitaliza los formularios de campo y apoya la gestión forestal, garantizando **calidad, seguridad y trazabilidad de los datos**.

---

## 🎯 Objetivos
- Registrar datos de especies vegetales en campo.
- Validar información con reglas de negocio.
- Gestionar usuarios, roles y sesiones con auditoría (Logs).
- Generar reportes e indicadores.

---

## 🏗️ Arquitectura
El sistema se organiza en cuatro componentes principales:

1. **Frontend (React – Vercel)**  
   Interfaz web para captura y consulta de datos.

2. **Orquestador (Django + DRF – Render)**  
   Punto único de entrada que valida JWT y enruta solicitudes.

3. **Servicio 1: Autenticación, Roles y Logs (Django + MongoDB Atlas)**  
   Manejo de usuarios, sesiones, permisos y trazabilidad.

4. **Servicio 2: Lógica de Negocio IFN (Django + Postgres/Neon)**  
   Gestión de formularios del inventario forestal y generación de indicadores.

---

## 🗄️ Bases de Datos
- **Postgres (Neon)** → Datos estructurados del inventario.  
- **MongoDB Atlas** → Usuarios, roles, sesiones y logs.

---

## 🚀 Despliegue
- **Frontend** → Vercel.  
- **Backends** → Render.  
- **Bases de datos** → Neon (Postgres) y MongoDB Atlas (Mongo).

---

## 📂 Organización del Repositorio
```bash
/frontend         # React (interfaz web)
/orchestrator     # Django DRF (API)
/service-auth     # Django DRF + Mongo (usuarios, roles, logs)
/service-core     # Django DRF + Postgres (lógica de negocio IFN)
```
---

## 👥 Equipo de Desarrollo

- Andrés Felipe Vargas Amaya – Estudiante
- Silvia Nathalia Hernandez Sandoval – Estudiante
