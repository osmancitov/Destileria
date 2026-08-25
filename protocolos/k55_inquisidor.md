# Inquisidor
*Mega-Mapa de Hechos*

## Definición

Un **inquisidor** es el expediente narrativo completo de un corpus: todo lo que ocurre, quién lo hace, con qué consecuencia, en qué orden. No interpreta. No jerarquiza. No omite. Es el documento que permite a quien no ha leído el corpus saber exactamente qué contiene, capítulo por capítulo, bloque por bloque, sin excepción.

El criterio rector es la exhaustividad. Si algo ocurre en el corpus, entra en el inquisidor. La selección editorial no existe aquí.

Operas en español independientemente del idioma del corpus.

---

## Fase 1 — Reconocimiento del corpus

Antes de registrar una sola línea, realizas un reconocimiento completo. Esta fase produce un informe que el operador debe confirmar antes de que comience el registro.

### 1a. Umbral de tamaño

Estima el total de palabras del corpus.

- Si el corpus supera las **60.000 palabras**, el registro no puede ejecutarse en una sola pasada sin riesgo de pérdida de detalle por saturación de contexto. El umbral considera no solo el corpus entrante sino el output acumulado y el propio protocolo, que también ocupan ventana.
- En ese caso, propone al operador el número de bloques recomendados. El tamaño ideal por bloque es de **60.000 palabras**; se tolera hasta **75.000** si el punto de corte narrativamente más limpio cae en ese rango. Por encima de 75.000 por bloque, se recomienda añadir un bloque más aunque resulten bloques más pequeños —bloques pequeños no tienen costo, solo producen sesiones más cortas e independientes entre sí.
- Para cada punto de corte propuesto, indica **dónde cortar exactamente** —entre qué unidades— y justifica brevemente por qué ese punto es narrativamente limpio: ninguna trama abierta cruza el borde, ningún episodio queda partido.
- Todas estas recomendaciones son propuestas: el operador tiene la última palabra sobre cuántos bloques hacer y dónde cortar. El sistema espera confirmación antes de proceder.
- Si el corpus está dentro del umbral, continúa a 1b.

### 1b. Inventario de unidades

Recorre el corpus completo de principio a fin. Identifica **toda unidad textual con título, encabezado o separación visible**, independientemente de cómo se llame. No te guíes por la etiqueta —guíate por la presencia de una separación estructural.

Clasifica cada unidad en una de estas categorías:

- **Capítulo declarado** — el corpus lo llama explícitamente capítulo, sección, parte o equivalente.
- **Paratexto funcional** — bloque que no se llama capítulo pero que contiene información narrativa, argumental o contextual relevante: prólogos, dedicatorias con contenido propio, notas del autor, epílogos, colofones, advertencias al lector. Puede contener hechos, personajes, declaraciones de intención o ficciones sobre el propio texto.
- **Paratexto ornamental** — bloque que no aporta contenido narrativo ni argumental: índices, tablas de contenido, listas de ilustraciones, páginas de derechos, poemas laudatorios sin contenido propio.

Para cada unidad de las dos primeras categorías, entrega:

**[Título o encabezado de la unidad] — [Categoría]**
*Recomendación:* una o dos oraciones que explican si conviene incluirla en el registro y por qué. Si es paratexto funcional, especifica qué tipo de contenido relevante contiene. Si es paratexto ornamental, lo declara brevemente.

### 1c. Estimación del output

Con base en el inventario, estima:

- Número total de unidades a registrar (según la recomendación del sistema)
- Extensión estimada del registro en palabras

La extensión del registro no tiene radio fijo: está determinada por el corpus. Un capítulo breve puede producir 150 palabras de registro; uno denso con múltiples tramas y personajes puede producir 600 o más. El sistema estima a partir de la densidad narrativa observada en la muestra.

### 1d. Confirmación del operador

El sistema presenta el informe completo de la Fase 1 —inventario de unidades con recomendaciones, propuesta de bloques y puntos de corte si aplica, estimación de output— y **espera confirmación antes de proceder**. Todo lo presentado son recomendaciones: el operador tiene la última palabra sobre qué entra, qué se excluye y cómo se secciona el corpus.

El operador puede en este momento:
- Confirmar el plan tal como está
- Excluir unidades específicas (por ejemplo: "omitir todos los paratextos ornamentales")
- Incluir unidades que el sistema recomendó excluir
- Modificar el alcance (por ejemplo: "registrar solo los capítulos I al XXV")
- Ajustar los puntos de corte propuestos

El sistema no inicia el registro hasta recibir confirmación explícita.

---

## Fase 2 — El registro

Una vez confirmado el plan, el sistema procede unidad por unidad en el orden original del corpus.

### Formato de cada unidad

---

**[Título exacto de la unidad tal como aparece en el corpus]**
*[Categoría: Capítulo declarado / Paratexto funcional]*

[Registro en prosa continua]

---

### Principios del registro

**Exhaustividad.** Todo lo que ocurre entra. No hay hecho menor, no hay personaje secundario ignorado, no hay conversación omitida por parecer redundante. Si ocurrió en el corpus, está en el registro.

**Prosa funcional.** El registro se escribe en prosa clara, densa en información, sin ornamento. El estilo está al servicio del registro, no al revés. No se imita el estilo del corpus —se reporta su contenido.

**Orden original.** Los hechos se registran en el orden en que ocurren en el corpus. No se reorganiza por personaje, por tema ni por importancia.

**Personajes con nombre.** Cada vez que aparece un personaje, se lo nombra. Si el corpus no le da nombre, se lo identifica por su función o descripción ("el ventero", "la doncella sin nombre", "el clérigo"). No se usan pronombres ambiguos que puedan confundir quién hace qué.

**Causas y consecuencias.** No basta registrar que algo ocurre —se registra por qué ocurre y qué produce. El registro conecta los hechos.

**Tramas abiertas y cerradas.** Al final de cada unidad, si una trama queda sin resolver, se declara: *[Trama abierta: X]*. Cuando una trama abierta de una unidad anterior se resuelve, se declara: *[Resuelve: X]*.

**Episodios interpolados.** Si el corpus contiene narraciones dentro de la narración —una historia que un personaje cuenta, una novela intercalada, un relato enmarcado— se registra completa, marcando su inicio y cierre: *[Inicio de episodio interpolado: título o descripción]* / *[Cierre del episodio interpolado]*.

**Diálogos con contenido.** Los diálogos que contienen información narrativa relevante —decisiones, revelaciones, conflictos, acuerdos— se registran en forma indirecta pero con precisión: quién dice qué a quién, y qué produce ese intercambio. Los diálogos puramente ornamentales se condensan en una línea.

**Sin interpretación.** El registro no evalúa, no juzga, no interpreta. No dice "en este capítulo Cervantes explora la locura" —dice qué hace don Quijote, qué dicen los otros personajes, qué ocurre como consecuencia.

---

## Señales de que algo salió mal

- Una unidad del inventario confirmado no aparece en el registro.
- Un personaje nombrado en el corpus no aparece en el registro de la unidad donde actúa.
- El registro dice "entre otras cosas" o "varios eventos" sin especificarlos.
- Se usa interpretación o juicio de valor en lugar de reporte de hechos.
- Una trama abierta en una unidad anterior se resuelve sin que el registro lo declare.
- El registro imita el estilo del corpus en lugar de reportar su contenido.
- Se omite un episodio interpolado o se lo menciona sin registrarlo completo.

---

## Resultados

El registro se presenta en un archivo .md, una sección por unidad, en el orden original del corpus.
