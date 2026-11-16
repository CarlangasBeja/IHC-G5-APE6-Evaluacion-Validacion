# Matriz de hallazgos con severidad

**Estado:** completada con la evidencia de inspección (M1, M2 y M4). La revisión de severidad con datos de P01–P05 se hace en la realización del APE 6 (tabla al final).

Escala de severidad (Nielsen): 0 no es problema · 1 cosmético · 2 menor · 3 mayor · 4 catástrofe.
Factores: **frecuencia** (a cuántos afecta) · **impacto** (cuánto cuesta superarlo) · **persistencia** (se repite o se aprende a evitar).

Métodos: M1 heurística · M2 recorrido cognitivo · M3 prueba con usuarios · M4 WCAG. En la columna «Evidencia de métodos», ✔ es evidencia ya obtenida y «M3 (T#)» indica la tarea donde se comprobará con usuarios.

| ID | Problema | Evidencia | Principio | Evidencia de métodos | Sev. | Recomendación | Backlog | En la v2 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| H1 | El buscador de Inicio no encuentra docentes | «Ramos» → «Sin resultados» · [captura](../../v1_capturas/14_H1_busqueda_docente_sin_resultados.jpg) | #4 · #9 | M1 ✔ · M3 (T1) | 3 | Buscar también docentes; estado vacío con sugerencias | B2 | [✔](../../v2_propuesta/capturas/02_B2_buscar_docente_Ramos.jpg) |
| H2 | «Cambiar horario» pierde hora y modalidad | [antes](../../v1_capturas/08_resumen.jpg) / [después](../../v1_capturas/09_H2_cambiar_horario_pierde_seleccion.jpg) | #3 · #6 | M1 ✔ · M2 ✔ · M3 (T3) | 3 | Conservar la selección y resaltarla al volver | B1 | [✔](../../v2_propuesta/capturas/05_B1_cambiar_horario_conserva.jpg) |
| H3 | No se puede cancelar ni reprogramar una tutoría confirmada o pendiente | [captura](../../v1_capturas/11_H3_detalle_pendiente_solo_cerrar.jpg) | #3 · #4 | M1 ✔ · M3 (T5) | 3 | «Cancelar» y «Reprogramar» con confirmación en toda tutoría futura | B3 | [✔](../../v2_propuesta/capturas/08_B3_confirmar_cancelacion.jpg) |
| H4 | No hay selector de fecha | [captura](../../v1_capturas/05_horario_sin_seleccion.jpg) | #3 · #7 | M1 ✔ · M3 (T2) | 3 | Selector de días hábiles | B4 | [✔](../../v2_propuesta/capturas/03_B4_B5_selector_dia_y_ocupado.jpg) |
| H5 | Datos inconsistentes entre pantallas | 09:00 «Próximo» vs «Ocupado»; 3 vs 4 tutorías | #1 · #4 | M1 ✔ | 2 | Una sola fuente de datos para horarios y contadores | B6 | — (depende del backend) |
| H6 | «Ocupado» sin respuesta al tocar; contraste bajo | Toque sin efecto · «Ocupado» ≈ 1,5:1 ([M4](../Fase3_Metodos/accesibilidad-wcag.md)) | #1 · 1.4.3 | M1 ✔ · M4 ✔ · M3 (T2) | 2 | Mensaje con la siguiente hora libre; contraste ≥ 4,5:1 | B5 | [✔](../../v2_propuesta/capturas/03_B4_B5_selector_dia_y_ocupado.jpg) |
| H7 | No se indica el tema de la tutoría | [captura](../../v1_capturas/08_resumen.jpg) | #2 | M1 ✔ | 2 | Campo opcional «¿Qué quieres revisar?» | B9 | [✔](../../v2_propuesta/capturas/04_B9_resumen_con_tema.jpg) |
| H8 | Reprogramar no conserva hora ni modalidad; «atrás» confuso | [captura](../../v1_capturas/13_H8_reprogramar_preseleccion.jpg) | #4 · #6 | M1 ✔ | 2 | Partir de la tutoría original; volver a Mis tutorías | B7 | [✔](../../v2_propuesta/capturas/09_B7_reprogramar_preseleccion.jpg) |
| H9 | La hoja de detalle no responde a Esc | Recorrido con teclado | WCAG 2.1.1 | M4 ✔ | 2 | Cerrar con Esc y devolver el foco | B8 | ✔ (Esc, foco retenido y devuelto) |
| H10 | «Pendiente» sin explicación | [captura](../../v1_capturas/11_H3_detalle_pendiente_solo_cerrar.jpg) | #10 | M1 ✔ | 1 | Texto de ayuda: «el docente aún no confirma» | B10 | [✔](../../v2_propuesta/capturas/06_B10_solicitud_enviada.jpg) |

**Resumen:** 10 hallazgos · 4 mayores · 5 menores · 1 cosmético · 9 resueltos en el [prototipo v2](../../v2_propuesta/prototipo-v2.html) · 1 fuera de alcance (H5).

## Severidad: cómo se decidió (inspección)

| ID | Frecuencia esperada | Impacto | Persistencia | Severidad |
| --- | --- | --- | --- | --- |
| H1 | Quien busque por nombre | Obliga a otra ruta (Materias) | Cada vez que busca así | 3 |
| H2 | Quien corrija desde el Resumen | Error silencioso de modalidad | Cada vez | 3 |
| H3 | Quien necesite cancelar | Impide completar T5 | Cada vez | 3 |
| H4 | Quien no pueda el día fijo | Impide reservar otro día | Cada vez | 3 |
| H6 | Quien toque una hora ocupada | Molestia; barrera de lectura | Se aprende a evitar | 2 |

## Revisión de severidad con datos de usuarios (realización del APE 6)

| ID | Participantes afectados (de 5) | Impacto observado | Persistencia | Severidad final | Decidido por |
| --- | --- | --- | --- | --- | --- |
| H1 | | | | | |
| H2 | | | | | |
| H3 | | | | | |
| H4 | | | | | |
| H6 | | | | | |
