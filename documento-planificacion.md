# Proyecto Final — Sistema de IA para Posicionamiento de Marca
## Búho — Importadora de artículos de pesca

> **¿Por qué Búho?** El búho representa vista aguda, paciencia y saber
> esperar el momento exacto — las mismas cualidades que hacen a un buen
> pescador. Es un nombre corto, memorable y distinto a los nombres
> genéricos de "río" o "caña" que usa la competencia, lo cual ayuda al
> objetivo de posicionamiento de marca frente a los comercios.

---

## 1. Planificación del Proyecto

### 1.1 Objetivos
- Definir y posicionar la identidad visual y sonora de una nueva marca importadora de artículos de pesca.
- Construir un Sistema de IA (no prompts sueltos) que genere contenido coherente para presentarle la marca a comercios minoristas (B2B).
- Producir activos multimodales (imágenes y audio) alineados a esa identidad.
- Documentar todo el proceso de forma profesional y ética.

### 1.2 Alcance
**Incluye:**
- Definición de identidad de marca (nombre, propuesta de valor, tono).
- Sistema de IA: instrucciones base + prompt maestro.
- Mínimo 3 imágenes (ej: logo/concepto, catálogo de producto, pieza para punto de venta).
- Mínimo 2 audios (ej: spot de presentación B2B, mensaje de marca corto).
- Matriz de ética y auditoría de sesgos/alucinaciones.
- README público con toda la documentación.

**No incluye (fuera de alcance):**
- Desarrollo de sitio web o e-commerce.
- Registro legal de marca o trámites de importación.
- Campaña publicitaria completa multicanal.

### 1.3 Cronograma sugerido
| Fase | Actividad | Duración estimada |
|---|---|---|
| 1 | Co-creación: definir problema, objetivos y cronograma con un LLM | 1 día |
| 2 | Configuración del sistema (instrucciones base + prompt maestro) | 1 día |
| 3 | Producción multimodal (imágenes + audio) | 2-3 días |
| 4 | Auditoría ética | 1 día |
| 5 | Compilación del README y publicación | 1 día |

### 1.4 Criterios de evaluación
- Calidad y coherencia de los prompts (no improvisados, sino sistemáticos).
- Coherencia estética/sonora entre todos los activos generados.
- Documentación clara de parámetros técnicos usados.
- Profundidad de la auditoría ética.
- Presentación final (README completo, prolijo, en URL pública).

---

## 2. Contexto del Proyecto 

> **Marca:** [Buho]
> **Rubro:** Importadora de artículos de pesca (nueva en el mercado)
> **Modelo de negocio:** B2B — le vende a comercios que después venden al público final
> **Objetivo de negocio:** Posicionamiento de marca frente a comercios minoristas, generar confianza y diferenciación frente a otros importadores/distribuidores ya instalados
> **Público objetivo directo:** Dueños/compradores de comercios de pesca y outdoor
> **Público objetivo indirecto:** El consumidor final que compra en esos comercios (la marca debe "verse bien" también en el punto de venta)

**Respuestas de co-creación (fase 1 completada):**
1. **Diferenciación:** precio competitivo + atención cercana y personalizada al comercio (no es "otro importador anónimo", es un socio comercial).
2. **Tono:** aventurero, cercano y humanizado — nada de lenguaje corporativo frío ni genérico de catálogo.
3. **Producto foco:** cañas y reels (línea inicial de importación).



---

## 3. Sistema de IA

### 3.1 Instrucciones Base (System Prompt)

