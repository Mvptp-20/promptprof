# Prompt Professor — Edición de Auditoría
**Un auditor de prompts de IA estricto. No es un generador de contenido — es un coach.**
*Creado por Victoria + Claude · Kindred Ink · Est. MMXXV*

---

## Qué Es

Prompt Professor es una herramienta HTML de un solo archivo que audita instrucciones (prompts) para IA y te da retroalimentación con puntuación y pasos concretos. Envías el prompt que quieres mejorar; el Profesor lo analiza, lo puntúa y te dice exactamente qué cambiar. Iteras hasta llegar a 10/10.

No es un generador de contenido. No ejecutará tu prompt, no escribirá tu correo ni generará tu informe. Lo que sí hará es mejorar drásticamente la instrucción que le das a tus herramientas de IA.

---

## Para Quién Es

- Cualquier persona que use herramientas de IA regularmente y quiera resultados más consistentes y de mayor calidad
- Investigadores, consultores y equipos de ONG que redactan prompts complejos o sensibles
- Quienes preparan prompts para contextos médicos, legales o regulados
- Principiantes que no saben por dónde empezar a construir un prompt desde cero

---

## Cómo Usarlo

### Opción 1 — Abrir directamente en el navegador
Descarga el archivo `.html` y haz doble clic. No requiere instalación.

### Opción 2 — Publicarlo en línea (Netlify, GitHub Pages u otro hosting estático)
Sube el archivo tal cual. La herramienta llama a un proxy backend en `kindredink-backend.onrender.com` — ninguna clave API queda expuesta en el archivo.

---

## Modos

| Modo | Qué hace |
|---|---|
| **Auditar mi prompt** | Puntúa un prompt existente y entrega retroalimentación estructurada |
| **Ayúdame a construir uno** | Hace preguntas de clarificación y construye un prompt contigo desde cero |
| **Modo Médico / Legal** | Igual que Auditoría, pero el peso de Ética sube al 40% para detectar sesgos, riesgos de responsabilidad y alucinaciones |

---

## Rúbrica de Puntuación

Cada prompt se puntúa en una escala de 1 a 10 usando tres dimensiones ponderadas:

| Dimensión | Peso Estándar | Peso Médico/Legal | Qué mide |
|---|---|---|---|
| **Claridad** | 40% | 30% | Verbo de acción presente, contexto definido, formato de salida especificado |
| **Precisión** | 40% | 30% | Límites de palabras/tokens, casos extremos contemplados, restricciones claras |
| **Ética** | 20% | 40% | Sin sesgos, sin riesgo de alucinación, sin contenido protegido por derechos de autor |

---

## Qué Recibes en Cada Auditoría

Cada auditoría entrega:

- **Puntuación general** (1–10)
- **Puntuaciones individuales** de Claridad, Precisión y Ética
- **Una fortaleza específica** con justificación
- **Una debilidad específica** con justificación
- **Un ejemplo concreto de reescritura** que corrige la debilidad principal
- **Un próximo paso** — la única acción que más mejorará tu puntuación

Itera hasta que el Profesor marque tu prompt como perfecto.

---

## Causas de Rechazo

El Profesor rechazará procesar un prompt que:

- Intente que ejecute contenido en lugar de auditarlo
- Contenga estereotipos, incluso implícitos
- Solicite predicciones futuras presentadas como hechos
- Pida contenido ilegal
- Contenga material protegido por derechos de autor reproducido textualmente

---

## Detalles Técnicos

| Detalle | Valor |
|---|---|
| Tipo de archivo | Archivo `.html` único — sin dependencias ni proceso de compilación |
| Modelo de IA | Claude Sonnet (vía proxy backend de Kindred Ink) |
| Backend | Proxy Node.js en Render (`kindredink-backend.onrender.com`) |
| Clave API | Gestionada en el servidor — no se expone en el archivo |
| Memoria de sesión | El historial de conversación se mantiene dentro de la sesión; se reinicia con "Iniciar nueva sesión" |
| Uso sin conexión | No compatible — requiere conexión a internet para llamar a la API |

---

## Limitaciones

- La herramienta requiere conexión a internet activa; no puede funcionar sin ella.
- El historial de sesión está en memoria — cerrar la pestaña borra la conversación.
- El backend está alojado en el nivel gratuito de Render; los arranques en frío pueden causar un retraso de 10–20 segundos en la primera solicitud después de un período de inactividad.
- La herramienta audita prompts — no enseña conceptos generales de IA ni responde preguntas sobre herramientas de IA.

---

## Archivos de Este Producto

| Archivo | Descripción |
|---|---|
| `promptprof_fixed_v7.html` | Versión en inglés |
| `promptprof_es_v7.html` | Versión en español |

---

## Licencia y Autoría

**Dirigido por humanos — Asistido por IA** bajo la marca Kindred Ink.
Esta herramienta fue diseñada, estructurada e iterada por una persona. La IA asistió en la generación y refinamiento del código.
No está permitida su redistribución ni reventa sin autorización.

---

*¿Preguntas? Escríbenos a través de Gumroad o al correo en tu recibo de compra.*
