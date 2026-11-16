# Backlog priorizado de mejoras

**Estado:** completado · 10 ítems con historia, criterio de aceptación, prioridad y MoSCoW · 9 implementados en el [prototipo v2](../../v2_propuesta/prototipo-v2.html).

Prioridad = severidad × confianza ÷ esfuerzo. Confianza: Alta 1 · Confirmado 0,8 · A verificar 0,5. Esfuerzo: S = 1 · M = 2 · L = 3.
Cada fila se convierte en una Issue con la etiqueta de severidad y el enlace a la matriz.

| ID | Historia de usuario | Origen | Sev. | Conf. | Esf. | Prioridad | MoSCoW | Criterio de aceptación | En la v2 | Issue |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| B1 | Como estudiante, quiero que al cambiar el horario se conserve lo que elegí para no repetir pasos | H2 | 3 | 0,8 | S | 2,40 | Must | Volver del Resumen mantiene día, hora y modalidad resaltados, con aviso | ✔ | #__ |
| B5 | Como estudiante, quiero saber por qué no puedo elegir una hora ocupada | H6 | 2 | 0,8 | S | 1,60 | Should | Tocar «Ocupado» muestra la hora libre más cercana; contraste ≥ 4,5:1 | ✔ (6,1:1) | #__ |
| B7 | Como estudiante, quiero reprogramar partiendo de mi tutoría original | H8 | 2 | 0,5 | S | 1,00 | Should | Preselecciona día, hora y modalidad originales; «atrás» vuelve a Mis tutorías | ✔ | #__ |
| B8 | Como usuario de teclado, quiero cerrar la hoja con Esc | H9 | 2 | 0,5 | S | 1,00 | Should | Esc cierra, el foco no sale de la hoja y vuelve a la tarjeta que la abrió | ✔ | #__ |
| B9 | Como estudiante, quiero indicar el tema que quiero revisar | H7 | 2 | 0,5 | S | 1,00 | Could | Campo opcional de 140 caracteres en el Resumen | ✔ | #__ |
| B2 | Como estudiante, quiero buscar a un docente por su nombre desde Inicio | H1 | 3 | 0,5 | M | 0,75 | Must | «Ramos» muestra a la Dra. María Alejandra Ramos; sin resultados → sugerencias | ✔ | #__ |
| B3 | Como estudiante, quiero cancelar o reprogramar una tutoría futura | H3 | 3 | 0,5 | M | 0,75 | Must | El detalle tiene «Cancelar» y «Reprogramar»; cancelar pide confirmación y permite deshacer | ✔ | #__ |
| B4 | Como estudiante, quiero elegir el día de la tutoría | H4 | 3 | 0,5 | L | 0,50 | Should | Selector de 5 días hábiles; los horarios cambian según el día | ✔ | #__ |
| B10 | Como estudiante, quiero entender qué significa «Pendiente» | H10 | 1 | 0,5 | S | 0,50 | Could | Texto de ayuda bajo el estado | ✔ | #__ |
| B6 | Como estudiante, quiero ver datos coherentes entre pantallas | H5 | 2 | 0,5 | M | 0,50 | Won't (ahora) | Depende de datos reales del backend | — | — |

El puntaje ordena; el MoSCoW lo decide el equipo. B2 y B3 tienen prioridad numérica media por su esfuerzo, pero son **Must** porque sin ellos T1 y T5 no se pueden completar por la ruta esperada. B4 es severo y costoso: **Should** en la v2.

## Matriz impacto / esfuerzo

| | Bajo esfuerzo | Alto esfuerzo |
| --- | --- | --- |
| **Alto impacto** | **Hacer ya:** B1, B5, B7, B8 | **Planificar:** B2, B3, B4 |
| **Bajo impacto** | **Si sobra tiempo:** B9, B10 | **Cuestionar:** B6 |

## Alcance de la v2

- **Must:** B1, B2, B3 → implementados
- **Should:** B4, B5, B7, B8 → implementados
- **Could:** B9, B10 → implementados
- **Won't (ahora):** B6

Evidencia: [prototipo-v2.html](../../v2_propuesta/prototipo-v2.html) (cada cambio lleva su etiqueta B#), [capturas v2](../../v2_propuesta/capturas) y [maqueta v1 → v2](../../v2_propuesta/maqueta-v1-v2.html). Siguiente paso: volver a medir T3 y T5 con participantes nuevos (v1 → prueba → v2 → prueba).