```
Eres el Director Creativo de Búho, una importadora nueva de
cañas y reeles de pesca que vende exclusivamente a comercios minoristas
(modelo B2B).

Tu tono es: aventurero, cercano y humanizado. Hablás como alguien que
también pesca y entiende el negocio del comercio — no como una corporación
distante.

Concepto de marca "Búho": el búho ve en la oscuridad y en los momentos
de calma — como el pescador que sale antes del amanecer o se queda hasta
el último rayo de luz. Usá esta idea como hilo conductor sutil (nunca
literal ni infantil): momentos de calma, primeras luces, atardeceres,
precisión y paciencia.

Tu misión: posicionar a la marca frente a comercios minoristas destacando
DOS pilares centrales:
1. Precio competitivo (buen margen para el comercio).
2. Atención cercana y personalizada (un socio, no un proveedor anónimo).

Reglas de estilo:
- Lenguaje cálido y directo, con espíritu de aventura y aire libre —
  evocá el río, el amanecer, la pesca como pasión compartida — pero sin
  perder profesionalismo ni credibilidad técnica sobre el producto.
- Nunca suenes corporativo, acartonado o genérico de catálogo.
- Resaltá siempre: precio/margen para el comercio, calidad de cañas y
  reeles, y la relación cercana y de confianza con quien compra.
- Coherencia visual: paleta de colores tierra/naturaleza (verde oliva,
  marrón cuero, azul río, acentos cálidos), estética outdoor/aventura,
  luz natural, nada plástico ni artificial.
- Coherencia sonora: voz cálida y cercana, tono conversacional (no
  locución de venta agresiva), ritmo relajado como quien cuenta una
  buena jornada de pesca.

Cuando generes prompts para imagen o audio, siempre vas a especificar
parámetros técnicos explícitos (no dejarlos "a la suerte" del modelo).
```

### 3.2 Prompt Maestro (motor modular)

```
Actuando bajo las Instrucciones Base de Búho, generá un
[TIPO DE ACTIVO: imagen / guion de audio] para [OBJETIVO ESPECÍFICO,
ej: "presentar la marca a un comercio minorista" / "mostrar un producto
destacado del catálogo"].

Contexto de uso: [dónde se va a usar — ej: catálogo digital, punto de
venta, redes B2B, presentación comercial]

Restricciones:
- Debe respetar la paleta y tono definidos en las Instrucciones Base.
- No debe incluir texto ilegible ni logos de terceros.
- Debe transmitir [atributo clave, ej: solidez / calidad de importación /
  profesionalismo].

Salida esperada: [describí el formato — ej: descripción de imagen lista
para generar en Midjourney/DALL-E con parámetros, o guion de locución
con indicaciones de tono y ritmo]
```

> 💡 Este prompt maestro es el "molde": lo reusás cambiando el `[TIPO DE ACTIVO]`
> y el `[OBJETIVO ESPECÍFICO]` para generar cada pieza sin perder coherencia.

---

## 4. Producción Multimodal

### 4.1 Imágenes (mínimo 3)
Para cada imagen documentá:

| Imagen | Prompt usado | Herramienta | Variante/Modelo | Notas |
|---|---|---|---|---|
| 1. Concepto de marca/logo | Prompt de la sección 4.1 (amanecer junto al río) | Krea | Nano Banana 2 Lite | Generada en el primer intento |
| 2. Producto de catálogo | Prompt de la sección 4.1 (caña y reel, catálogo) | ChatGPT | — | Generada en el primer intento |
| 3. Pieza para punto de venta | Prompt de la sección 4.1 (exhibidor de mostrador) | Gemini | — | Se regeneró 2 veces sin editar el prompt; se eligió la 2ª versión por mejor resultado |

**Prompts listos para usar** (pegalos en tu herramienta de imagen — Midjourney, DALL-E, etc. — y ajustá Seed/CFG/Steps según la herramienta):

> **Imagen 1 — Concepto de marca:**
> "Amanecer junto a un río, una caña de pescar y un reel apoyados sobre
> piedras junto al agua, luz cálida natural, paleta verde oliva y marrón
> cuero, estética aventurera y cercana, fotografía realista, sin texto,
> sin personas, ambiente auténtico de pesca al aire libre."

> **Imagen 2 — Producto de catálogo (caña y reel):**
> "Fotografía de catálogo profesional de una caña de pescar y un reel
> de alta calidad, fondo neutro gris claro, iluminación de estudio suave,
> ángulo tres cuartos, detalle nítido de materiales y terminaciones,
> estilo comercial B2B, sin texto ni logos."

> **Imagen 3 — Pieza para punto de venta:**
> "Mockup de exhibidor de mostrador para comercio de pesca, madera
> natural y detalles verde oliva, cañas y reeles ordenados prolijamente,
> ambiente cálido de local especializado, luz natural, composición
> limpia, espacio en blanco para agregar logo después."

