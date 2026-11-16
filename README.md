# Instalación de PostgreSQL en Docker y Configuración en DataGrip

**Estudiante:** Luis Pedro Diaz Martinez  
**Carné:** 2890-21-12316  
**Universidad:** Universidad Mariano Gálvez de Guatemala (UMG)  

---

## Objetivo
Implementar un servidor de base de datos **PostgreSQL** mediante contenedores en **Docker**, configurar **JetBrains DataGrip** como entorno de desarrollo integrado (IDE) y crear una primera base de datos funcional.

---

## 1. Comando para ejecutar Docker con PostgreSQL

Con **Docker Desktop** instalado y en ejecución, abrí una terminal y ejecuté el siguiente comando para descargar la imagen oficial de PostgreSQL, crear el contenedor llamado `postgres-db`, establecer la contraseña del usuario administrador y exponer el puerto `5432`:

```bash
docker run --name postgres-db -e POSTGRES_PASSWORD=yourpassword -p 5432:5432 -d postgres