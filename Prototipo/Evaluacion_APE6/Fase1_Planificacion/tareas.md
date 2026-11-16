# Escenario y tareas (T1–T5)

**Estado:** completado · se prueba con P00 en el pilotaje en vivo y se aplica a P01–P05 en la realización del APE 6.

**Escenario (se lee al participante):**
«Eres estudiante de la UTA. Tienes examen de Programación la próxima semana y quieres ayuda de un docente. Vas a usar la app Tutoría Fácil desde este celular.»

| ID | Tipo | Consigna (tarjeta del participante) | Criterio de éxito (observable) | Ruta óptima | Meta* |
| --- | --- | --- | --- | --- | --- |
| T1 | Localizar | «Averigua qué docentes de Base de Datos pueden atenderte hoy.» | Llega a la lista de docentes de Base de Datos (o a «Disponibles hoy») y nombra uno | Materias › Base de Datos (2 toques) | ≤ 45 s |
| T2 | Operar | «Reserva una tutoría virtual de Programación con la Msc. Andrea Paola Mendoza a las 10:00.» | Llega al Resumen con docente, 10:00 y Virtual correctos | Reservar tutoría › Programación › Ver horarios › Virtual › 10:00 › Continuar (6 toques) | ≤ 90 s |
| T3 | Corregir y confirmar (rama de error) | «A las 10:00 tienes clase. Cámbiala a las 11:00, sigue siendo virtual, y confírmala.» | Confirma con 11:00 + Virtual. Se registra si tuvo que volver a elegir la modalidad | Cambiar horario › 11:00 › (Virtual) › Continuar › Confirmar | ≤ 60 s |
| T4 | Consultar | «Averigua dónde y a qué hora es tu tutoría de Base de Datos y si ya está confirmada.» | Dice lugar (Lab Informática 2 — Bloque B), hora (16:00) y estado (Pendiente) | Mis tutorías › Base de Datos (2 toques) | ≤ 40 s |
| T5 | Gestionar | «Ya no podrás asistir a tu tutoría de Matemáticas del jueves. Haz lo necesario en la app.» | Cancela o reprograma. Si declara que no puede, se registra como fallo con su explicación | Por definir según la app | ≤ 60 s |

\*Las metas son **hipótesis del equipo** para comparar; no son resultados.

## Reglas de redacción aplicadas

- Motivación realista (escenario) y lenguaje del estudiante, sin revelar la ruta ni las etiquetas de los botones.
- Una sola meta y un final observable por tarea.
- Orden de simple a compleja; T3 depende de T2.
- T5 se mantiene aunque se sospeche que la app no lo permite: las tareas representan necesidades reales, no lo que la app ya hace bien.

## Trazabilidad con el flujo de usuario

- T2 = rama de éxito del flujo de reserva.
- T3 = rama de error y recuperación (corregir desde el Resumen sin perder datos).
- T5 = control y libertad del usuario sobre sus tutorías.

## Códigos de resultado

| Código | Significado |
| --- | --- |
| É | Éxito sin ayuda |
| P | Parcial: falta un dato o recibió 1 ayuda |
| F | Fallo: resultado incorrecto o 2+ ayudas |
| A | Abandono: el participante desiste, o se bloquea más de 60 s sin avanzar y acepta pasar a la siguiente tarea |
