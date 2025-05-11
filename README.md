# 🛒 MultiShop – Proyecto Final DevOps (EQUIPO 6)

Este repositorio contiene el desarrollo y despliegue del proyecto **MultiShop**, una tienda en línea completamente funcional, basada en una plantilla web profesional, adaptada, contenerizada con Docker y desplegada mediante infraestructura como código usando Terraform en Amazon Web Services (AWS). Desarrollado como proyecto final de la materia de **DevOps**.

---

## 🎯 Objetivo del Proyecto

Desarrollar una aplicación web de comercio electrónico con las siguientes características:

- **Frontend responsivo** utilizando una plantilla HTML profesional.
- **Autenticación básica** de usuarios (registro e inicio de sesión).
- **Gestión de productos e inventario** (visualización, compra, modificación).
- **Despliegue contenerizado con Docker.**
- **Infraestructura automatizada con Terraform en AWS (EC2 y RDS).**
- **Control de versiones y documentación técnica detallada en GitHub.**

---

## ⚙️ Tecnologías Utilizadas

| Herramienta     | Descripción                                                   |
|-----------------|---------------------------------------------------------------|
| **AWS EC2**     | Instancia para ejecutar la aplicación                         |
| **AWS RDS**     | Base de datos (MySQL/PostgreSQL) para usuarios e inventario   |
| **Terraform**   | Infraestructura como código                                   |
| **Docker**      | Contenerización de la aplicación                              |
| **GitHub**      | Repositorio de código y control de versiones                  |
| **Lucidchart**  | Diagrama de arquitectura                                      |
| **HTML/CSS/JS** | Plantilla MultiShop para frontend                             |

---

## 📁 Estructura del Repositorio
EQUIPO6-DEVOPS/
│
├── frontend/ # Código de la plantilla web MultiShop
│ ├── cart.html
│ ├── checkout.html
│ ├── contact.html
│ ├── detail.html
│ ├── index.html
│ ├── shop.html
│ ├── CSS/
│ ├── js/
│ ├── img/
│ ├── lib/
│ ├── mail/
│ └── SCSS/
│
├── backend/ # (Opcional) Archivos PHP o conexión a BD futura
│
├── infra/ # Archivos Terraform para infraestructura AWS
│ ├── main.tf
│ ├── variables.tf
│ ├── outputs.tf
│
├── Dockerfile # Imagen Docker de la aplicación
├── README.md # Este archivo
└── Documentacion.docx # Evidencias, errores y capturas del despliegue

---

## 🚀 Guía de Despliegue

### 🔧 Requisitos Previos

- Docker instalado
- AWS CLI y credenciales configuradas
- Terraform instalado

### 📦 Construcción y ejecución con Docker

```bash
# Construir imagen
docker build -t multishop .

# Ejecutar contenedor
docker run -d -p 80:80 multishop
☁️ Despliegue en AWS con Terraform
bash
Copiar
Editar
cd infra
terraform init
terraform apply
Una vez desplegado, accede a la tienda desde la IP pública generada por Terraform (EC2).

🔐 Seguridad
Security Groups: solo permiten tráfico en puertos necesarios (80, 22).

VPC/Subnets: configuradas para control de red.

Variables sensibles: excluidas del repositorio (usar variables de entorno).

📝 Documentación Incluida
README.md: guía de uso y despliegue.

Documentacion.docx:

Capturas de pantalla de AWS (EC2, RDS, VPC, SG).

Diagrama de arquitectura.

Registro de errores encontrados y soluciones aplicadas.

🧠 Diagrama de Arquitectura
Desarrollado en Lucidchart.

Incluye EC2 (app), RDS (DB), VPC, SG y conexiones Docker.

👥 Roles del Equipo
Nombre	Rol
Alan [Tu Apellido]	Infraestructura (Terraform, EC2, Docker)
Gael Quintanilla Clemente	Frontend (Plantilla MultiShop)
Jair Emmanuel Rivera Cano	Apoyo técnico y despliegue
José Manuel Nájera Loera	QA, documentación, validación

📌 Notas Finales
Este proyecto demuestra habilidades clave de un entorno DevOps moderno: contenerización, automatización del despliegue en la nube, documentación profesional y colaboración en equipo. A pesar de partir de una plantilla visual ya existente, se integró con herramientas de desarrollo reales para crear una solución funcional, replicable y documentada.
