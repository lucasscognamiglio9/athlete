# Athlete

## Terminás de entrenar, hablás con tu coach y él hace el resto.

![Athlete — coach personal de entrenamiento dentro de ChatGPT](assets/athlete-banner.png)

[Instalar Athlete](#instalación) · [Ver cómo funciona](#una-sesión-real)

Athlete es un coach personal de entrenamiento que funciona dentro de ChatGPT.

Cuando el seguimiento exige volver una y otra vez sobre planillas, notas y sesiones para entender lo que el atleta ya mostró, Athlete revisa todo tu historial antes de decidir. Detecta patrones, busca la evidencia científica que realmente aplica a vos, anticipa lo que sigue y cambia lo que no te funciona. Cada ajuste y cada progresión siguen una lógica y tienen un porqué.

## Una sesión real

> “Hice banca con 55 kg, 10 y 10, RIR 2 en ambas. Sentadilla 70 kg, 10 y 10, RIR 3. Estuvo muy bien el día de hoy.”

Athlete interpreta el mensaje, pregunta sólo si falta algo importante, registra la sesión en la misma planilla, verifica la escritura y te dice qué corresponde hacer después.

> conocer → planificar → entrenar → registrar → revisar → adaptar

## Qué puede hacer

Athlete crea y adapta tu plan, acompaña cada sesión, registra lo que hiciste y revisa tu progreso.

## Cómo conserva tu progreso

Athlete guarda tu progreso en una única planilla de **Google Drive**.

- **Perfil** con tus objetivos, contexto y preferencias.
- **Plan** con tu entrenamiento y sus reglas de progresión.
- **Sesiones** con el trabajo que realizaste.
- **Decisiones** con cada cambio y su motivo.

Así evitás copias y cientos de sesiones ocupando ChatGPT Memory.

## Instalación

### Directorio público — próximamente

1. Instalá **Athlete** desde Plugins.
2. Instalá y autorizá **Google Drive**.
3. Abrí un chat nuevo y escribí **“Quiero empezar con Athlete.”**

### Desde este repositorio

Desde la raíz del repositorio ejecutá

```bash
codex plugin marketplace add .
```

El comando agrega este repositorio como fuente local. Reiniciá ChatGPT Desktop, instalá **Athlete** desde Plugins y comenzá en una conversación nueva.

## Probalo

- “Conoceme y prepará mi primer plan.”
- “¿Qué me toca entrenar hoy?”
- “Registrá lo que hice, revisá mi progreso y decime qué sigue.”

## Alcance

Athlete está pensado para fuerza, hipertrofia y entrenamientos de gimnasio.

## Arquitectura

Un único coach se ocupa de conocerte, planificar, acompañarte, registrar lo que hiciste y revisar tu progreso. Athlete funciona con ChatGPT y Google Drive sin una aplicación propia.

## Referencias

Athlete adapta al coaching patrones de [Skills for Real Engineers](https://github.com/mattpocock/skills) de Matt Pocock, especialmente sus skills pequeñas y los métodos `grill-me`/`grilling` y `research`.

[Licencia MIT](LICENSE)
