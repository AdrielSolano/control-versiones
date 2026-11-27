# Control de versiones: sitio web (Unidad 2)

Sitio estático de una sola página (`public/index.html`) publicado con **GitHub Pages**
y desplegado automáticamente con **GitHub Actions**.

## Estructura
```
public/              Sitio web (HTML + CSS)
.github/workflows/   ci.yml (revisión en pull requests) y deploy.yml (despliegue)
```

## Flujo de trabajo
1. `git switch -c feature/nombre` desde `main`.
2. Commits pequeños con mensajes claros.
3. Pull request hacia `main` (se ejecuta `ci.yml`).
4. Merge → se ejecuta `deploy.yml` y se actualiza el sitio.
5. Etiqueta de versión: `git tag v1.0.0` y `git push origin v1.0.0`.

Autor: Adriel Arturo Solano Peraza · Universidad Tecnológica Riviera Maya
