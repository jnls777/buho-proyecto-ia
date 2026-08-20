# Búho — Proyecto Final IA

## Contexto y objetivos
Búho es una nueva marca importadora de artículos de pesca (foco en cañas
y reeles) que vende exclusivamente a comercios minoristas (modelo B2B).
El objetivo de este proyecto fue diseñar un Sistema de IA que permitiera
posicionar la marca frente a esos comercios, destacando precio competitivo
y atención cercana, con un tono aventurero y humanizado — y usar ese
sistema para producir activos multimodales (imágenes y audio) coherentes
con esa identidad.

## Sistema de IA usado

**Instrucciones Base (System Prompt):**
Definen a la IA como Director Creativo de Búho, estableciendo tono
(aventurero, cercano, humanizado), los dos pilares de diferenciación
(precio y atención), y reglas de coherencia visual (paleta tierra/naturaleza)
y sonora (voz cálida, ritmo conversacional).

**Prompt Maestro:**
Plantilla modular reutilizada para generar cada prompt específico de
imagen o audio, siempre respetando el tono y la paleta definidos en las
Instrucciones Base, y especificando el objetivo y contexto de uso de
cada pieza.

*(Ver el detalle completo de ambos prompts en el documento de
planificación del proyecto.)*

## Prompts y parámetros

### Imágenes
| Imagen | Contenido | Herramienta | Variante/Modelo |
|---|---|---|---|
| 1 | Concepto de marca — amanecer junto al río con caña y reel | Krea | Nano Banana 2 Lite |
| 2 | Producto de catálogo — caña y reel, fondo neutro | ChatGPT | — |
| 3 | Punto de venta — mockup de exhibidor de mostrador | Gemini | — (2 intentos, se eligió la 2ª versión) |

### Audio (generado con ElevenLabs)
| Audio | Contenido | Herramienta |
|---|---|---|
| 1 | Spot de presentación B2B (~30 seg) | ElevenLabs |
| 2 | Mensaje corto de marca / firma sonora (~10-15 seg) | ElevenLabs |

### Video (generado con Arena AI, editado en CapCut)
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

## Activos generados

### Imágenes
![Concepto de marca](https://raw.githubusercontent.com/jnls777/buho-proyecto-ia/main/buho-imagen1-concepto-marca.png)
![Producto de catálogo](https://raw.githubusercontent.com/jnls777/buho-proyecto-ia/main/buho-imagen2-producto-catalogo.jpeg)
![Punto de venta](https://raw.githubusercontent.com/jnls777/buho-proyecto-ia/main/buho-imagen3-punto-venta.jpeg)

### Audio
- [Escuchar Audio 1 — Spot B2B](https://github.com/jnls777/buho-proyecto-ia/blob/main/buho-audio1-spot-b2b.mp3)
- [Escuchar Audio 2 — Mensaje de marca](https://github.com/jnls777/buho-proyecto-ia/blob/main/buho-audio2-mensaje-marca.mp3)

### Video
- [Ver Video 1 — Versión original (sonido de agua)](https://github.com/jnls777/buho-proyecto-ia/blob/main/buho-video1-original-ambiente.mp4)
- [Ver Video 2 — Versión final (con Audio 2 mezclado)](https://github.com/jnls777/buho-proyecto-ia/blob/main/buho-video2-final-con-audio.mp4)

## Consideraciones éticas
Se auditaron los 3 activos de imagen y no se detectó texto ilegible ni
logos inventados. Los 2 audios generados sonaron naturales sin necesidad
de ajustes adicionales. No se incluyó un avatar de persona real en esta
entrega; de sumarse en una futura iteración, se auditará especialmente
la representación de género y edad antes de publicar. Se confirmó que
ningún activo reproduce marcas, logos o personas reales existentes — todo
fue generado desde cero a partir del Sistema de IA definido.

## Conclusiones
[Mi reflexion sobre el curso de IA, es que a traves del avance del curso adquirí nuevos conocimientos sobre IA que ya utilizaba en la cotidianidad y tambien conoci diferente IA que no sabia de su existencia, gracias a esas nuevas herramientas pude crear este proyecto. Lo que mejoraria del proyecto es hacerlo mas personalizado poder utilizar el logo, fotos reales mejoradas con IA para poder llevarlo a cabo en la vida real.]
