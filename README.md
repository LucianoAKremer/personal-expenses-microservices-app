 📱💡 Personal Expenses Platform: App + Microservicios

Plataforma completa para la gestión y análisis de gastos personales, integrando una app móvil Android (Kotlin) con un backend robusto basado en microservicios (FastAPI, Node.js, PostgreSQL, Docker).

---

## 🧩 Arquitectura General
- **App Android:** Registro y visualización de gastos, balances y reportes, desarrollada en Kotlin con Jetpack Compose.
- **Backend Microservicios:** Autenticación, CRUD de gastos/categorías, análisis avanzado y generación de gráficos, todo orquestado con Docker Compose.

---

## 📱 App Móvil (Kotlin)
- Jetpack Compose para UI moderna y reactiva
- Room/SQLite para persistencia local
- Retrofit para integración con APIs REST
- Registro y edición de gastos/ingresos
- Visualización de balances y reportes
- (Integrado) Sincronización y autenticación con backend propio

---

## ⚙️ Backend Microservicios
- **auth-service:** Registro, login y validación JWT
- **data-service:** CRUD de gastos y categorías, validación de usuario
- **analytics-service:** Estadísticas, análisis y templates de gráficos
- **gateway:** API Gateway para unificar rutas y seguridad
- **db:** PostgreSQL con scripts de inicialización

---

## 🔗 Integración App + Backend
- La app consume los microservicios vía API REST (gateway)
- Autenticación de usuario y obtención de JWT desde la app
- Sincronización de gastos/categorías entre app y backend
- Visualización de estadísticas y gráficos generados por analytics-service

---

## 🚀 Tecnologías
- Kotlin, Jetpack Compose, Room, Retrofit (App)
- FastAPI, Node.js, Express, PostgreSQL, Docker, Pandas (Backend)

---

## 🛡️ Seguridad
- Autenticación JWT centralizada
- Endpoints protegidos en backend