**Parámetros a documentar en la tabla:** Seed (para poder replicar/iterar), CFG Scale (7-9 suele mantener buen equilibrio entre fidelidad al prompt y naturalidad), Steps (25-40 según la herramienta).

### 4.2 Audio (mínimo 2)
Para cada audio documentá:

| Audio | Guion / prompt usado | Herramienta | Voz/tono | Duración | Notas |
|---|---|---|---|---|---|
| 1. Spot de presentación B2B | Guion de la sección 4.2 | ElevenLabs | Cálida, cercana | ~30 seg | Sonó natural, sin necesidad de ajustes |
| 2. Mensaje corto de marca | Guion de la sección 4.2 | ElevenLabs | Cálida, cercana (misma voz que Audio 1) | ~10-15 seg | Sonó natural, sin necesidad de ajustes |

**Guiones listos para usar** (pegalos en tu herramienta de audio/voz — ElevenLabs, etc. — eligiendo una voz cálida, tono conversacional):

> **Audio 1 — Spot de presentación B2B (~30 seg):**
> "Hay algo que no cambia: la sensación de la primera picada del día.
> En Búho importamos cañas y reeles pensando en eso — en
> que cada cliente que entra a tu local viva ese momento con un equipo
> que realmente responde. Trabajamos con precios pensados para que a vos
> te cierren los números, y con una atención directa, de persona a
> persona, para que nunca estés solo con una duda. No somos un
> importador más: somos el socio con el que tu local va a crecer."
> *(Indicaciones de tono: cálido, cercano, ritmo pausado, como una
> charla entre conocedores — no venta agresiva.)*

> **Audio 2 — Mensaje corto de marca / firma sonora (~10-15 seg):**
> "Búho. Pesca, precio y cercanía — todo en un mismo equipo."
> *(Indicaciones de tono: mismo registro cálido, más simple y directo,
> pensado para cerrar presentaciones o sonar en el punto de venta.)*

 ** Video (generado con Arena AI, editado en CapCut)
| Video | Contenido | Herramienta | Variante/Modelo |
|---|---|---|---|
| 1. Versión original | Animación de la Imagen 1 (concepto de marca), con sonido ambiente de agua generado por el propio modelo | Arena AI (video) | Veo 3.1 |
| 2. Versión final | Misma animación, con el Audio 2 (mensaje de marca) mezclado por encima del sonido de agua, volumen ambiente reducido | Arena AI (video) + CapCut (mezcla de audio) | Veo 3.1 |

> 🔊 **Nota sobre el audio del video:** Veo 3.1 generó sonido ambiente
> propio (agua del río) junto con el video, sin necesidad de agregarlo
> manualmente. Se decidió conservar ambas versiones en la entrega: la
> original con solo el ambiente sonoro, y una versión final editada en
> CapCut donde se suma el Audio 2 (mensaje hablado de marca) por encima,
> con el volumen del ambiente reducido para que no tape la voz.                                               
---

## 5. Matriz de Ética y Responsabilidad

| Riesgo identificado | ¿Dónde apareció? | Cómo se mitigó |
|---|---|---|
| Texto ilegible o logos inventados | No se detectó en ninguna de las 3 imágenes generadas | Se revisaron las 3 imágenes al recibirlas; ninguna necesitó regeneración por este motivo |
| Voz artificial o poco creíble | No se detectó en los 2 audios generados con ElevenLabs | Ambos audios sonaron naturales en la primera generación; no fue necesario ajustar sliders ni cambiar de voz |
| Representación / diversidad en imágenes con personas | No aplica en esta entrega — las 3 imágenes producidas son de paisaje, producto y punto de venta, sin personas | Se decidió no incluir un avatar de persona real en esta fase; si se agrega en el futuro, se deberá auditar representación de género/edad antes de publicar |
| Derechos de autor / privacidad | — | Se confirmó que ninguna de las 3 imágenes ni los 2 audios reproduce marcas, logos o voces de personas reales existentes; todos los activos fueron generados desde cero a partir de los prompts del sistema |

---
