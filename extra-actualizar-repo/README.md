# Extra - Mantén tu repo actualizado

> Tu copia local envejece: los módulos mejoran cada semana. Actualiza antes de estudiar para no aprender sobre una versión vieja.

## Instalar primero (una sola vez)

Necesitas una de estas dos herramientas. Verifica cuál tienes antes de descargar nada.

### Git (terminal)

Git es el programa que copia y mezcla versiones de archivos.

1. Comprueba si ya lo tienes: abre tu terminal y corre `git --version`. Si muestra un número, listo.
2. Si no lo tienes, instálalo según tu sistema:
   - macOS: al correr `git` el sistema ofrece instalarlo solo; acepta y listo. Si no, descárgalo desde la [página oficial de Git](https://git-scm.com/downloads).
   - Windows: descárgalo desde la [página oficial de Git](https://git-scm.com/downloads) e instala con las opciones por defecto (incluye Git Bash, una terminal que entiende `ls` y `pwd`).
   - GNU/Linux: usa tu gestor de paquetes, por ejemplo `sudo apt install git` en Ubuntu y derivadas.
3. Confirma con `git --version` de nuevo.

### GitHub Desktop (app con botones)

GitHub Desktop es la app oficial de GitHub para hacer lo mismo sin terminal: ver cambios, traer y subir con botones. Solo existe para macOS y Windows; en GNU/Linux usa Git por terminal.

1. Descárgala desde la [página oficial de GitHub Desktop](https://desktop.github.com/).
2. Instálala, ábrela e inicia sesión con tu cuenta de GitHub.
3. Añade el repo con `File` y luego `Clone repository` pegando su URL.

## Actualizar con Git (terminal)

Corre esto dentro de la carpeta del repo:

```bash
git status             # ¿tengo cambios sin guardar?
git pull               # trae lo último de GitHub
git log --oneline -3   # muestra los últimos 3 cambios
```

Si `git status` muestra tus propios cambios (tu diario lleno, por ejemplo), guárdalos primero con un commit o no hagas `pull` todavía: el `pull` mezcla y con cambios a medias salen conflictos (dos versiones peleando por el mismo archivo).

## Actualizar con GitHub Desktop

Repo es la carpeta del proyecto en GitHub; clonarla es copiarla entera a tu compu.

1. Abre el repo en la app.
2. Pulsa `Fetch origin` (mirar si hay novedades sin traerlas todavía).
3. Si aparece `Pull origin`, púlsalo para traerlas.
4. Revisa el historial para confirmar qué cambió.

## Cómo saber si tu copia está al día

Cada documento termina con un pie de versión así:

```text
Doc v1.0.0 · 2026-11-04 · Motivo del cambio
```

Compara la versión de tu archivo local con la que ves en GitHub: si la de GitHub es mayor, te falta un `pull`.

> [!TIP]
> Actualiza siempre antes de empezar tu sesión de estudio, igual que afilas el lápiz antes de escribir.

---
> Doc v1.3.0 · 2026-11-04 · Define repo, clonar, fetch y conflictos.
