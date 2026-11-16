# Triangulación de hallazgos

**Regla:** 3 o más métodos con evidencia = **Alta** · 2 = **Confirmado** · 1 = **A verificar**.
Si los usuarios no sufren un problema que la inspección sí marcó, se discute: puede ser un falso positivo o un perfil no representado en la muestra.

**Estado:** completada con los tres métodos de inspección (M1, M2, M4). La columna M3 se llena con P01–P05 en la realización del APE 6 y la confianza se recalcula.

| Hallazgo | M1 Heurística | M2 Recorrido | M4 WCAG | M3 Usuarios (P01–P05) | Confianza actual |
| --- | --- | --- | --- | --- | --- |
| H1 Buscador no encuentra docentes | ✔ | — | — | _pendiente (T1)_ | A verificar |
| H2 Cambiar horario pierde datos | ✔ | ✔ | — | _pendiente (T3)_ | **Confirmado** |
| H3 No se puede cancelar | ✔ | — | — | _pendiente (T5)_ | A verificar |
| H4 Sin selector de fecha | ✔ | — | — | _pendiente (T2)_ | A verificar |
| H5 Datos inconsistentes | ✔ | — | — | — | A verificar |
| H6 «Ocupado» sin respuesta / contraste | ✔ | — | ✔ (≈ 1,5:1) | _pendiente (T2)_ | **Confirmado** |
| H7 Sin campo de tema | ✔ | — | — | _pendiente (cierre)_ | A verificar |
| H8 Reprogramar no conserva datos | ✔ | — | — | — | A verificar |
| H9 Hoja no responde a Esc | — | — | ✔ | — | A verificar |
| H10 «Pendiente» sin explicar | ✔ | — | — | _pendiente (T4)_ | A verificar |

En la columna M3 escribir «Lo sufrieron X de 5» o «No se observó», y recalcular la confianza.

## Qué cambia en la prioridad

Con dos métodos, **H2** y **H6** suben a «Confirmado» (peso 0,8). Por eso B1 (2,40) y B5 (1,60) encabezan el backlog: Prioridad = severidad × confianza ÷ esfuerzo.
