# Plan de evaluación — Tutoría Fácil UTA

APE 6 · Fase 1 · Grupo 5 · Paralelo B
Marco de planificación: DECIDE (Rogers, Sharp y Preece).

## 1. Contexto y producto

| Campo | Valor |
| --- | --- |
| Producto | Tutoría Fácil UTA — app móvil para buscar docentes por materia, reservar tutorías presenciales o virtuales y gestionarlas |
| Versión evaluada | v1 · prototipo navegable de alta fidelidad en Figma Make |
| Enlace | Ver [Prototipo/README.md](../../README.md) |
| Rol evaluado | Estudiante |
| Fuera de alcance | Roles docente y administrador (no existen en el prototipo); datos reales y backend |
| Tipo de evaluación | Formativa · mixta (cuantitativa + cualitativa) · moderada presencial · laboratorio ligero |

## 2. Objetivos y preguntas de investigación

**Objetivo general:** determinar si estudiantes de la UTA pueden buscar, reservar y gestionar una tutoría en Tutoría Fácil con eficacia, eficiencia y satisfacción, e identificar los problemas que lo impiden para priorizar la versión 2.

| ID | Objetivo específico | Pregunta de investigación | Tareas / instrumento |
| --- | --- | --- | --- |
| O1 | Medir la eficacia y eficiencia del flujo de reserva | PI1 ¿Qué % completa la reserva sin ayuda y en cuánto tiempo? | T1, T2 · hoja + cronómetro |
| O2 | Evaluar la recuperación ante errores | PI2 ¿Pueden corregir hora o modalidad desde el Resumen sin perder datos? | T3 · observación |
| O3 | Evaluar la gestión de tutorías existentes | PI3 ¿Encuentran lugar y estado, y pueden cancelar o reprogramar? | T4, T5 · observación |
| O4 | Valorar satisfacción y accesibilidad básica | PI4 ¿Qué puntaje SUS obtiene? ¿Cumple contraste y teclado de WCAG 2.2 AA? | SEQ, SUS · checklist WCAG |

## 3. Participantes

- **Perfil:** estudiante de la UTA, cualquier carrera y semestre, usa smartphone a diario y ha necesitado o podría necesitar una tutoría.
- **Muestra:** P00 (piloto) + P01–P05 (evaluación). Al menos 2 de carreras distintas a Software.
- **Inclusión:** mayor de edad; acepta el consentimiento; no ha usado este prototipo.
- **Exclusión:** integrantes del G5 o personas que diseñaron la app; estudiantes con experiencia en diseño UX o Figma.
- **Justificación del tamaño:** evaluación formativa de un solo perfil; con ~5 usuarios aparecen la mayoría de problemas frecuentes (Nielsen y Landauer, 1993). No se generalizan métricas cuantitativas.
- **Reclutamiento:** invitación verbal en la FISEI y biblioteca; ~20 min; sin compensación económica.

| Código | Carrera | Semestre | Uso del celular al día | Fecha de sesión |
| --- | --- | --- | --- | --- |
| P00 (piloto) | | | | |
| P01 | | | | |
| P02 | | | | |
| P03 | | | | |
| P04 | | | | |
| P05 | | | | |

## 4. Escenario y tareas

Ver [tareas.md](tareas.md).

## 5. Métricas y metas

Ver [metricas.md](metricas.md).

## 6. Métodos e instrumentos

| ID | Método | Tipo | Instrumento | Archivo |
| --- | --- | --- | --- | --- |
| M1 | Evaluación heurística (Nielsen) | Inspección | Lista de 10 heurísticas + severidad | `Fase3_Metodos/heuristica-nielsen.md` |
| M2 | Recorrido cognitivo de T3 | Inspección | 4 preguntas por paso | `Fase3_Metodos/recorrido-cognitivo-T3.md` |
| M3 | Prueba con usuarios + think-aloud + SEQ/SUS | Empírico | Hoja de observación, cronómetro, cuestionarios | `Fase3_Metodos/observacion.csv`, `sus.csv` |
| M4 | Revisión de accesibilidad WCAG 2.2 AA | Normativo | Checklist + axe/WAVE/Lighthouse + lector de pantalla | `Fase3_Metodos/accesibilidad-wcag.md` |

## 7. Roles y guion

Ver [guion-facilitador.md](guion-facilitador.md).

## 8. Ética

Ver [consentimiento.md](consentimiento.md). Principios: voluntariedad, anonimato (P0X), minimización de datos, grabación solo de pantalla con permiso explícito, finalidad académica.

## 9. Logística

| Campo | Valor |
| --- | --- |
| Lugar | Aula o biblioteca FISEI _(completar)_ |
| Fecha(s) | _(completar)_ |
| Dispositivo | Celular con el enlace de Figma Make abierto en vista móvil |
| Duración por participante | ~20 min |
| Materiales | Tarjetas de tareas, consentimiento, hoja de observación digital, cuestionario SUS |
| Reinicio entre participantes | Recargar el enlace del prototipo |

## 10. Registro y análisis previsto

- Registro por tarea en `observacion.csv` (resultado, tiempo, errores, ayudas, SEQ, emoción observada, frase textual).
- Tasa de éxito por tarea = (É + 0,5·P) ÷ intentos; tiempo como mediana y rango; SUS con media, mínimo y máximo.
- Hallazgos consolidados en la matriz con severidad 0–4, triangulados entre M1–M4 y convertidos en backlog.
