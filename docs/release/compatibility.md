# Compatibilidad verificada — Athlete 0.1.0

Fecha de verificación: 2026-08-19.

Esta matriz contiene sólo ejecuciones realizadas. No convierte documentación de plataforma en una promesa de producto.

| Superficie | Athlete | Google Sheets | Estado |
|---|---|---|---|
| Codex desktop, proyecto local | Paquete y cinco skills validados; instalación desde catálogo no disponible en esta sesión | Plugin oficial Google Drive conectado; lectura, escritura y read-back en una única planilla nativa verificados | Parcialmente verificado |
| ChatGPT personal | Formato oficialmente compatible; instalación limpia pendiente de una ficha o marketplace accesible | Requiere instalar y autorizar Google Drive por separado | No declarar todavía |
| ChatGPT Project | No ejecutado | No ejecutado | No declarar todavía |
| Codex CLI | No ejecutado | No ejecutado | No declarar todavía |
| Extensión IDE | Fuera de las superficies de plugins documentadas | — | No compatible |

## Contrato de Google Sheets demostrado

- La integración pertenece al plugin oficial Google Drive, no a Athlete.
- Todas las operaciones usaron el mismo spreadsheet ID.
- La escritura fue releída y coincidió con los valores solicitados.
- Una búsqueda posterior encontró un único archivo de QA con ese título e ID.

## Regla de publicación

Una superficie pasa a “compatible” sólo después de una instalación limpia, descubrimiento de las cinco skills y un ciclo completo con escritura verificada. La disponibilidad por plan, región o workspace se documenta desde la cuenta realmente probada; no se infiere.
