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

Cada uno trabaja en su propia rama, creada desde `develop`:

| Rama | Persona |
|---|---|
| `feature/pablo` | Pablo |
| `feature/alvaro` | Álvaro |

- Cada uno trabaja **solo en su rama**. Nunca se hacen commits en la rama del otro.
- Antes de empezar cada tarea, actualiza tu rama con lo último de `develop` (en GitHub Desktop: **Branch → Update from develop**).
- Cuando termines una tarea, abre una PR de tu rama hacia `develop`. **Una tarea por PR.**
- Mientras tu PR esté abierta, no subas commits de otra tarea: se añadirían a esa PR. Espera al merge.
- Tu rama no se borra tras el merge: sigues trabajando en ella.

## ✍️ Commits

[Conventional Commits](https://www.conventionalcommits.org/) en inglés:

```
feat(auth): add login form
fix(expenses): round split amounts to two decimals
docs(readme): add setup instructions
```

Commits pequeños: un cambio lógico por commit.

## 🔀 Pull Requests

1. Actualiza tu rama desde `develop`.
2. Haz tus commits y súbelos (Push).
3. Abre la PR hacia `develop` con el título en formato Conventional Commits (`feat(auth): add login form`).
4. Rellena la plantilla (Summary / Changes / Notes).
5. Revisa **Files changed** antes de pedir revisión.
6. Tras la revisión, se mergea con **Create a merge commit**.

## 🐛 Issues

Bugs e ideas se abren como issue con su plantilla. Antes de trabajar en uno, asígnatelo para no pisarnos.

## 🎨 Diseño

El diseño está en Figma. Antes de cambiar una pantalla respecto al diseño, lo hablamos.