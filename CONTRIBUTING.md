# Contribuir a Athlete

Athlete busca hacer simple lo complejo sin bajar la calidad del coaching. Una contribución debe mejorar una conducta observable del producto, no agregar arquitectura preventiva.

## Antes de proponer un cambio

1. Describí el problema desde la experiencia del atleta.
2. Agregá o actualizá un caso en `evals/` que falle sin el cambio.
3. Mantené un solo head coach, las cinco skills actuales y un único archivo canónico.
4. No agregues registros de deportes, persistencia en Memory, proveedores hipotéticos, backend ni MCP propio.

## Verificación local

Ejecutá:

```bash
python3 -m unittest tests/test_release_contract.py -v
python3 /ruta/a/plugin-creator/scripts/validate_plugin.py plugins/athlete
```

Reemplazá `/ruta/a/plugin-creator` por la ubicación de la skill oficial instalada en tu entorno. Después validá cada carpeta de `plugins/athlete/skills/` con el validador oficial de skills.

## Evaluación conductual auditable

Los tests locales validan contratos estáticos; no sustituyen la ejecución del coach. Para cada cambio conductual:

1. Abrí un contexto limpio con la versión exacta del paquete.
2. Entregá un solo caso de `evals/product-cases.json` sin revelar su `expected_skills` ni su `observable`.
3. Conservá la respuesta, la secuencia de skills y un trace semántico de lecturas, escrituras y read-backs.
4. Evaluá el resultado con `evals/rubric.md` en integridad y calidad por separado.
5. Guardá el input, output, versión, fecha, resultado por criterio y limitaciones en `evals/results/`.
6. Para la regresión de routing, repetí el procedimiento con los prompts de `evals/activation-cases.json` sin mostrar el expected al evaluador.

Si el cambio toca Google Sheets, conservá además la lectura previa, request de mutación, respuesta, read-back, spreadsheet ID y hash de un export posterior; nunca crees un archivo auxiliar como fallback del atleta.

## Pull requests

Incluí el caso afectado, el resultado antes y después, y cualquier limitación que siga abierta. Los cambios de alcance o de arquitectura deben actualizar primero la especificación.
