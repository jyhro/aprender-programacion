# Extra - Mantén tu repo actualizado

> Tu copia local envejece: los módulos mejoran cada semana. Actualiza antes de estudiar para no aprender sobre una versión vieja.

## Actualizar con Git (terminal)

Corre esto dentro de la carpeta del repo:

```bash
git status             # ¿tengo cambios sin guardar?
git pull               # trae lo último de GitHub
git log --oneline -3   # confirma qué llegó
```

Si `git status` muestra tus propios cambios (tu diario lleno, por ejemplo), guárdalos primero con un commit o no hagas `pull` todavía: el `pull` mezcla y con cambios a medias salen conflictos.

## Actualizar con GitHub Desktop

1. Abre el repo en la app.
2. Pulsa `Fetch origin` para ver si hay novedades.
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
> Doc v1.0.0 · 2026-11-04 · Creación del módulo extra.
