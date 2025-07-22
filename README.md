# Go-Web - Project Management API

[![Go Report Card](https://goreportcard.com/badge/github.com/spookycoincidence/go-web)](https://goreportcard.com/report/github.com/spookycoincidence/go-web)  
[![Build Status](https://github.com/spookycoincidence/go-web/actions/workflows/go.yml/badge.svg)](https://github.com/spookycoincidence/go-web/actions/workflows/go.yml)

---

## Descripción

Este proyecto es una aplicación web desarrollada en Go que implementa un sistema completo para la gestión de proyectos y tareas. Basado en una arquitectura modular, utiliza Echo como framework HTTP, GORM para manejo de base de datos PostgreSQL y Redis para cacheo, proporcionando una API RESTful segura y escalable.

---

## Funcionalidades

- CRUD completo para proyectos y tareas
- Autenticación y autorización de usuarios
- Cacheo de consultas frecuentes con Redis
- Documentación automática de API con Swagger
- Configuración flexible mediante variables de entorno
- Soporte para migraciones y seeders

---

## Tecnologías principales

- Golang
- Echo (framework web)
- GORM (ORM para PostgreSQL)
- Redis (cacheo)
- Docker & Docker Compose (para orquestar servicios)

---

## Instalación y ejecución local

1. Clonar el repositorio:
```bash
git clone https://github.com/spookycoincidence/go-web.git
cd go-web
```


2. Configurar variables de entorno (puede ser en un archivo .env):
```bash
DATABASE_URL=postgres://usuario:password@localhost:5432/tu_db?sslmode=disable
REDIS_ADDR=localhost:6379
SERVER_PORT=:8080
```

3. Ejecutar con Docker Compose (opcional):
```bash
docker-compose up
```

4. O ejecutar directamente:
```bash
go mod tidy
go run main.go
```

5. La API estará disponible en http://localhost:8080


## 📌 Endpoints Disponibles

| POST   | /projects           |Crear nuevo proyecto      |
| GET    | /proyects           |Listar Proyectos          |
| GET    | /projects/:id       | Obtener proyecto por ID  |
| PUT    | /projects/:id       | Actualizar proyecto      |
| DELETE | /projects/:id       | Eliminar proyecto        |

## 📝 Inspiración
Este proyecto está basado y adaptado del repositorio original StarpTech/go-web, con modificaciones para ajustarlo a un sistema de gestión de proyectos y tareas personalizado..

## Desarrollado con ❤️ por spookycoincidence






