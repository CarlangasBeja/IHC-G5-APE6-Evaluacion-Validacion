# M4 · Revisión de accesibilidad — WCAG 2.2 nivel AA

Principios POUR: Perceptible · Operable · Comprensible · Robusto.

**Estado:** revisión de la v1 completada en lo que se puede inspeccionar (capturas y recorrido); revisión automática de la v2 completada con axe-core. Lo que necesita lector de pantalla en el celular se revisa en la realización del APE 6.

## v1 · Tutoría Fácil UTA en Figma Make (inspección 10/11/2026)

| Criterio | Qué revisamos | Estado | Evidencia / medición |
| --- | --- | --- | --- |
| 1.4.1 Uso del color | Los horarios dicen «Disponible / Seleccionado / Ocupado» en texto; los estados de tutoría tienen etiqueta | Cumple | [05_horario_sin_seleccion.jpg](../../v1_capturas/05_horario_sin_seleccion.jpg) |
| 1.4.3 Contraste mínimo (4,5:1) | Texto del horario ocupado | **Bajo** | Etiqueta «Ocupado» ≈ **1,5:1** (texto ≈ #CDCED0 sobre #F9FAFC); hora «09:00» ocupada ≈ **2,2:1** (#A9AAAE). Referencia: hora disponible «08:00» ≈ 9:1 |
| 2.1.1 Teclado | La hoja de detalle no se cerró con Esc (H9) | No cumple | Recorrido con teclado sobre el sitio publicado |
| 2.4.7 Foco visible | La barra inferior muestra contorno de foco | Parcial | Se ve en la barra inferior; no en todos los controles |
| 2.5.8 Tamaño del objetivo (24 × 24 px) | Botones de horario amplios; «×» de la hoja pequeño | Parcial | Estimación visual sobre capturas |
| 1.1.1 Contenido no textual | Fotos de docentes e íconos | Con lector | Se revisa con TalkBack o VoiceOver en la realización |
| 4.1.2 Nombre, función, valor | ¿El lector anuncia «10:00, seleccionado, botón»? | Con lector | Se revisa con TalkBack o VoiceOver en la realización |

**Cómo se midió el contraste:** sobre la captura `05_horario_sin_seleccion.jpg` (440 px de ancho) se tomó el trazo más oscuro del texto (percentil 3 de luminancia) y la mediana del fondo del botón, y se aplicó la fórmula de luminancia relativa de WCAG. Es una **medición aproximada** (la compresión JPG aclara los trazos finos), pero incluso el píxel más oscuro da ≤ 2,7:1, lejos de 4,5:1. Se confirma con el analizador de contraste en la app.

**Nota de criterio:** WCAG 1.4.3 exime el texto de componentes inactivos. El equipo lo trata igual como barrera porque «Ocupado» es información que el estudiante necesita leer para decidir; por eso H6 lleva la recomendación de contraste ≥ 4,5:1.

## v2 · prototipo del G5 (`v2_propuesta/prototipo-v2.html`)

Revisión automática con **axe-core 4.10.2** (reglas WCAG 2.0, 2.1 y 2.2, niveles A y AA) sobre siete estados del prototipo.

| Estado revisado | Violaciones | Reglas superadas | Revisión manual |
| --- | --- | --- | --- |
| Inicio | 0 | 18 | contraste sobre fondos con degradado |
| Búsqueda «Ramos» (B2) | 0 | 18 | contraste sobre fondos con degradado |
| Horario con «Ocupado» (B4, B5) | 0 | 14 | rayado de «Ocupado»: medido a mano |
| Resumen con tema (B9) | 0 | 17 | — |
| Horario conservado (B1) | 0 | 14 | — |
| Mis tutorías + detalle Pendiente (B3, B8, B10) | 0 | 18 | — |
| Reprogramar (B7) | 0 | 14 | — |

| Criterio | Cambio en la v2 | Medición |
| --- | --- | --- |
| 1.4.3 Contraste | «Ocupado» en #4A5566 sobre el rayado #EEF1F5 / #E3E8EF | **6,1:1 a 6,7:1** (calculado con los colores del código) |
| 2.1.1 Teclado | La hoja de detalle se cierra con Esc, retiene el foco con Tab y lo devuelve a la tarjeta (B8) | Probado con teclado (Esc y Tab) |
| 2.5.8 Tamaño del objetivo | Todos los controles del prototipo miden ≥ 24 × 24 px en los diez estados revisados (la menor dimensión es 30 px) | Medido con `getBoundingClientRect` |
| 4.1.2 Nombre, función, valor | Días, modalidad y horas con `aria-pressed`; hoja con `role="dialog"` y `aria-modal`; horas ocupadas con etiqueta «ocupado» | Revisado en el código y con axe |

Las herramientas automáticas detectan solo una parte de los problemas: el resultado «0 violaciones» no equivale a cumplir WCAG 2.2 AA. Falta la prueba con lector de pantalla en el celular.
