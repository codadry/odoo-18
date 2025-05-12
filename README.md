# Odoo 18 con Docker Compose

Este repositorio despliega una instancia de **Odoo 18** junto con **PostgreSQL 16** utilizando Docker Compose. Es ideal para entornos de desarrollo y pruebas.

---

## 🧾 ¿Qué es Odoo?

**Odoo** es un conjunto de aplicaciones empresariales de código abierto que cubre todas las necesidades de gestión de una empresa: desde CRM, ventas, contabilidad, inventario y recursos humanos, hasta manufactura, comercio electrónico y más.

### ✅ Ventajas de usar Odoo

- Plataforma modular: puedes activar solo los módulos que necesites.
- Interfaz moderna y amigable.
- Altamente personalizable con módulos propios.
- Comunidad activa y soporte empresarial disponible.
- Código abierto, sin costos de licencia para la versión Community.

---

## 🚀 Cómo iniciar

1. Clona el repositorio:
   ```bash
   git clone https://github.com/tu-usuario/tu-repositorio.git
   cd tu-repositorio
````

2. Verifica o crea el archivo `.env` con el siguiente contenido:

   ```env
   ODOO_HOST=db
   ODOO_USER=odoo
   ODOO_PASSWORD=odoo
   ```

3. Levanta los servicios:

   ```bash
   docker compose up -d
   ```

4. Accede a Odoo en tu navegador:

   ```
   http://tu-ip:8201
   ```

---

## 🔐 Credenciales por defecto

* **Usuario:** `admin`
* **Contraseña:** `admin`

---

## 🛑 Detener los servicios

```bash
docker compose down
```

---

## ✅ Requisitos

* Docker
* Docker Compose

---

## ⚙️ Personalización

Puedes cambiar configuraciones como credenciales u otras opciones desde los archivos `.env` y `docker-compose.yml`.

---

## 📌 Notas

* Odoo expone su servicio en el puerto interno **8069**, pero se mapea al puerto **8201** externamente.
* Se recomienda usar un proxy reverso con HTTPS para producción.


