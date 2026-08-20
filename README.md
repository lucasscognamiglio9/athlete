# Athlete

![Athlete — coach personal de entrenamiento dentro de ChatGPT](assets/athlete-banner-favorite-v6.png)

## Terminás de entrenar, hablás con tu coach y él hace el resto.

[Instalar Athlete](#instalación) · [Ver cómo funciona](#una-sesión-real)

Athlete es un coach personal de entrenamiento que funciona dentro de ChatGPT.

Cuando el seguimiento exige volver una y otra vez sobre planillas, notas y sesiones para entender lo que el atleta ya mostró, Athlete usa IA para revisar todo tu historial en cada decisión, detectar patrones, buscar la evidencia científica que realmente aplica a vos, anticipar lo que sigue, cambiar lo que no te funciona y hacer que cada etapa, cada ajuste y cada progresión sigan una lógica y tengan un porqué.

## Una sesión real

> “Hice banca con 55 kg, 10 y 10, RIR 2 en ambas. Sentadilla 70 kg, 10 y 10, RIR 3. Estuvo muy bien el día de hoy.”

Athlete interpreta el mensaje, pregunta sólo si falta algo importante, registra la sesión en la misma planilla, verifica la escritura y te dice qué corresponde hacer después.

```text
conocer → planificar → entrenar → registrar → revisar → adaptar
```

No necesitás completar formularios, ordenar columnas ni aprender comandos.

## Qué puede hacer

- Crear un plan ajustado a vos y modificarlo cuando cambie tu contexto.
- Mostrarte la sesión y ayudarte a decidir cuando algo cambia durante el entrenamiento.
- Registrar, corregir y detectar posibles duplicados sin inventar datos faltantes.
- Revisar tendencias, preparar la próxima progresión y explicar la evidencia relevante.

## Cómo conserva tu progreso

Athlete usa el plugin oficial **Google Drive** para organizar el estado durable en cuatro bloques:

- **Perfil:** objetivos, contexto y preferencias.
- **Plan:** entrenamiento vigente y reglas de progresión.
- **Sesiones:** trabajo realizado y métricas relevantes.
- **Decisiones:** cambios, motivos y evidencia aplicada.

La misma planilla concentra todo el historial: evita copias y no satura ChatGPT Memory.

## Instalación

### Directorio público — próximamente

1. Instalá **Athlete** desde Plugins.
2. Instalá y autorizá **Google Drive**.
3. Abrí un chat nuevo y escribí: **“Quiero empezar con Athlete.”**

### Desde este repositorio

Desde la raíz del repositorio:

```bash
codex plugin marketplace add .
```

El comando agrega este repositorio como fuente local. Reiniciá ChatGPT Desktop, instalá **Athlete** desde Plugins y comenzá en una conversación nueva.

## Probalo

- “Conoceme y prepará mi primer plan.”
- “¿Qué me toca entrenar hoy?”
- “Registrá lo que hice, revisá mi progreso y decime qué sigue.”

## Alcance

La primera versión está diseñada para fuerza, hipertrofia y otras prácticas de gimnasio que comparten tareas, dosis, esfuerzo y progresión. No usa un catálogo rígido de deportes: adapta el método a la forma real del entrenamiento y al atleta.

## Arquitectura

El usuario conversa con un único coach. El plugin coordina cinco skills automáticas: conocer al atleta, diseñar el entrenamiento, acompañar la sesión, registrar y revisar el progreso. Google Drive es una integración oficial separada; Athlete no requiere una aplicación, backend ni MCP propios.

## Referencias

Athlete toma como referencia patrones del proyecto open source [Skills for Real Engineers](https://github.com/mattpocock/skills) de Matt Pocock: skills pequeñas y componibles, `grill-me`/`grilling` para discovery estructurado, `research` para investigación con fuentes primarias y la separación entre skills invocadas por el usuario y por el modelo. Estos patrones fueron adaptados al coaching atlético; Athlete no depende de ese proyecto.

Proyecto: [compatibilidad](docs/release/compatibility.md) · [contribuir](CONTRIBUTING.md) · [licencia MIT](LICENSE)
