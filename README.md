# IHC · Grupo 5 · APE 6 — Evaluación y validación de **Tutoría Fácil UTA**

**Universidad Técnica de Ambato · FISEI · Carrera de Software**
Interacción Humano–Computador · 5.º nivel · Paralelo B · Unidad Evaluativa II · 2026

| Dato | Valor |
| --- | --- |
| Tema asignado (matriz) | Evaluación y validación + métodos de evaluación |
| APE | APE 6 completo – Fases 1 a 4 (grupo referente) |
| Objeto evaluado | Prototipo navegable **Tutoría Fácil UTA** (Figma Make) |
| Exposición | Una sola, de 118 minutos: Parte 1 tema general + Parte 2 Guía APE 6 |
| Para los grupos | 8 actividades de 3 min dentro de la exposición, ronda de preguntas en modo juego y taller general en Word (1 h) |
| Evidencias | [Prototipo/Evaluacion_APE6/EVIDENCIAS.md](Prototipo/Evaluacion_APE6/EVIDENCIAS.md) |


## Responsabilidad según la matriz (5B · G5)

- **Responsabilidad:** construir el APE 6 completo como grupo referente: planificación, pilotaje, aplicación de métodos, análisis, priorización y cierre.
- **Implementación obligatoria:** diseñar la evaluación, pilotear tareas, aplicar al menos 2 métodos, registrar métricas, triangular resultados y construir backlog de mejoras.
- **Evidencia:** plan + consentimiento + tareas + datos + matriz de hallazgos + severidad + backlog + presentación final del APE 6.

## Qué está hecho

| Componente | Resultado | Dónde |
| --- | --- | --- |
| Plan, tareas, métricas, guion y consentimiento | Completos | `Prototipo/Evaluacion_APE6/Fase1_Planificacion` |
| Métodos de inspección | Heurística (10 hallazgos), recorrido cognitivo de T3 y WCAG 2.2 AA (contraste medido) | `Fase3_Metodos` |
| Análisis | Matriz con severidad, triangulación (H2 y H6 confirmados), backlog B1–B10 y conclusiones | `Fase4_Analisis` |
| Prototipo | 14 capturas de la v1 · **prototipo v2 navegable con 9 mejoras** · 9 capturas de la v2 · maqueta v1 → v2 | `Prototipo/v1_capturas` · `Prototipo/v2_propuesta` |
| Pilotaje con P00 | Se hace en vivo durante la exposición (láminas 65–66) | `Fase2_Pilotaje` |
| Prueba con P01–P05 y SUS | Se hace el día 2, en la realización del APE 6 | `observacion.csv` · `sus.csv` |

## Estructura del repositorio

```
.
├── README.md                     ← este archivo
├── .gitignore
├── Actividades/                  ← para los grupos G1–G4
│   ├── README.md
│   ├── Taller_APE6_General.docx  ← taller general de 1 hora (Word, lo completa cada grupo)
│   ├── Parte1_Tema_General/      ← A1 – A4 (3 min, dentro de la exposición)
│   └── Parte2_Guia_APE6/         ← B1 – B4 (3 min, dentro de la exposición)
├── Presentacion/
│   ├── README.md
│   ├── G5_Exposicion_APE6.html   ← exposición única (Parte 1 + Parte 2, 118 min)
│   └── G5_Preguntas_APE6.html    ← preguntas por grupos en modo juego
└── Prototipo/                    ← prototipo evaluado y su evaluación
    ├── README.md
    ├── Evaluacion_APE6/          ← entregables por fase + EVIDENCIAS.md
    ├── v1_capturas/              ← 14 capturas de la v1
    └── v2_propuesta/             ← prototipo-v2.html, capturas y maqueta v1 → v2
```

## Cómo abrir cada cosa

| Qué | Dónde | Cómo |
| --- | --- | --- |
| Prototipo evaluado (v1) | [Prototipo/README.md](Prototipo/README.md) | Enlace a Figma Make; abrir en el celular o en vista móvil |
| Prototipo v2 | [Prototipo/v2_propuesta/prototipo-v2.html](Prototipo/v2_propuesta/prototipo-v2.html) | Doble clic; botón «Probar» por cada mejora |
| Exposición | [Presentacion/G5_Exposicion_APE6.html](Presentacion/G5_Exposicion_APE6.html) | ←/→ navegar · N notas · M índice · F pantalla completa |
| Preguntas por grupos | [Presentacion/G5_Preguntas_APE6.html](Presentacion/G5_Preguntas_APE6.html) | Nombres de grupo editables, **Iniciar partida** y puntaje automático |
| Actividades de 3 min | [Actividades/README.md](Actividades/README.md) | A1–A4 (Parte 1) y B1–B4 (Parte 2), con aviso previo |
| Taller general (1 h) | [Actividades/Taller_APE6_General.docx](Actividades/Taller_APE6_General.docx) | Word que completa cada grupo con su propio proyecto |
| Evidencias del APE 6 | [Prototipo/Evaluacion_APE6/EVIDENCIAS.md](Prototipo/Evaluacion_APE6/EVIDENCIAS.md) | Índice con estado y lámina de cada evidencia |

## Trazabilidad (completar con enlaces reales)

| Elemento | Enlace |
| --- | --- |
| Plan de evaluación | [plan-evaluacion.md](Prototipo/Evaluacion_APE6/Fase1_Planificacion/plan-evaluacion.md) |
| Tareas T1–T5 | [tareas.md](Prototipo/Evaluacion_APE6/Fase1_Planificacion/tareas.md) |
| Consentimiento | [consentimiento.md](Prototipo/Evaluacion_APE6/Fase1_Planificacion/consentimiento.md) |
| Ajustes del piloto | [ajustes-piloto.md](Prototipo/Evaluacion_APE6/Fase2_Pilotaje/ajustes-piloto.md) |
| Datos de observación | [observacion.csv](Prototipo/Evaluacion_APE6/Fase3_Metodos/observacion.csv) |
| Matriz de hallazgos | [matriz-hallazgos.md](Prototipo/Evaluacion_APE6/Fase4_Analisis/matriz-hallazgos.md) |
| Backlog priorizado | [backlog.md](Prototipo/Evaluacion_APE6/Fase4_Analisis/backlog.md) |
| Prototipo v2 | [prototipo-v2.html](Prototipo/v2_propuesta/prototipo-v2.html) |

## Reglas de trabajo

- Cada integrante: Issue asignada, rama propia, commits con cambios sustantivos y revisión cruzada en el PR.
- No se suben datos personales de participantes: solo códigos P00–P05.
- Las metas del plan son hipótesis; los resultados se reportan con los datos medidos, aunque no cumplan la meta.
- Mantener intactas las entregas de APE anteriores.
# IHC-G5-APE6-Evaluacion-Validacion
