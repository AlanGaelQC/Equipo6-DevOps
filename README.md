# 🛒 MultiTienda AWS – Proyecto Final DevOps

Bienvenido al repositorio oficial del proyecto **MultiTienda**, una aplicación web funcional desarrollada como parte del Proyecto Final de la materia de DevOps. Este sistema permite a los usuarios registrarse, explorar productos organizados por tiendas, realizar compras simuladas, y a los administradores gestionar el inventario de cada tienda. Todo el entorno ha sido desplegado y configurado utilizando servicios de AWS y Docker, con infraestructura definida mediante Terraform.

---

## 🎯 Objetivo del Proyecto

Desarrollar una **aplicación web de tipo multi tienda**, alojada en AWS mediante instancias EC2 y bases de datos RDS, desplegada en un contenedor Docker y documentada completamente en GitHub. Este proyecto tiene como meta integrar conocimientos de infraestructura, automatización, desarrollo y buenas prácticas de documentación profesional.

---

## ⚙️ Tecnologías Utilizadas

- **AWS EC2** – Para alojar la aplicación.
- **AWS RDS (MySQL/PostgreSQL)** – Para almacenar usuarios, productos e inventario.
- **Terraform** – Infraestructura como código para todo el entorno en AWS.
- **Docker** – Contenerización de la aplicación web.
- **GitHub** – Control de versiones y documentación colaborativa.
- **HTML/CSS/JS/PHP/Node.js/etc.** – Según las tecnologías usadas en tu stack.
- **Lucidchart** – Para el diagrama de arquitectura.
- **Markdown & Word** – Para documentación técnica y entregables.

---

## 🧩 Funcionalidades Principales

- Registro e inicio de sesión de usuarios.
- Navegación por productos organizados por tienda.
- Carrito de compras y simulación de pago.
- Actualización automática del inventario tras cada compra.
- Panel administrativo para modificar inventario, precios y productos.

---

## 🚀 Despliegue

Este proyecto se encuentra desplegado en una instancia EC2 con acceso público, utilizando Docker para la ejecución de la aplicación. Toda la infraestructura fue creada desde cero mediante Terraform, siguiendo prácticas de seguridad en AWS (Security Groups, VPC).

---

## 📁 Estructura del Repositorio

- `/frontend/` – Código de la interfaz web.
- `/backend/` – Lógica del servidor, autenticación y conexión a la base de datos.
- `/infra/` – Archivos Terraform para desplegar la infraestructura.
- `Dockerfile` – Contenerización de la aplicación.
- `README.md` – Este archivo.
- `Documentacion.docx` – Capturas, registro de errores y evidencia del despliegue.

---

## 👥 Equipo de Trabajo

- Alan [Tu Apellido] – Infraestructura y despliegue en AWS.
- Gael Quintanilla Clemente – Frontend.
- Jair Emmanuel Rivera Cano – Backend.
- José Manuel Nájera Loera – QA y documentación.

---

## 📌 Notas

Este repositorio incluye toda la documentación necesaria para replicar el entorno, así como instrucciones para desplegar la aplicación desde cero. Para más detalles, consulta el archivo `README.md` completo y la documentación adjunta en Word.

