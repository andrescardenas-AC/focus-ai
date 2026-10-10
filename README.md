# Focus AI

Instrumento de visión por computador que mide **señales faciales observables**
—apertura ocular (EAR), posición del iris y postura aproximada de la cabeza—
con una cámara web, de forma local y sin guardar video.

> **Focus AI no mide la atención ni diagnostica.** Describe lo que se ve en el rostro
> y está diseñado para comprobar si esas medidas son estables antes de interpretarlas.

## Estado
Herramienta de investigación **en desarrollo**. Todavía no hay resultados con
participantes: la captura empieza solo con el aval del comité de ética.
Este repositorio no contiene datos personales.

## Cómo funciona
1. Cada fotograma se procesa en memoria con MediaPipe Face Mesh (478 puntos) y se descarta.
2. Se guardan solo indicadores numéricos por fotograma (CSV) y metadatos de la sesión.
3. Las reglas que definen un evento (p. ej., cierre ocular ≥ 400 ms) se aplican después
   y se pueden ajustar sin repetir la captura.
4. El análisis calcula la fiabilidad entre sesiones (ICC, CV, Bland–Altman) y genera
   informes en CSV, Excel y PDF.

## Equipo
Andrés Santiago Cárdenas González · David Santiago Quiroga Orjuela · Olmos Orlando Araque  
Tutora: Zalma Valentina Moreno Galeano  
Semillero de Investigación SYNTHESIS · Ingeniería de Datos e IA  
Universidad Santo Tomás, seccional Tunja

Presentado en el I Encuentro Virtual de Semilleros de Investigación en IA,
Semana Tomasina 2026 (14 de octubre).

## Contacto
andres.cardenasg@usantoto.edu.co

## Cómo citar
Cárdenas González, A. S., Quiroga Orjuela, D. S., Araque, O. O., y Moreno Galeano, Z. V.
(2026). *Focus AI: visión por computador aplicada al análisis de comportamientos
observables en entornos universitarios* [Software en desarrollo]. Semillero SYNTHESIS,
Universidad Santo Tomás, Tunja.

El código fuente se publicará en este repositorio más adelante.
