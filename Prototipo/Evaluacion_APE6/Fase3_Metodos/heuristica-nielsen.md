# M1 · Evaluación heurística (Nielsen)

**Objeto:** Tutoría Fácil UTA v1 (Figma Make) · rol estudiante
**Fecha de inspección:** 10/11/2026 · **Evaluadores:** equipo G5 · **Estado:** completada (10 hallazgos, 6 aciertos)
**Procedimiento:** 2 pasadas por T1–T5 (flujo y detalle) → anotar pantalla, problema, heurística y evidencia → consolidar duplicados → severidad 0–4 por consenso.

## Heurísticas de referencia

1. Visibilidad del estado del sistema
2. Coincidencia entre el sistema y el mundo real
3. Control y libertad del usuario
4. Consistencia y estándares
5. Prevención de errores
6. Reconocer antes que recordar
7. Flexibilidad y eficiencia de uso
8. Diseño estético y minimalista
9. Ayudar a reconocer, diagnosticar y recuperarse de errores
10. Ayuda y documentación

## Hallazgos

| ID | Pantalla | Problema | Pasos para reproducir | Heurística | Sev.* | Evidencia |
| --- | --- | --- | --- | --- | --- | --- |
| H1 | Inicio → Materias | El buscador dice «Buscar materia o docente», pero un apellido de docente visible en Inicio («Ramos») devuelve «Sin resultados», sin sugerencias | Inicio › escribir «Ramos» › Buscar | #4 · #9 | 3 | [14_H1_busqueda_docente_sin_resultados.jpg](../../v1_capturas/14_H1_busqueda_docente_sin_resultados.jpg) |
| H2 | Resumen → Seleccionar horario | «Cambiar horario» vuelve sin hora marcada y con «Presencial»: se pierde lo elegido | Reservar 10:00 Virtual › Continuar › Cambiar horario | #3 · #6 | 3 | [08_resumen.jpg](../../v1_capturas/08_resumen.jpg) → [09_H2_cambiar_horario_pierde_seleccion.jpg](../../v1_capturas/09_H2_cambiar_horario_pierde_seleccion.jpg) |
| H3 | Mis tutorías → Detalle | Una tutoría Confirmada o Pendiente solo ofrece «Cerrar»; no se puede cancelar ni reprogramar | Mis tutorías › Base de Datos | #3 · #4 | 3 | [11_H3_detalle_pendiente_solo_cerrar.jpg](../../v1_capturas/11_H3_detalle_pendiente_solo_cerrar.jpg) |
| H4 | Seleccionar horario | Se muestra un único día fijo (jueves 8 de octubre de 2026); no encontramos cómo elegir otra fecha | Cualquier docente › Ver horarios | #3 · #7 | 3 | [05_horario_sin_seleccion.jpg](../../v1_capturas/05_horario_sin_seleccion.jpg) |
| H5 | Docentes / Inicio / Mis tutorías | La tarjeta dice «Próximo: Mañana, 09:00» y en horarios las 09:00 aparecen «Ocupado»; Inicio muestra 3 próximas y Mis tutorías lista 4 | Comparar pantallas | #1 · #4 | 2 | [04_docentes_programacion.jpg](../../v1_capturas/04_docentes_programacion.jpg), [10_mis_tutorias.jpg](../../v1_capturas/10_mis_tutorias.jpg) |
| H6 | Seleccionar horario | Tocar un horario «Ocupado» no produce ninguna respuesta; el texto gris muy claro podría no cumplir contraste | Tocar 09:00 | #1 · WCAG 1.4.3 (≈ 1,5:1 medido, ver M4) | 2 | [05_horario_sin_seleccion.jpg](../../v1_capturas/05_horario_sin_seleccion.jpg) |
| H7 | Resumen | No se puede indicar el tema o la duda; el docente no sabe qué preparar | Llegar al Resumen | #2 (validación) | 2 | [08_resumen.jpg](../../v1_capturas/08_resumen.jpg) |
| H8 | Detalle reprogramada → Horario | Al reprogramar una tutoría virtual de 09:00 se preseleccionan 14:00 y «Presencial»; «atrás» dice «Ingeniería de Software» aunque se venía de Mis tutorías | Mis tutorías › Ingeniería de Software › Reprogramar | #4 · #6 | 2 | [12_detalle_reprogramada.jpg](../../v1_capturas/12_detalle_reprogramada.jpg) → [13_H8_reprogramar_preseleccion.jpg](../../v1_capturas/13_H8_reprogramar_preseleccion.jpg) |
| H9 | Detalle (hoja inferior) | La hoja no se cerró con Esc en nuestra revisión (a verificar con Tab) | Abrir detalle › Esc | WCAG 2.1.1 | 2 | Prueba con teclado |
| H10 | Detalle pendiente | «Pendiente» no explica qué significa ni qué debe hacer el estudiante | Mis tutorías › Base de Datos | #10 · #1 | 1 | [11_H3_detalle_pendiente_solo_cerrar.jpg](../../v1_capturas/11_H3_detalle_pendiente_solo_cerrar.jpg) |

\*Severidad por consenso del equipo a partir de la inspección; se revisa con los datos de P01–P05.

**Resumen:** 4 mayores (H1–H4) · 5 menores (H5–H9) · 1 cosmético (H10). Todos menos H5 tienen su cambio en el [prototipo v2](../../v2_propuesta/prototipo-v2.html).

## Aciertos (se conservan en la v2)

- «Continuar» deshabilitado hasta elegir hora; luego dice «Continuar con 10:00» (#1, #5) — [06_horario_10h_virtual.jpg](../../v1_capturas/06_horario_10h_virtual.jpg)
- Estados de carga «Consultando horarios…» / «Verificando…» (#1) — [07_estado_carga.jpg](../../v1_capturas/07_estado_carga.jpg)
- Resumen antes de confirmar (#5).
- Horarios con texto, no solo color (WCAG 1.4.1).
- Barra inferior consistente con foco visible (#4, WCAG 2.4.7).
- Estado vacío «Sin resultados» presente (aunque sin sugerencias).
