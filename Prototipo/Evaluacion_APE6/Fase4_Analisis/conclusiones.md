# Conclusiones del APE 6

Estructura de cada conclusión: **dato** (qué se midió) → **interpretación** (por qué ocurre, con hallazgo y método) → **acción** (ítem del backlog) → **límite** (qué no se puede afirmar).

## 1. Conclusiones de la inspección (completadas)

1. **La rama de error de la reserva es el problema más sólido.** Dato: la heurística (#3, #6) y el recorrido cognitivo de T3 coinciden en que «Cambiar horario» borra hora y modalidad (H2, confianza «Confirmado»). Interpretación: el estudiante no tiene motivo para volver a elegir «Virtual», así que puede confirmar una tutoría presencial sin notarlo (error silencioso). Acción: B1, ya implementado en la v2. Límite: falta ver cuántos de P01–P05 caen en el error.
2. **Dos necesidades reales no tienen ruta en la v1.** Dato: no hay forma de cancelar o reprogramar una tutoría confirmada o pendiente (H3) ni de elegir otro día (H4). Interpretación: son problemas de validación, no solo de usabilidad: la app hace bien lo especificado, pero no cubre lo que el estudiante necesita. Acción: B3 y B4 en la v2. Límite: T5 y T2 con usuarios dirán cuánto pesa cada uno.
3. **La accesibilidad tiene una barrera medible.** Dato: la etiqueta «Ocupado» tiene un contraste aproximado de 1,5:1 (meta 4,5:1) y la hoja de detalle no se cierra con Esc. Interpretación: H6 y H9 afectan a quien ve con dificultad o usa teclado. Acción: B5 y B8; en la v2 «Ocupado» llega a 6,1:1 y axe-core no reporta violaciones en siete estados. Límite: falta la prueba con lector de pantalla.
4. **La v1 tiene aciertos que se conservan.** Feedback inmediato («Continuar con 10:00»), estados de carga, Resumen antes de confirmar y horarios con texto, no solo color.
5. **Resultado de la inspección:** 10 hallazgos (4 mayores, 5 menores, 1 cosmético); 9 tienen su cambio en el prototipo v2 y 1 (H5) queda fuera porque depende del backend.

## 2. Conclusiones con datos de usuarios (realización del APE 6)

Se completan con lo medido en P01–P05. Ningún número se escribe antes de medirlo.

1. **Reserva (T2):** __ de 5 completaron la reserva sin ayuda (mediana __ s, meta ≤ 90 s). _Interpretación:_ ____ . _Acción:_ ____ .
2. **Recuperación de errores (T3):** __ de 5 corrigieron la hora sin perder la modalidad (mediana __ s). La heurística y el recorrido cognitivo explican la causa (H2). Acción: B1. Con n = 5, el resultado orienta el rediseño, pero no es generalizable a toda la UTA.
3. **Gestión (T5):** __ de 5 lograron cancelar o reprogramar. _Interpretación:_ H3. _Acción:_ B3.
4. **Satisfacción:** SUS medio __ (mín __, máx __; n = 5). _Interpretación respecto a 68:_ ____ .

## 3. Comparación v1 → v2 (después de volver a probar)

| Tarea | Métrica | v1 (medido) | v2 (medido) | ¿Mejoró? |
| --- | --- | --- | --- | --- |
| T3 | Éxito | | | |
| T3 | Mediana de tiempo | | | |
| T5 | Éxito | | | |

Las mejoras esperadas son predicciones hasta que se miden en la v2.

## Limitaciones

- Solo se evaluó el rol estudiante; el prototipo usa datos de ejemplo y no tiene backend.
- El contraste de la v1 se midió sobre capturas (aproximado); se confirma con el analizador en la app.
- Muestra prevista pequeña (5 participantes) de un solo campus.
- El think-aloud concurrente puede alargar los tiempos.

## Aprendizajes del equipo

- La inspección encuentra rápido y barato, pero no dice cuánto pesa cada problema: para eso están los usuarios.
- Dos métodos que coinciden (H2, H6) dan más confianza que un hallazgo visto por uno solo.
- Separar metas de resultados evita «maquillar» la evaluación.
