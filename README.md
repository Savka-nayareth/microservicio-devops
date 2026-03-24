# Microservicio - Evaluación Parcial 1 DevOps

Evaluación parcial de Ingeniería DevOps implementando prácticas de CI/CD y automatización.

## 1. Estrategia de Ramificación (Branching Strategy)
Para este proyecto hemos decidido utilizar **GitFlow**. 
**Justificación:** Elegimos GitFlow porque nos permite mantener un control estricto sobre las versiones de producción (`main`) mientras integramos continuamente el nuevo trabajo en un entorno de desarrollo (`develop`). Facilita el trabajo colaborativo al aislar las nuevas funcionalidades en ramas `feature/` y permite reaccionar rápidamente a errores críticos en producción mediante ramas `hotfix/`.

## 2. Convenciones de Nomenclatura de Ramas (Branch Naming)
Todas las ramas deben seguir este formato en minúsculas:
* **Producción:** `main`
* **Desarrollo:** `develop`
* **Nuevas características:** `feature/<nombre-breve-de-la-caracteristica>` (Ej: `feature/login-api`)
* **Corrección de errores en producción:** `hotfix/<nombre-del-error>` (Ej: `hotfix/error-cors`)

## 3. Convenciones de Mensajes de Commit
Utilizaremos Conventional Commits para asegurar la trazabilidad. El formato es: `tipo: mensaje breve`.
* `feat:` Para nuevas características.
* `fix:` Para solucionar errores.
* `docs:` Para cambios en la documentación.
* `chore:` Para tareas de mantenimiento o configuración.

## 4. Flujos de Merge y Estrategias de Revisión
* Todo el código nuevo se desarrolla en ramas `feature/` o `hotfix/`.
* No se permiten *commits* directos a `main` ni a `develop`.
* Para integrar código a `develop` o `main`, se debe crear un **Pull Request (PR)** en GitHub.
* El PR debe ser revisado por al menos un miembro del equipo antes de ser aprobado.

## 5. Reflexiones Individuales
* En esta primera etapa, lo que más me costó fue entender cómo enlazar las carpetas correctamente entre la terminal y el editor. Siento que hoy aprendí mucho, especialmente a clonar repositorios de GitHub. Ya que estoy realizando este encargo de forma individual, mi contribución ha sido realizar todo el trabajo práctico: configurar el repositorio base inicial, crear la rama develop y documentar las convenciones.