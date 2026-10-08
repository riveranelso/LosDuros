# Estado de sincronización con GitHub

## Estado actual

- **Guardado localmente:** sí. Ampliación completa en `~/workspace/zion/los-duros/`.
- **Preparado para GitHub:** sí. Ver manifiesto de adiciones abajo.
- **Publicado en GitHub:** NO. El acceso actual es de solo lectura (fine-grained token, Contents: Read-only). No se afirmó ni se realizará publicación sin acceso de escritura autorizado.

## Manifiesto de adiciones propuestas (para cuando exista escritura autorizada)

Archivos nuevos propuestos bajo la raíz del repositorio `riveranelso/LosDuros`:

```
INDICE.md
01-identidad-alcance.md
02-voz-editorial.md
03-comprension-comentario.md
04-cero-chotiaera.md
05-respuestas-ctas.md
06-dos-fijos.md
07-caption-ig.md
08-youtube-descripciones.md
09-lives-shorts-retencion.md
10-logo-oficial.md
11-preservacion-visual.md
12-metricas-historicas.md
13-personas-correcciones.md
14-indio-blaze.md
15-investigacion-titulos.md
16-referencias-assets.md
17-zion-enrutamiento.md
18-checklist-preflight.md
19-pendiente-recuperar.md
FUENTES-Y-CAMBIOS.md
SYNC-GITHUB.md
```

Archivos que NO se tocan: `brain/brand-rules.md`, `brain/comment-rules.md`, `brain/asset-registry.md` (originales intactos).

## Handoff a Claude Code (2026-10-07)

- Se preparó `los-duros-brain.zip` con toda la carpeta (originales + ampliación + índice + registros), verificado sin secretos.
- Se entregó el bloque de instrucciones `CLAUDE-CODE-SYNC.md` para que Claude Code revise el diff, compruebe ausencia de secretos y publique con su acceso autorizado.
- **Estado: guardado localmente, pendiente de GitHub.** No se marcará como publicado hasta verificar el commit y las rutas publicadas.

## Cobertura de esta entrega

**Qué cubre:** reglas editoriales, voz, comprensión de comentarios, CERO CHOTIAERA, CTAs y dos fijos, formatos de IG/YouTube, lives/Shorts, logo bloqueado (regla + diferencia de asset), preservación visual, métricas históricas (1–4 oct 2026), correcciones de nombres, contexto Indio/Blaze (solo lo solicitado, no la cronología), investigación/títulos, referencias de assets (pistas), enrutamiento ZION (reportado), checklist complementario, índice y registro de fuentes.

**Qué falta:** ver `19-pendiente-recuperar.md` (cronología de Indio, conversaciones originales, archivo del logo, textos aprobados, assets referenciados, detalle 28/90 días, handles oficiales, library de ChatGPT).

No se declara "brain completo".
