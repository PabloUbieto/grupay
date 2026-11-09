# Guía de contribución

Normas que seguimos para trabajar en Grupay. Si algo no está aquí, lo hablamos antes de hacerlo.

## 🌳 Ramas principales

| Rama | Contenido |
|---|---|
| `main` | Versión final del proyecto. Bloqueada hasta la entrega |
| `develop` | Rama de trabajo donde se integra todo |

- No se trabaja directamente en `main` ni en `develop`.
- Todo cambio entra por **Pull Request** y se revisa antes de mergear.
- **Un propósito por PR.** Si se arregla un bug y se añade una pantalla, son dos PR.
- Antes de borrar, mover o renombrar archivos o carpetas, o de tocar la configuración del repo, lo hablamos.
- Nunca se suben contraseñas, claves de API ni archivos `.env`.

## 🌿 Ramas de trabajo

Formato `tipo/descripcion-corta`, en inglés y en minúsculas:

| Tipo | Uso | Ejemplo |
|---|---|---|
| `feat` | Nueva funcionalidad | `feat/user-login` |
| `fix` | Corrección de un error | `fix/expense-total` |
| `docs` | Documentación | `docs/api-endpoints` |
| `refactor` | Reestructurar sin cambiar el comportamiento | `refactor/group-service` |
| `style` | Formato, sin cambios de lógica | `style/format-css` |
| `test` | Tests | `test/expense-service` |
| `chore` | Configuración y mantenimiento | `chore/update-gitignore` |

Las ramas se crean desde `develop` actualizada y se borran solas tras el merge.

## ✍️ Commits

[Conventional Commits](https://www.conventionalcommits.org/) en inglés:

```
feat(auth): add login form
fix(expenses): round split amounts to two decimals
docs(readme): add setup instructions
```

Commits pequeños: un cambio lógico por commit.

## 🔀 Pull Requests

1. Actualiza `develop` (Fetch + Pull) y crea tu rama desde ella.
2. Haz tus commits y publica la rama.
3. Abre la PR hacia `develop` con el título en formato Conventional Commits (`feat(auth): add login form`).
4. Rellena la plantilla (Summary / Changes / Notes).
5. Revisa **Files changed** antes de pedir revisión.
6. Tras la revisión, se mergea con **Create a merge commit**.

## 🐛 Issues

Bugs e ideas se abren como issue con su plantilla. Antes de trabajar en uno, asígnatelo para no pisarnos.

## 🎨 Diseño

El diseño está en Figma (enlace en [docs/design](docs/design/README.md)). Las capturas exportadas van en `docs/design/screens/` con el formato `NN-nombre-pantalla.png`.
