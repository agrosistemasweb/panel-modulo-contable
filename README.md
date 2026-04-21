# Módulo Contable — Avance Global

Panel consolidado del avance del Módulo Contable completo, combinando las 5 listas de Sprint (carpeta `Sprint 2026`).

## Fuentes

- Sprint 1 — list `901323690606`
- Sprint 2 — list `901324230121`
- Sprint 3 — list `901324539845`
- Sprint 4 — list `901325316130`
- Sprint 5 — list `901326731539`

Se consume todo vía el Cloudflare Worker `panel-bugs-proxy` (inyecta el token de ClickUp).

## Qué muestra

- **Agrupación por sección funcional**: Configuración, Listas, Registración, Informes Contables, Informes Impositivos, Otros.
- **Dentro de cada sección, los flujos** (Cuentas Corrientes, Cuentas Contables, Centro de Costos, etc.) parseados del título de cada tarjeta.
- **Buckets de estado**:
  - *Por Hacer* (`to do`)
  - *En Desarrollo* (`in progress`, `a revisar`, `blocked`, `review`, `automation`)
  - *En QA* (`waiting qa`, `qa`)
  - *Done* (`done`, `closed`)
- **Indicador de retrabajo 🔁**: detecta tarjetas cuyo título contiene "Reabierta" / "Reabierto".
- **Progreso global** y **por sección/flujo** con barra visual.
- Filtros por sección, estado, sprint, búsqueda por nombre, solo reabiertas.
- Auto-refresh cada 5 min para reflejar cambios.
- Exportar PDF con resumen y detalle por sección.

## Publicación

GitHub Pages desde `main`, raíz del repo.
