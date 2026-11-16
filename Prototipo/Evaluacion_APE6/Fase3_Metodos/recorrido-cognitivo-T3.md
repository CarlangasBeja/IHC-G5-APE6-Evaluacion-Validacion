# M2 · Recorrido cognitivo de T3

Método: Wharton, Rieman, Lewis y Polson (1994).

**Estado:** completado (inspección del equipo G5 sobre la v1, 10/11/2026).

- **Persona:** estudiante de la UTA que usa la app por primera vez.
- **Tarea:** T3 — desde el Resumen (10:00 · Virtual), cambiar a 11:00 manteniendo la modalidad virtual y confirmar.
- **Estado inicial:** Resumen de tutoría con Msc. Andrea Paola Mendoza, Programación, 10:00, Virtual.

## Las 4 preguntas por paso

1. ¿**Intentará** el usuario lograr el efecto correcto?
2. ¿**Notará** que la acción correcta está disponible?
3. ¿**Asociará** la acción con el efecto que busca?
4. ¿**Verá progreso** después de ejecutarla?

## Resultado

| Paso de la ruta correcta | ¿Intentará? | ¿Notará? | ¿Asociará? | ¿Verá progreso? | Historia de fallo / éxito |
| --- | --- | --- | --- | --- | --- |
| 1. Tocar «Cambiar horario» en el Resumen | ✔ | ✔ | ✔ | ✘ | Vuelve a horarios sin hora marcada y con «Presencial»: no hay señal de que su elección previa se conservó |
| 2. Elegir 11:00 | ✔ | ✔ | ✔ | ✔ | «Seleccionado» y botón «Continuar con 11:00»: buen feedback |
| 3. Volver a elegir «Virtual» | ✘ | ✔ | ✔ | ✔ | Cree que la modalidad se mantuvo; no tiene motivo para tocarla → riesgo de reservar presencial |
| 4. Continuar al Resumen | ✔ | ✔ | ✔ | ✔ | El Resumen muestra la modalidad: última oportunidad de detectar el error |
| 5. Confirmar tutoría | ✔ | ✔ | ✔ | ? | La v1 no muestra con claridad qué quedó registrado; la v2 añade una pantalla de éxito con los datos y el estado (B10) |

## Conclusión

Confirma **H2** por un camino independiente de la heurística y revela una consecuencia: un **error silencioso** (modalidad equivocada) que solo el Resumen puede atrapar. En la prueba con usuarios se observa si P01–P05 revisan la modalidad en el Resumen.

En la v2, «Cambiar horario» conserva día, hora y modalidad con el aviso «Conservamos tu selección» (B1): el paso 1 pasa a ✔ en «¿Verá progreso?» y el paso 3 deja de ser necesario. Ver [capturas v2](../../v2_propuesta/capturas/05_B1_cambiar_horario_conserva.jpg).

Evidencia: [08_resumen.jpg](../../v1_capturas/08_resumen.jpg) → [09_H2_cambiar_horario_pierde_seleccion.jpg](../../v1_capturas/09_H2_cambiar_horario_pierde_seleccion.jpg)
