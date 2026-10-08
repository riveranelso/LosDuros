# BLOQUE PARA CLAUDE CODE — Publicar ampliación del brain en `riveranelso/LosDuros`

Pega este bloque completo en Claude Code. Claude Code debe ejecutarlo con su acceso autorizado de escritura al repositorio.

---

## Objetivo

Incorporar la ampliación local del brain de LOS DUROS al repositorio `riveranelso/LosDuros` (rama `main`) **sin borrar ni modificar contenido existente**.

## Entrada

El ZIP `los-duros-brain.zip` contiene la carpeta `los-duros/` con:

- `brain/` — los 3 archivos originales: `brand-rules.md`, `comment-rules.md`, `asset-registry.md` (copias de verificación, **no modificar los del repo**).
- `INDICE.md`, `01-identidad-alcance.md` … `19-pendiente-recuperar.md` — archivos **nuevos** de la ampliación.
- `FUENTES-Y-CAMBIOS.md`, `SOURCE.md`, `SYNC-GITHUB.md`, `CLAUDE-CODE-SYNC.md` — documentación.

## Pasos

1. **Extrae el ZIP** en un directorio temporal de trabajo.
2. **Revisa el diff antes de publicar.** Compara cada archivo nuevo contra el contenido actual de `riveranelso/LosDuros@main`. Verifica que:
   - Ningún archivo existente del repo se modifica ni se elimina.
   - Solo se **agregan** archivos nuevos en la raíz del repo (los `01–19`, `INDICE.md`, `FUENTES-Y-CAMBIOS.md`, `SOURCE.md`, `SYNC-GITHUB.md`, `CLAUDE-CODE-SYNC.md`).
   - El contenido agregado coincide con el del ZIP.
3. **Comprueba que no incluya secretos.** Busca en todos los archivos tokens, API keys, contraseñas, credenciales, `hsurr:`, `Bearer`, emails privados o datos de sesión. Si encuentras algo, **detén la publicación** y repórtalo.
4. **Publica los cambios** usando tu acceso autorizado de escritura:
   - Agrega únicamente los archivos nuevos listados arriba.
   - Mensaje de commit sugerido: `Add Los Duros brain expansion (local workspace import, 2026-10-07)`
   - Haz push a la rama `main`.
5. **Confirma la entrega** con:
   - El SHA del commit creado.
   - La lista exacta de rutas publicadas en el repositorio.
   - Confirmación de que ningún archivo existente fue modificado o eliminado.

## Restricciones

- No toques `brain/brand-rules.md`, `brain/comment-rules.md` ni `brain/asset-registry.md` del repo.
- No inventes contenido ni agregues archivos fuera de la lista.
- Si el diff muestra cualquier modificación a archivos existentes, detente y pide confirmación antes de continuar.
