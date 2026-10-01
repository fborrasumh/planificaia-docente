# PlanificaIA Docente

Aplicación web de un solo fichero para que el profesorado de **Planificación del Entrenamiento Deportivo** (Universidad Miguel Hernández de Elche) evalúe por rúbrica los ficheros que exporta [PlanificaIA](https://github.com/fborrasumh/planificaia).

**Usar la app:** https://fborrasumh.github.io/planificaia-docente/

## Qué hace

- **Rúbrica:** incorpora la de la asignatura (12 criterios, niveles 0 a 4) y permite cargar otro documento Word. La IA lo estructura y el código valida que los pesos sumen 100 y que cada descriptor aparezca literalmente en el documento.
- **Estudiantes:** carga varios JSON, los agrupa por correo, avisa de posibles duplicados, recalcula la huella SHA-256 de cada fichero y comprueba el encadenamiento entre hitos. Muestra cambios entre hitos y señales calculadas por código.
- **Evaluación:** la IA propone un nivel por criterio con citas literales; el código descarta las que no aparecen en el trabajo. El profesorado elige el nivel definitivo de cada criterio (no se promedia nada). Modo ciego, aviso de discrepancias de dos o más niveles y notas de la defensa oral aportadas por el profesor.
- **Resultados:** CSV de notas, CSV detallado por criterio, informe Word por estudiante y ZIP con todos; copia de seguridad.

## Privacidad

Los ficheros y las evaluaciones se guardan solo en el navegador. A OpenAI viaja únicamente texto del trabajo con el estudiante como «E01», «E02»…, con nombres y datos personales enmascarados y tras una confirmación previa que muestra lo que sale. No se envían nombres, correos ni grupos.

## Límites

- La IA propone; la evaluación y sus decisiones son del profesorado.
- La huella de integridad es una señal, no una prueba.
- Con criterios sin confirmar, el resultado figura como provisional.

## Autoría y atribución

Realizada entre **Fernando Borrás Rocher** y **Manuel Moya Ramón** (Universidad Miguel Hernández de Elche). La rúbrica incorporada y el modelo de datos proceden del trabajo docente sobre **Entrenamiento 360**, de Manuel Moya Ramón.

## Cómo citar

Borrás Rocher, F. y Moya Ramón, M. (2026). *PlanificaIA Docente* (v1.0.0) [Software]. Universidad Miguel Hernández de Elche. (DOI en trámite)

## Licencia

MIT. Véase [LICENSE](LICENSE).
