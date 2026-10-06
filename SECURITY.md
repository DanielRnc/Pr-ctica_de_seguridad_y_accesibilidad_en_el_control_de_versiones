# Seguridad y Accesibilidad del Proyecto

## 1. Quitar archivos (.gitignore)
He creado el archivo `.gitignore` para no subir cosas innecesarias.

* **Credenciales (`.env`):** Evita publicar mis contraseñas o claves de la base de datos.
* **Archivos del IDE (`nbproject/private/`, `.vscode/`):** Son mis configuraciones locales del editor y rutas de mi PC.
* **Compilados (`build/`, `*.class`):** Ocupan espacio que no vale para nada.
* **Temporales (`*.log`):** Basura que ensucia los commits que hago.

---

## 2. Medidas de seguridad en el equipo
* **Ramas protegidas:** Así  la rama `main` esta limpia.
* **Revisión de Pull Requests:** Mi compañero revisa los cambios antes de fusionarlos a `main` para que no haya errores.
* **Plantillas de configuración:** Uso un archivo `.env.example` sin contraseñas reales como plantilla.

---

## 3. Plan de recuperación
* **Copias locales:** Cada clon local sirve como respaldo si falla GitHub.
* **Uso de `git reflog`:** Si borro un commit o rama por error en mi PC, lo puedo recuperar fácilmente.
* **Uso de Tags:** Etiqueto versiones (ej. `v1.0`) para poder volver a un punto seguro si jodo algo.