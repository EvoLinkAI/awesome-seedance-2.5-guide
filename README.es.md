<div align="center">

<a href="https://evolink.ai/seedream-5-0?utm_source=github&utm_medium=banner&utm_campaign=awesome-seedance-2.5-guide"><img src="assets/banner.png" alt="Seedance 2.5 Early Access guide" width="100%"></a>

# Guía oficial de Seedance 2.5

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](LICENSE)
[![Get Seedance 2.5 Early Access](https://img.shields.io/badge/Get_Seedance_2.5-Early_Access-black)](https://evolink.ai/seedream-5-0?utm_source=github&utm_medium=badge&utm_campaign=awesome-seedance-2.5-guide)
[![Official Guide](https://img.shields.io/badge/Official_Guide-36_Media_Assets-7C3AED)](data/seedance-2-5-manifest.json)
[![API Key](https://img.shields.io/badge/API_Key-EvoLink-orange)](https://evolink.ai/signup?utm_source=github&utm_medium=badge&utm_campaign=awesome-seedance-2.5-guide)

[English](README.md) · **Español** · [Português](README.pt.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · [Türkçe](README.tr.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Русский](README.ru.md)

</div>

## 🍌 Introducción

Seedance 2.5 early access ya está abierto mediante EvoLink. Este repositorio convierte los materiales oficiales de lanzamiento en una guía nativa de GitHub para creadores, desarrolladores y equipos de video con IA.

La guía cubre 36 recursos oficiales: demos de lanzamiento, showcases, control narrativo, expresión multilingüe y edición controlable. Todos son casos oficiales, por eso no añadimos autor ni línea de fuente por caso.

[Get Seedance 2.5 Early Access](https://evolink.ai/seedream-5-0?utm_source=github&utm_medium=readme&utm_campaign=awesome-seedance-2.5-guide) · [Obtener API key](https://evolink.ai/signup?utm_source=github&utm_medium=readme&utm_campaign=awesome-seedance-2.5-guide) · [Ejemplos actuales de API Seedance](https://github.com/EvoLinkAI/Seedance-2.5-Gateway-Service)

Si buscas Seedance 2, la guía original se conserva aquí: [Guía original de Seedance 2](seedance-2-guide/README.es.md) · [Índice de 55 casos](use-cases/README.md).

> [!NOTE]
> Los snippets ejecutables actuales siguen usando la ruta estable de la API Seedance 2 mientras Seedance 2.5 early access se despliega. No reemplaces los model IDs verificados `seedance-2.0-*` por IDs 2.5 no verificados.

## 📑 Menú

- Introducción
- Inicio rápido
- Guía original de Seedance 2
- Guía oficial de Seedance 2.5
- Estructura del repositorio
- Reconocimiento

## 🚀 Inicio rápido

Usa este repositorio para revisar ejemplos oficiales 2.5, copiar estructuras de prompt y unirte al rollout 2.5.

> [!NOTE]
> Este inicio rápido mantiene intencionalmente el model ID verificado `seedance-2.0-text-to-video` y la ruta actual de la API Seedance 2. Seedance 2.5 API access está llegando mediante early access; no sustituyas este model ID ejecutable por un ID 2.5 no verificado.

```bash
export EVOLINK_API_KEY="your_key_here"

curl --request POST \
  --url https://api.evolink.ai/v1/videos/generations \
  --header "Authorization: Bearer ${EVOLINK_API_KEY}" \
  --header 'Content-Type: application/json' \
  --data '{
    "model": "seedance-2.0-text-to-video",
    "prompt": "A cinematic product reveal, slow dolly-in, reflective glass table, premium commercial lighting",
    "duration": 5,
    "quality": "720p",
    "aspect_ratio": "16:9",
    "generate_audio": true
  }'
```

## 🧭 Guía original de Seedance 2

La nueva guía oficial de Seedance 2.5 está primero. La guía original completa de Seedance 2 se conserva como destino legacy para la ruta API actual, patrones de casos de uso, plantillas de prompt, notas de parámetros y workflow multimodal.

- [Abrir la guía original completa de Seedance 2](seedance-2-guide/README.es.md)
- [Abrir el índice original de 55 casos](use-cases/README.md)
- [Casos Seedance 2 en inglés](use-cases/en/README.md)
- [Casos Seedance 2 en chino simplificado](use-cases/zh-CN/README.md)
- [Casos Seedance 2 en chino tradicional](use-cases/zh-TW/README.md)
- [Ejemplos actuales de API Seedance](https://github.com/EvoLinkAI/Seedance-2.5-Gateway-Service)

## 🎬 Guía oficial de Seedance 2.5

## Vídeo en la mitad superior de la página

### Case 1: Vídeo de la mitad superior de la página 1

[![Vídeo de la mitad superior de la página 1](assets/thumbnails/01-hero-demo-1-official-launch-film-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/firstScreen/group2/2.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/firstScreen/group2/2.mp4) · Haz clic en la miniatura para reproducir el video.

**Prompt:**

```text
Una secuencia cinematográfica de gráficos en movimiento 3D de 30 segundos de alta gama, que utiliza exquisitos estilos de paisajes en miniatura steampunk y retro, con movimientos de cámara envolventes y penetrantes continuos y suaves.
[0-10 segundos]: Primer plano macro de la esfera de un reloj de latón antiguo, que se despliega milagrosamente en anillos de engranajes giratorios entrelazados y niebla volumétrica. La cámara penetra hacia abajo a través de los engranajes y un ornitóptero mecánico se eleva hacia el cielo desde un cañón en miniatura hecho de pilas de libros antiguos.
[10-20 segundos]: La cámara sigue la trayectoria del ornitóptero mientras se desliza hacia adelante, penetrando sin problemas en una caja fantasma de latón ornamentada y giratoria de alta velocidad (Zoetrope), que proyecta la luz y la sombra dinámicas de un caballo mecánico al galope. La luz y la sombra saltaron de la caja, y la escena se transformó instantáneamente en un teleférico suspendido con textura de latón, que viajaba a través del bosque de engranajes mecánicos a lo largo de relucientes rieles de cobre, bañado en una luz dorada de nivel cinematográfico.
[20-30 segundos]: La cámara se desplaza con gracia hacia abajo y un hermoso velero mecánico de madera con mecanismo de relojería aparece debajo del teleférico, cortando las ondulantes olas hechas de vidrio azul oscuro. El final de las olas evolucionó sin problemas hasta convertirse en una luna gigante brillante, y las siluetas de un grupo de exploradores sosteniendo linternas oscilantes caminaban a lo largo de la cresta de la mina de cristal bajo las estrellas. La cámara se aleja en una suave espiral, a través de nubes etéreas, y regresa a la gran esfera de latón del reloj.
Especificaciones técnicas: texturas mecánicas hiperrealistas, ricos tonos dorados y latón y poca profundidad de campo cinematográfica. Movimiento fluido y coherente del transbordador, una fuerte sensación de atmósfera de aventura épica y fantástica.
```

---

### Case 2: Vídeo de la mitad superior de la página 2

[![Vídeo de la mitad superior de la página 2](assets/thumbnails/02-hero-demo-2-official-launch-film-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/firstScreen/group1/1.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/firstScreen/group1/1.mp4) · Haz clic en la miniatura para reproducir el video.

**Prompt:**

```text
Un cortometraje de ritmo rápido, cinematográfico y con una transición fluida (match-cut) con ritmos electrónicos dinámicos. En el centro del cuadro siempre hay una bola de cristal impecable, con el logotipo luminoso "seedance" grabado en su interior. La bola de cristal mantiene un enfoque extremo y, con el potente ritmo del tambor musical, el fondo cambia sin problemas a alta velocidad:
Escena 1: Primer plano macro, agua similar a una película salpicando alrededor de la bola de cristal, refractando luces y sombras complejas.
Escena 2: Un café retro por la mañana. La bola de cristal se coloca sobre la mesa de madera. El fondo es el vapor del café y el flujo borroso de viajeros fuera de la ventana.
Escena 3: En la hora dorada de la noche, un joven que practica skate lanza una bola de cristal con una mano. El fondo es la escena de la calle que retrocede rápidamente y la hermosa luz de fondo del atardecer.
Escena 4: En el Frenzy Music Festival, la gente sostiene bolas de cristal, reflejando el láser del escenario con un hermoso fondo.
Escena 5: Una animada mesa de fiesta familiar, con una bola de cristal en el centro y figuras borrosas al fondo celebrando un brindis y tomando comida.
Escena 6: En un cine oscuro, ambas manos sostienen una bola de cristal y la tenue luz de la enorme pantalla fluye sobre su superficie.
Escena 7: La bola de cristal se coloca sobre el diafragma de sonido que vibra fuertemente y cambia sin problemas al centro del reproductor DJ giratorio con el clímax de la música.
Escena 8: Noche de acampada al aire libre, el fondo cambia a una cálida hoguera y puntos de luz oscilantes (Bokeh).
Lanzamiento y final: Con el acento final de la música, la bola de cristal fue lanzada muy por encima de la pantalla; instantáneamente se cortó a un fondo negro puro, y la palabra blanca minimalista "seedance" sobre un fondo negro apareció en el centro de la pantalla.
Siga de cerca la edición dinámica del ritmo BGM (transición atascada) y la gradación de color cinematográfica de primer nivel (Cinematic Color Grading). Materiales realistas de refracción y transmisión de vidrio, trazado de rayos complejo e iluminación global. El sujeto es extremadamente claro, el fondo tiene un fuerte desenfoque dinámico y el impacto visual es extremadamente fuerte.
```

---

### Case 3: Vídeo de la mitad superior de la página 3

[![Vídeo de la mitad superior de la página 3](assets/thumbnails/03-hero-demo-3-official-launch-film-3.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/firstScreen/group3/output.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/firstScreen/group3/output.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 5

**Prompt:**

```text
Cortometraje cinematográfico sobre concepto de marca.<<<image_1_1>>>es el primer fotograma, la pantalla tiembla ligeramente, la cámara se acerca gradualmente y llega a la sombra del árbol que retrocede rápidamente fuera de la ventana. La sombra del árbol retrocede cada vez más rápido y de repente corta a<<<image_2_2>>>, la velocidad disminuye repentinamente, la cámara se mueve lentamente a lo largo del arroyo, los pájaros cantan y las flores son fragantes.
La cámara descendió hacia el agua. El efecto de sonido incluía el sonido de burbujas en el agua. Un grupo de medusas de color naranja nadaba con gracia frente a la cámara.<<<image_3_3>>>. La cámara retrocedió lentamente. Un grupo de peces pequeños pasó junto a la cámara, atravesó el agua y entró por la ventana.<<<image_4_4>>>. La niña miró a izquierda y derecha, observando al pequeño pez.
La cámara se retira lentamente y la imagen queda desenfocada, luego vuelve a enfocar y la imagen se vuelve clara, cambiando al ritmo de la música: círculos de luz de la ventana del jardín chino<<<image_5_5>>>, vidrieras de iglesias, ojos de buey de aviones, claraboyas de cúpula, ventanales, persianas, buhardillas europeas, ojos de gato en las puertas, visores de cámaras, ojos de pájaros y primeros planos de ojos humanos.
La pantalla permanece en un primer plano de ojos humanos, luego los ojos se cierran y la pantalla se vuelve negra. Entonces, de repente, se abren los ojos y aparece la palabra "seedance" con acento en el centro de los ojos.
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

## El usuario trabaja

### Case 4: efectos visuales 1

[![efectos visuales 1](assets/thumbnails/04-official-showcase-4-visual-effects.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/16-9/169-1.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/16-9/169-1.mp4) · Haz clic en la miniatura para reproducir el video.

**Prompt:**

```text
Un vídeo de animación de texto creativo en bucle continuo de 15 segundos, 4K, 30 fps. Cada idioma tarda aproximadamente 1,2 segundos y la transición se logra mediante la disolución, deformación o dispersión de partículas del texto, sin cortes bruscos. La música de fondo tiene un ritmo evidente y un fuerte desfase.
0-1.2s "Creación" china·Op ilusión óptica fondo negro puro, círculos concéntricos blancos y negros extendidos desde el centro para formar un túnel visual. El carácter chino tridimensional blanco "Creación" sobresale lentamente desde el centro del círculo hacia la cámara. Es atrevido y sans serif con sombras sutiles en los bordes. Los círculos concéntricos crean ondas y distorsiones a medida que avanza el texto, como ondas en el agua. El texto se detuvo después de que sobresalió por completo, luego se disolvió en partículas de crayón azul y se alejó flotando.
1.2-2.4s Inglés "CREAR" · Fondo de textura de papel kraft amarillo cálido con crayón pintado a mano, trazos ásperos de crayón azul escriben el "CREAR" en inglés en mayúsculas uno por uno. Las pinceladas tienen un granulado pastel evidente y marcas superpuestas, y la última línea horizontal de la E está ligeramente elevada. Después de escribir, la superficie de las letras tiene un ligero brillo ceroso y aparecen líneas auxiliares de lápiz tenues en el fondo. Luego, el texto es absorbido por las líneas de escaneo del CRT y desaparece.
2.4-3.6s Español "CREAR" · Marco arcade oscuro arcade retro, la pantalla CRT central tiene líneas de escaneo sutiles y granulosidad de polvo de fósforo. La palabra tridimensional en píxeles "CREAR" con un degradado azul y morado se eleva desde la parte inferior. La superficie de las letras tiene una animación ondulada blanca como las olas del océano y el borde emite una luz azul neón. Hay "CRÉDITO 00" en la esquina superior izquierda de la pantalla y "INSERT COIN" parpadea en la esquina inferior derecha. Luego, el texto se pixeló y se desintegró en un patrón de batik índigo.
3,6-4,8s "CIPTAKAN" indonesio · Tejido batik. Fondo de tela batik indonesia tradicional azul índigo oscuro, con finos patrones parabólicos en la superficie de la tela. La fuente serif blanca "CIPTAKAN" se eleva lentamente desde la parte inferior de la tela, como si fuera un estampado en caliente, y la tela crea arrugas y fluctuaciones reales a medida que emerge el texto. Después de que aparecieron las palabras, la tela fue arrastrada por el viento y los escombros dorados volaron, convirtiéndose en patrones geométricos islámicos.
4.8-6.0s "CIPTA" malayo·Geometría islámica. Fondo de terciopelo verde oscuro, motivos geométricos arabescos dorados extendidos desde las cuatro esquinas hasta el centro. La palabra serif clásica blanca "CIPTA" gira y emerge del centro. Las letras están rodeadas de patrones de estrellas y caen partículas de polvo de oro. Luego, las palabras fueron grabadas palabra por palabra en la placa de metal negro con un cuchillo de grabado dorado.
6.0-7.2s "สร้างสรรค์" tailandés · Grabado en lámina de oro sobre fondo negro, el "สร้างสรรค์" tailandés se presenta en oro, como si estuviera tallado en una placa de un templo antiguo. Hay una animación sutil de una lámina dorada despegándose de la superficie del texto, revelando la imprimación roja oscura debajo, con fragmentos dorados volando. Una vez finalizado el grabado, las palabras se funden en gotas de mercurio plateado y gotean.
7.2-8.4s Árabe "إبداع" · Paso de página mecánico. La pantalla de paso de página de metal negro ocupa toda la pantalla y las cuchillas mecánicas hacen clic y giran a su vez. El texto árabe "إبداع" compuesto por cuadrículas de píxeles blancos aparece uno por uno de derecha a izquierda, y cada cambio de letra va acompañado de un movimiento mecánico preciso y una ligera vibración. Cuando se completa el cambio de página, el texto es arrastrado por una tormenta de coloridas plumas de samba.
8.4-9.6s "CRIAR" portugués · Plumas de Carnaval. Sobre un fondo negro, coloridas plumas de samba convergen desde el borde de la imagen hacia el centro para formar un enorme abanico de plumas. Las letras blancas en negrita "CRIAR" brotaron del centro del abanico de plumas, y las plumas volaron con el impacto de las palabras. La superficie de las palabras se reflejaba en las lentejuelas del Carnaval y los puntos verdes, amarillos y azules de la bandera brasileña destellaban. Luego se lavó el texto con tinta negra.
9.6-10.8s Vietnamita "SÁNG TẠO" · Tinta de seda. Sobre un fondo de seda blanquecino, tinta negra fluye lentamente desde la parte superior de la imagen, formando gradualmente la palabra vietnamita "SÁNG TẠO". La tinta crea un borde difuminado natural en la seda y algunas de las gotas de tinta gotean para formar perlas de tinta colgantes. Una vez finalizada, la seda fue arrastrada por el viento, revelando el patrón oscuro del loto debajo y el texto se condensó en una bola de vidrio transparente.
10.8-12.0s "Creación" en japonés · Vidrio óptico Una perfecta bola de vidrio óptico transparente está suspendida en el centro de un fondo negro puro. La bola refleja el astigmatismo con los colores del arcoíris. Detrás de la bola de cristal, el carácter chino japonés "Creación" se presenta en una proyección de dispersión de arco iris. A medida que la bola de cristal gira lentamente, el texto produce una distorsión óptica que se tuerce, se estira y se separa. En la superficie de la esfera de vidrio se encuentran finas partículas de polvo que luego se funden formando un metal líquido plateado.
12.0-13.2s Coreano 「창조」· Metal líquido. Contra el fondo del profundo cielo estrellado, el mercurio líquido plateado gotea desde la parte superior de la imagen y, naturalmente, se condensa en la palabra coreana "창조" en el aire. La superficie de los caracteres líquidos tiene una fuerte reflexión especular, reflejando las estrellas circundantes. Después de que se formaron las palabras, parte del líquido de mercurio continuó goteando hacia abajo, formando cuentas de metal colgantes. Finalmente, todo el líquido metálico se reunió en una enorme esfera plateada.
```

---

### Case 5: Película 2

[![Película 2](assets/thumbnails/05-official-showcase-5-cinematic-film.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/3-4/34-1.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/3-4/34-1.mp4) · Haz clic en la miniatura para reproducir el video.

**Prompt:**

```text
【Configuración de estilo general】
Un éxito de taquilla visual de alta gama de 30 segundos con una fuerte sensación cinematográfica y una textura de alta gama. La imagen enfatiza puntos de luz de ensueño (Bokeh), transiciones sedosas de desenfoque de movimiento (Desenfoque de movimiento), iluminación volumétrica y expresión de detalles de materiales ultrarrealistas.
[Descripción del guión gráfico]
[0-5 segundos]: prólogo del sueño y primer plano macro
Primeros planos macro de muy alta calidad. Una mano delgada se extendió en el aire y sus dedos tocaron puntos coloridos tan brillantes y centelleantes como estrellas. Con el flujo de luces y sombras, la escena pasa de manera fluida y fluida a una mujer elegante vestida con una falda de tul de color blanco puro, que toca embriagada un piano antiguo. Con poca profundidad de campo, el fondo se difumina en un hermoso tono azul verdoso.
[5-15 segundos]: Luego pasa a una suave toma de seguimiento: una mujer con un sombrero de paja francés de ala ancha y una falda blanca suelta, corriendo con ligereza por el denso sendero de flores lleno de rosas de color rosa anaranjado y hortensias azules. La luz proyecta luces y sombras moteadas a través de las hojas, mostrando perfectamente la suave brisa, la física realista del aleteo de la tela de la falda y la textura ultrarrealista de los pétalos.
[15-24 segundos]: Estética silenciosa y refracción de luces y sombras
El ritmo de la cámara se ralentiza y entra en la más hermosa cámara lenta (cámara lenta). Una niña está sentada en una mesa de hierro forjado negro junto a una fuente dorada retro europea y leyendo tranquilamente. Hay pompas de jabón cristalinas flotando en el aire y la superficie de las burbujas refleja perfectamente las flores circundantes y el cálido sol. El momento en que las gotas de agua salpican es claramente visible, lo que demuestra las capacidades de representación de alto nivel del modelo para materiales transparentes, refracción del agua e iluminación compleja.
```

---

### Case 6: Efectos de postproducción 3

[![Efectos de postproducción 3](assets/thumbnails/06-official-showcase-6-post-production-vfx.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/1-1/11-1.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/1-1/11-1.mp4) · Haz clic en la miniatura para reproducir el video.

**Prompt:**

```text
Una escena de arrecifes de coral de aguas profundas, un mundo submarino tropical dominado por el azul, con una gran área de corales vivos coloridos, saludables y prósperos, incluidos corales ramificados, corales cerebro, corales disco y corales abanicos de mar blandos, con una gran cantidad de peces tropicales que se desplazan naturalmente entre ellos. La vista de cerca es clara y vívida, mientras que la vista de lejos se vuelve gradualmente más azul y gris y el contraste se debilita. La luz natural de arriba es filtrada por el agua de mar para formar una suave luz volumétrica. Hay pequeñas partículas suspendidas y una ligera sensación de flujo en el agua de mar. 8-12 de varios tamaños. El cuerpo en forma de paraguas tiene un suave efecto de bioluminiscencia, los tentáculos revolotean suavemente con las olas y hay tenues puntos de luz púrpura en los extremos de los tentáculos. El tamaño de las medusas es proporcional al de los corales y los peces, y el efecto luminoso es suave y no deslumbrante, formando puntos de luz de ensueño sobre el fondo oscuro del agua del mar. El movimiento del enjambre de medusas es natural, en una espiral que se eleva lentamente, y algunas medusas nadan más allá del frente de la lente, creando un ligero efecto de destello en la lente. Manteniendo la iluminación en tonos azules bajo el agua, el brillo de las medusas coexiste armoniosamente con los débiles reflejos de los corales circundantes. Durante el proceso de natación del grupo de medusas, se generaron burbujas que flotaron, formando la palabra "Seedance" en el mar.
```

---

### Case 7: Película 4

[![Película 4](assets/thumbnails/07-official-showcase-7-cinematic-film.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/1-1/11-2.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/1-1/11-2.mp4) · Haz clic en la miniatura para reproducir el video.

**Prompt:**

```text
Textura cinematográfica, sensación de alta gama, desierto dorado por la mañana, un museo de arte blanco minimalista flotando sobre las dunas de arena, con finas texturas de piedra y suaves reflejos en la superficie del edificio. La luz del sol atraviesa la arena y el polvo para formar una luz volumétrica, y las dunas a lo lejos están claramente estratificadas. La cámara parte de un panorama del desierto de gran angular, avanza lentamente, atraviesa la arena voladora y entra al interior del edificio flotante. El interior presenta esculturas suspendidas, instalaciones de seda translúcida y un personaje con una túnica blanca, cuya tela se balancea naturalmente con el viento. La cámara se mueve suavemente alrededor de los personajes y, finalmente, las paredes del edificio se abren lentamente para revelar una vasta extensión de cielo y desierto. Estilo publicitario artístico de alta gama, iluminación real, materiales exquisitos, composición a nivel de película, movimiento elegante, surrealista pero auténtico.
```

---

### Case 8: Publicidad 5

[![Publicidad 5](assets/thumbnails/08-official-showcase-8-advertising.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/16-9/169-2.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/16-9/169-2.mp4) · Haz clic en la miniatura para reproducir el video.

**Prompt:**

```text
Un cortometraje de 30 segundos de alto nivel de concepto de marca y gran tensión visual. La apertura adopta una perspectiva invertida surrealista. La cámara gira con la gravedad, mostrando los pies de la modelo con botas de gamuza retro pisando ligeramente las onduladas dunas de arena roja. La lente macro cierra la textura aterciopelada esmerilada de la superficie de las botas y las ásperas partículas de arena roja manchadas en ella. Luego pasa a una serie de montajes llenos de ingravidez y colores de ensueño: jóvenes modelos masculinos y femeninos caen ligeramente hacia atrás en medio del viento ambarino, la arena y la fría luz del borde; la cámara rápidamente muestra un primer plano muy nítido de la cara: el viento y la arena soplan a través de las pestañas manchadas con una pequeña arena dorada, y la modelo usa gafas de sol con montura de metal retro, el sol abrasador y la tormenta de la naturaleza se reflejan claramente en las lentes curvas. Luego, los dedos que llevaban viejos y gruesos anillos de plata rozaron suavemente las ásperas paredes de roca y las cañas bailando con el viento.
Las imágenes hacen un uso extensivo de un lenguaje óptico altamente expresivo: a través de una lente macro de ángulo muy bajo, a través de los cristales minerales naturales borrosos y claros, el profundo y vasto cielo estrellado y los exploradores que viajan sin sentido son capturados desde arriba. La gran escena está densamente intercalada con primeros planos de alta calidad: la textura de la camisa de lino flameado susurrando con el viento, la mandíbula fría y apretada de la modelo y el brillo del sudor en la piel del cuello brillando bajo la luz de fondo. Combinando lentes de ojo de pez, rápidos movimientos de cámara giratorios y sedosas transiciones de dislocación visual, crea una dinámica misteriosa, vanguardista y llena de tensión salvaje.
En el clímax del cortometraje, la cámara se aleja dramáticamente, rompiendo la "cuarta pared", revelando que en realidad se trata de un estudio virtual avanzado con un dosel circular con un rastro de estrellas LED gigante y un conjunto de arena roja real, que choca perfectamente con la inmensidad de la naturaleza y la sensación de un estudio industrial pionero. Al final, el ritmo se ralentiza y vuelve a un primer plano de texturas delicadas: una mujer con el pelo despeinado apoyada en un todoterreno retro. La cámara recorre lentamente la pesada pintura metálica moteada y descascarada del vehículo. La mujer casualmente deja que la fina arena de su palma se resbale de sus dedos. La luz lateral fresca y brillante de la luna delinea con precisión los poros de la tela áspera de la chaqueta de cuero desgastada, la luz fría reflejada por la pesada cremallera de metal y el frío contorno facial tridimensional de la mujer. El diseño general presenta una estética de color retro a nivel de película, con un azul nocturno profundo entrelazado con un naranja mineral ardiente. La imagen es atmosférica, libre y llena de tensión de marca de alta calidad. Finalmente, el texto "seedance" aparece elegantemente en el centro de la imagen.
```

---

### Case 9: Película 6

[![Película 6](assets/thumbnails/09-official-showcase-9-cinematic-film.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/3-4/34-2.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/3-4/34-2.mp4) · Haz clic en la miniatura para reproducir el video.

**Prompt:**

```text
Cortometraje sobre patrimonio cultural inmaterial de la Ópera de Pekín, con aire cinematográfico, estética oriental, calidez y sobriedad. Entre bastidores de las compañías de teatro tradicionales y talleres de artesanía, los maestros artesanos confeccionan silenciosamente tocados para la ópera de Pekín, arreglan el vestuario y delinean el maquillaje facial. Los detalles de sus manos son delicados y los hilos de seda, cuentas, pinturas y patrones de bordado son todos de alta calidad. Un joven aprendiz observó atentamente, luego tomó con cuidado las herramientas y completó los pequeños pasos bajo la guía del maestro. El viejo maestro enderezó la cabeza y se arregló la ropa, como si entregara suavemente un oficio y una emoción en sus manos. Finalmente, el joven se vistió pulcramente y se paró junto al escenario donde estaba a punto de subir al escenario. La tenue luz iluminaba su traje y su perfil, y el viejo maestro observaba en silencio detrás de él. El ambiente general es tranquilo, afectuoso y con un sentido de herencia, con pocos subtítulos y líneas apropiadas intercaladas.
```

---

### Case 10: Juego 7

[![Juego 7](assets/thumbnails/10-official-showcase-10-game-trailer.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/16-9/169-3.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/16-9/169-3.mp4) · Haz clic en la miniatura para reproducir el video.

**Prompt:**

```text
"Civilización Oceánica"
(Ciencia ficción épica / Duna × Interestelar / Ninguna persona real / Escultura de forma de vida)
[0–5 segundos | Apertura cósmica·El océano como memoria planetaria]
El océano azul profundo ocupa toda la escena, y los cuerpos de agua extremadamente profundos presentan una estructura en capas, al igual que el universo líquido dentro del planeta.
La cámara cae lentamente verticalmente desde una gran altura, atraviesa las nubes y la niebla marina y entra al mar.
La superficie del mar fluctúa como una película de metal, refractando grietas irregulares en los rayos del sol, creando una luz volumétrica épica.
[5–10 segundos | Entrando en la falla de la civilización de las profundidades marinas]
La lente penetra la superficie del mar y entra en las profundidades del mar.
La enorme "estructura de la civilización submarina" surgió gradualmente:
Megaestructuras fracturadas en forma de anillo, cúpulas de piedra hundidas y plataformas de ruinas geométricas flotantes.
El estilo estructural combina templos antiguos + sentido tecnológico de civilización alienígena (similar al lenguaje de las ruinas de Dune).
Hay partículas brillantes suspendidas en el agua, como polvo de estrellas que flota lentamente en el agua.
[10–15 segundos | Aparece una forma de vida escultórica (no humana)]
En el centro del teatro hay una escultura gigante de una forma de vida:
Una "estatua humanoide" hecha de piedra blanca y minerales translúcidos, pero sin detalles de la vida (sin piel, sin rasgos humanos reales).
Su postura es como una antigua estructura ritual, y su cuerpo tiene una estructura geométrica segmentada, similar al portador de memoria de la civilización.
La superficie de la escultura ha sido erosionada por el agua durante mucho tiempo y está cubierta de algas y estructuras de cristales de coral.
La cámara rodea lentamente la escultura, creando una "sensación de la llegada de los dioses".
[15–20 segundos｜Se despierta la civilización·Flujo óptico activado]
Todas las ruinas submarinas comenzaron a "despertar".
Dentro de la escultura aparecen débiles patrones de luz que fluyen de energía, iluminándose como una red neuronal.
Los pilares de piedra rotos se elevan lentamente y se reorganizan para formar una estructura anular de teatro.
El cuerpo de agua comenzó a mostrar un "flujo ordenado", como si se estuviera recalculando el espacio.
La cámara está rodeada de estática → rotación ligeramente acelerada.
[20–24 segundos | Inversión de la superficie del mar · avance creciente]
La cámara acelera repentinamente hacia arriba y fuera del mar.
El agua de mar se separó a ambos lados, formando una cortina de agua gigante.
El casco de una nave espacial gigante/templo de una antigua civilización se eleva desde el fondo del mar:
Parece un cruce entre un templo de piedra y un barco de ciencia ficción, con su superficie cubierta de coral y estructuras mineralizadas.
El casco del barco se eleva como una cascada con el agua del mar.
[24–27 segundos | Toma giratoria épica (clímax visual)]
La cámara gira alrededor de la nave gigante a gran velocidad (toma en órbita en espiral).
El sol penetra a través de las grietas de las nubes, formando un pilar de luz sagrado.
El flujo de agua gira y se dibuja en forma de espiral, como la estructura de una galaxia.
El casco se voltea lentamente, revelando su enorme estructura:
Similar a las "reliquias de la civilización móvil" en lugar del transporte.
【27–30 segundos ｜ Visión definitiva · Revelando la escala de la civilización】
La cámara se aleja muy rápidamente hasta una perspectiva a nivel del espacio.
El océano, las ruinas, los barcos gigantes que se elevan y los templos escultóricos están dispuestos verticalmente en la misma pantalla:
Formando la estructura cósmica de tres secciones de "capa de luz de la civilización submarina-superficie del mar-cielo".
El mundo entero es como el sistema de memoria despierto de un planeta antiguo.
Al final, la imagen se desvaneció lentamente hasta convertirse en una pantalla negra, quedando sólo débiles puntos de luz.
Estética épica de ciencia ficción / Estructura de civilización de mar de arena y viento de dunas / Escala espacial a nivel interestelar / Narrativa sin carácter / Ruinas de civilización escultórica / Estructura de templo alienígena / Luz volumétrica que penetra el agua de mar / Colapso y reorganización de edificios gigantes / Tomas de rituales sagrados / Movimiento de espejo en espiral / Océano de partículas de polvo de estrellas / Realidad de alto rango dinámico a nivel de película
```

---

### Case 11: Cine y televisión 8

[![Cine y televisión 8](assets/thumbnails/11-official-showcase-11-cinematic-film.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/1-1/11-3.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/1-1/11-3.mp4) · Haz clic en la miniatura para reproducir el video.

**Prompt:**

```text
El tema es "Floración mecánica". La imagen debe resaltar las ventajas del modelo de vídeo generado en términos de luces y sombras, detalles artísticos, realismo, movimiento de la cámara y sensación cinematográfica de los personajes. El estilo general es un anuncio de marca de tecnología de punta con un fuerte impacto visual. El vídeo utiliza una toma macro de una sola toma, que comienza con los capullos de flores de metal en la oscuridad, ingresa gradualmente a la estructura mecánica precisa dentro de los pétalos y finalmente termina con la flor mecánica floreciendo completamente y la luz extendiéndose hacia afuera como clímax. Requiere iluminación física real, materiales exquisitos de metal y vidrio, movimiento mecánico delicado, composición estable, gradación de color a nivel de película y sin subtítulos.
```

---

### Case 12: Divulgación científica 9

[![Divulgación científica 9](assets/thumbnails/12-official-showcase-12-educational-film.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/3-4/34-3.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/3-4/34-3.mp4) · Haz clic en la miniatura para reproducir el video.

**Prompt:**

```text
Requisitos generales de estilo: animación plana en color roca, estética decorativa oriental y de la Ruta de la Seda, textura de pigmento mineral, rojo cinabrio, ocre, verde piedra, ultramar, adornos dorados, texturas de papel y murales, capas planas, sin fotografía real, sin realismo 3D. El ritmo de la imagen cambia de la quietud al movimiento, y luego del movimiento nuevamente a la quietud, resaltando la sensación de viaje y la riqueza de "de la tierra a la copa". La música es alegre y de estilo occidental.
Plano 1: Las ramas empiezan a aparecer y comienza la riqueza (0-4 segundos)
Bloques de ocre y bermellón florecen en el papel de la pintura de la Ruta de la Seda, y una rama de granada se extiende desde el lado derecho de la pintura. Las hojas son gruesas y tienen capas evidentes de pigmentos minerales. Una granada regordeta apareció lentamente en la rama. Su caparazón era rojo con oro y su contorno era redondo y tranquilo. La luz del sol cae sobre la cáscara con manchas redondas doradas y puntos de lámina dorada. La superficie de la granada tiene un brillo cálido, como una fruta madura con el tiempo. El temperamento inicial es rico pero comedido.
Plano 2: Quítalo suavemente y comienza el viaje (4-7 segundos)
La granada fue recogida suavemente por una criada de las regiones occidentales con movimientos suaves y elegantes. Patrones de hierba rizada, patrones antiguos y composiciones decorativas de volutas largas emergen gradualmente en el fondo, lo que sugiere que proviene de una tierra lejana. La imagen pasa naturalmente de ramas estáticas al desarrollo del viaje. Montañas, carreteras y pueblos empiezan a aparecer al fondo, como una larga ruta de la seda que se va desplegando lentamente.
Plano 3: Cruzando caminos antiguos y cruzando montañas y ríos (7-13 segundos)
Las siluetas del equipo de camellos avanzan lentamente, las campanas representan el ritmo con pequeños puntos dorados y aparecen granadas en la mochila del camello. La antigua carretera pasa por dunas de arena, oasis y puertas de la ciudad. El viento y la arena pasan en patrones fluidos, y el camino delineado por la línea dorada continúa extendiéndose en la distancia. Los colores son fuertes y de alta gama, como una fusión de murales de la Ruta de la Seda e ilustraciones en color rock. La granada siempre ha estado brillante y llena durante el largo viaje, como si hubiera conservado el sol, el calor y la riqueza de la tierra lejana hasta el día de hoy.
Plano 4: Transición entre la antigüedad y la modernidad, llegando al momento presente (13-16 segundos)
Los patrones antiguos y los contornos arquitectónicos del fondo se simplifican gradualmente y el tiempo pasa silenciosamente al espacio moderno. La granada se coloca sobre una encimera moderna y la mesa y los utensilios se presentan con una geometría plana simple. Las visiones antiguas y modernas están conectadas en la misma imagen, y el ritmo de la imagen cambia del "viaje" a la "llegada".
Plano 5: Cortando la granada, clímax visual (16-20 segundos)
Corta suavemente la granada con una mano, con movimientos lentos y restringidos. El momento en que se abre la cáscara es muy ritual.
Tiro 6: Exprimido en jugo, fluyendo abundantemente (20-24 segundos)
Las semillas entran en el recipiente y se exprimen hasta obtener un rico jugo de granada. El líquido fluye con una textura de color rojo intenso y transparente, con finas partículas de color roca. El jugo de granada se vierte lentamente en un vaso moderno. El contorno del cristal es claro y conciso. El líquido rojo sube en la copa, formando ligeras ondulaciones y reflejos en la superficie. Unos cuantos cubitos de hielo cayeron en la taza y el blanco frío y el rojo intenso contrastaron marcadamente. Aparecieron finas gotas de agua en la pared de la taza y la sensación refrescante se llenó.
Plano 7: Bebida moderna, viaje hasta el final (24-27 segundos)
El fondo está cortado en una escena de la vida moderna, y la luz de la ventana, la mesa, las telas y las plantas mantienen elementos decorativos planos y colores cálidos. La taza de jugo está colocada en el centro de la imagen, con patrones de caminos antiguos, caravanas de camellos y puertas de la ciudad vagamente superpuestos a su alrededor, lo que sugiere que esta taza de jugo proviene de un largo viaje. El ambiente es rico, cálido y tranquilo.
Plano 8: El tiempo converge, final estilo cartel (27-30 segundos)
Los antiguos patrones de carreteras al fondo se fusionan gradualmente con el espacio moderno, como el tiempo convergiendo en este vaso de jugo. La imagen recuerda brevemente a la granada en la rama, la sombra del camello en el camino antiguo y las semillas rojas, formando un circuito completo "desde la tierra hasta la copa". Finalmente, se reúne en una composición similar a un cartel publicitario: en el centro se coloca jugo de granada de color rojo intenso, con una granada rota al lado de la taza, rodeada de patrones de caminos antiguos, puntos de luz dorada y elementos de la vida moderna. La imagen es tranquila pero llena de vitalidad, como un viaje a través del tiempo y una tierra que finalmente ha llegado al momento presente. El lema publicitario es "Seedance, un regalo de las regiones occidentales".
```

---

## Empujando los límites narrativos

### Case 13: Rompiendo los límites de la narrativa - 30 segundos de continuidad - salida - 1

[![Rompiendo los límites de la narrativa - 30 segundos de continuidad - salida - 1](assets/thumbnails/13-narrative-control-13-30-second-continuous-output-group-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab1/group1/output.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab1/group1/output.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 8

**Prompt:**

```text
De izquierda a derecha, la cámara sigue constantemente a un hombre con un abrigo negro (consulte<<<image_1_1>>>) a través de seis habitaciones conectadas de diferentes colores y atmósferas. La estructura de cada habitación es la misma: paredes blancas, pisos de madera clara en forma de espiga, ventanas francesas dobles del piso al techo y cortinas de gasa blancas, se refieren a<<<image_2_2>>>, pero el paisaje fuera de la ventana y la atmósfera interior son completamente diferentes. El protagonista se mueve a una velocidad constante durante todo el juego, atravesando cada puerta abierta en la pared.
0-5 segundos, la primera sala, el tema es la lucha cómica estadounidense, el protagonista entra a la sala y pelea con el personaje (<<<image_3_3>>>), el personaje pierde;
5-10 segundos, la segunda habitación, el tema es cálido, estilo fieltro, la escena fuera de la ventana es un campo de girasoles (<<<image_4_4>>>), la luz interior es de color naranja cálido y suave, y un pintor está pintando girasoles (<<<image_5_5>>>). El protagonista también cambia a un estilo sentido después de entrar;
10-15 segundos, la tercera habitación, el tema es la tristeza, toda la imagen tiene el estilo de una animación cómica stop-motion en blanco y negro, está lloviendo fuera de la ventana, la luz del interior es fría y gris, una persona está sentada sola en el suelo en el centro de la habitación vacía, agachando la cabeza y abrazando sus rodillas, y un teléfono móvil al lado ilumina la interfaz de llamada sin que nadie responda. Después de que el protagonista entra a la habitación, apaga las luces de la habitación e inmediatamente las enciende. La habitación se vuelve colorida y las flores crecen por toda la casa en un instante;
15-20 segundos, la cuarta sala, el tema es la alegría, toda la escena es una habitación empapada en el mar, consulte<<<image_6_6>>>, el protagonista nada hacia la habitación, con hermosos arrecifes de coral y bancos de peces a su lado;
20-25 segundos, la quinta habitación, el tema es sorpresa, la escena fuera de la ventana está llena de fuegos artificiales en el cielo nocturno, consulte<<<image_7_7>>>, la luz interior está coloreada y parpadea, y el protagonista está involucrado en la atmósfera alegre.
Después de 25-30 segundos, el protagonista finalmente llega a una habitación en blanco, se para en el centro y chasquea los dedos. Al mismo tiempo, el efecto de sonido es un chasquido, toda la pantalla está negra y la palabra "seedance" aparece en el medio; consulte<<<image_8_8>>>.
La calidad general de la película es un estilo publicitario de moda de alta gama. La luz está completamente determinada por la escena fuera de la ventana, creando un fuerte contraste emocional. No hay texto en la imagen.
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

### Case 14: Rompiendo los límites de la narrativa - 30 segundos de continuidad - salida - 2

[![Rompiendo los límites de la narrativa - 30 segundos de continuidad - salida - 2](assets/thumbnails/14-narrative-control-14-30-second-continuous-output-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab1/group2/output.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab1/group2/output.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 3

**Prompt:**

```text
Produzca un vídeo breve de divulgación científica de 30 segundos sobre los tres mil años de evolución del fútbol. Toda la película utiliza la misma pelota como línea visual principal. La bola rueda, viaja y se deforma desde la antigüedad, conectando diferentes civilizaciones y épocas. El ritmo general es compacto, los gráficos son de alta gama, el cortometraje de ciencia histórica se combina con transiciones artísticas para resaltar la sensación de una bola que abarca tres mil años y la transmisión oral es simple y poderosa.
Al principio, una bola antigua apareció lentamente desde un fondo negro con una textura del tiempo en la superficie, y luego rodó hacia una escena Cuju del Período de los Reinos Combatientes en China. La imagen se convirtió en un estilo de tinta, haciendo referencia al estilo de<<<image_1_1>>>. Los antiguos vestidos con trajes antiguos jugaban al Cuju en el patio con movimientos elegantes y la pelota rebotaba bajo sus pies. Transmisión oral: Historia de fútbol, ​​empezando por Cuju.
Luego, la pelota continúa rodando hacia adelante y la imagen pasa naturalmente a una escena de un juego de pelota griego antiguo. La imagen tiene el estilo de una pintura al óleo clásica y el estilo se refiere a<<<image_2_2>>>. El fondo de los pilares cuadrados y de piedra es obvio, y las personas vestidas con túnicas griegas antiguas juegan al fútbol. El panorama es denso e histórico. Boca a boca: a los griegos también les encantan los juegos de pelota.
Luego, el baile llegó a la Europa medieval y el cuadro aún conservaba el estilo de la pintura al óleo. Pueblos, campos de barro y gente corriente perseguían la pelota. El ambiente era cálido y áspero, como si el antiguo fútbol popular continuara con el fuego. Transmisión oral: los europeos continúan el partido de fútbol.
Luego patearon el balón y la pantalla cambió a un estilo documental en blanco y negro. Refiriéndose a<<<image_3_3>>>, llegamos a Inglaterra en 1863. Poco a poco aparecieron caballeros, clubes y campos de césped, que simbolizan el nacimiento oficial del fútbol moderno. Este balón mostró por primera vez el aspecto estándar del fútbol moderno. Hablado: 1863, el fútbol moderno toma forma.
Luego, la escena entra rápidamente en la era moderna, con la bola girando en el aire, sacando a la luz nodos clave de desarrollo. Las luces, el estadio, los espectadores, los trofeos y diferentes escenas alrededor del mundo se entrelazan, mostrando que el fútbol ha evolucionado de un deporte local a uno global.
Al final, el balón está en el centro de un estadio moderno, y multitudes y vítores de todo el mundo se funden en el fondo, creando la sensación de "un balón que conecta el mundo". La imagen es grandiosa y épica. Transmisión oral: Ahora el fútbol conecta al mundo entero.
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

### Case 15: Rompiendo los límites de la narrativa - 30 segundos de continuidad - salida - 3

[![Rompiendo los límites de la narrativa - 30 segundos de continuidad - salida - 3](assets/thumbnails/15-narrative-control-15-30-second-continuous-output-group-3.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab1/group3/output.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab1/group3/output.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 6

**Prompt:**

```text
Un vídeo tutorial de 30 segundos sobre cómo instalar y utilizar una máquina de café de cápsulas.
0-2 segundos, el texto del título al principio es: tutorial de instalación y uso de la máquina de café en cápsulas seedance
2-5 segundos, paso 1: instale el tanque de agua, consulte<<<image_1_1>>>Lente: Plano medio, vista ligeramente superior Posición: Acción en la parte posterior del fuselaje: Alinee el tanque de agua con la ranura en la parte posterior del fuselaje, empújelo verticalmente hacia abajo y escuche un sonido de "clic" para fijarlo en su lugar. Requisitos: muestre claramente la relación de alineación entre la hebilla en el fondo del tanque de agua y la ranura en el fuselaje, y la línea del nivel del agua se puede ver en la parte transparente del tanque de agua.
Narrador: "Primero, instale el tanque de agua".
5-9 segundos, paso 2: Instale la bandeja de goteo, consulte<<<image_2_2>>>Lente: Primer plano, vista frontal, Posición: Frente a la parte inferior del fuselaje, Acción: Empuje la bandeja de goteo dentro del riel guía en la parte inferior del fuselaje en paralelo, empújela hasta que la parte inferior esté completamente ajustada, Requisitos: Muestre el proceso de alineación del riel guía, resalte la suavidad de la acción de deslizamiento
Narrador: "A continuación, alinee la plataforma con los rieles inferiores".
9-13 segundos, paso 3: Instale la caja de recolección de cápsulas de desechos, consulte<<<image_3_3>>>Lente: Primer plano, ángulo de visión ligeramente elevado, Posición: Cavidad debajo de la bandeja de goteo, Acción: Alinee la caja de recolección con la ranura y empújela hacia adentro, al ras con la bandeja de goteo. Requisitos: mostrar la relación de ajuste entre la caja de recolección y el fuselaje y confirmar que esté instalado en su lugar
Narrador: "Entonces póngalo en la caja de recolección de cápsulas".
13-18 segundos, paso 4: primera inyección de agua, consulte<<<image_4_4>>>Lente: Primer plano, vista lateral, posición: tanque de agua en la parte superior/trasera del fuselaje, acción: abrir la tapa del tanque de agua, verter agua hasta el nivel MÁXIMO, cerrar la tapa del tanque de agua, requisitos: resaltar la marca del nivel de agua y el agua vertida es claramente visible
Narrador: "Abra la tapa del tanque de agua y vierta agua limpia. Tenga cuidado de no exceder el nivel máximo de agua".
La pantalla resalta el nivel máximo de agua.
18-25 segundos, paso 5: encendido, consulte<<<image_5_5>>>Toma: Plano medio, vista frontal, Posición: Frente del fuselaje, Acción: Conecte el cable de alimentación, presione el botón de encendido, la luz indicadora cambia de intermitente a fija (precalentamiento completado), Requisitos: Primer plano de los cambios de estado del botón de encendido y la luz indicadora, que refleja el proceso de espera hasta que esté listo
Narrador: "Conecte la corriente y presione el botón de encendido".
25-30 segundos, paso 6: primer enjuague (sin colocar la cápsula), consulte<<<image_6_6>>>Lente: plano medio a primer plano, vista frontal, posición: frente al fuselaje, taza debajo de la salida de agua, acción: presione el botón de extracción directamente sin insertar la cápsula, el agua caliente sale del tubo de lavado y el agua fluye hacia la taza. Requisitos: enfatice la marca de aviso "No es necesario colocar una cápsula" y muestre todo el proceso de eliminación del agua.
Narrador: "El último paso es enjuagar por primera vez. No es necesario introducir la cápsula, solo presiona el botón de extracción. Tu cafetera está lista para su uso oficial".
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

### Case 16: Ampliando los límites narrativos: más referencias Entrada-Salida-1

[![Ampliando los límites narrativos: más referencias Entrada-Salida-1](assets/thumbnails/16-narrative-control-16-multi-reference-input-group-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/output.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/output.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 17

**Prompt:**

```text
Instrucciones principales: un cortometraje narrativo de una sola toma de 26 segundos, con seguimiento y entrelazado estables, consulte<<<video_1_1>>>, y movimiento envolvente suave, consulte<<<video_2_2>>>. Sensación de viaje suave. La alternancia del día y la noche y el flujo de las cuatro estaciones se realizan dentro de la lente. La protagonista es una mujer europea<<<image_1_3>>>, situada en un mar de gente llena de fuegos artificiales, resaltando la máxima sensación de soledad y la calidad de la cinematografía.
Movimiento de cámara segmentado y descripción de la escena:
0-3 segundos (parte posterior suave): la vieja puerta de madera<<<image_2_4>>>se abre con un crujido y la cámara sigue la figura de una mujer europea vestida con<<<image_3_5>>>saliendo. Se detuvo levemente en el umbral. Las calles que había delante estaban moteadas de luces y sombras, y se acercaban sonidos de vendedores ambulantes y multitudes. Parecía distante y lentamente caminó hacia la calle.
3-6 segundos (toma de seguimiento posterior y lateral): la cámara mantiene un seguimiento fluido, ella camina hacia el concurrido mercado matutino, la atmósfera hace referencia a<<<video_3_6>>>. Los dos lados estaban llenos de coloridos puestos de frutas y tiendas de especias, y un grupo de malabaristas callejeros respiraban dragones de fuego, consulte<<<image_4_7>>>. La luz del fuego iluminó a la multitud, pero ella no entrecerró los ojos y caminó a paso firme.
6-9 segundos (envolvente suave desde el costado): la cámara comienza a girar suavemente hacia el costado y el frente, capturando la cara lateral del protagonista. Pasó por delante de la ruidosa carnicería<<<image_5_8>>>y una joven madre pasó junto a él con un bebé<<<image_6_9>>>en brazos. El bebé la miró con curiosidad, pero ella solo bajó un poco los ojos para evitar mirar, sin detenerse en absoluto.
9-12 segundos (disparo de seguimiento hacia adelante y hacia atrás): la cámara continúa dando vueltas directamente frente al protagonista y realiza disparos de seguimiento hacia atrás y hacia atrás. La multitud al frente de repente se retiró a ambos lados, naturalmente, como Moisés partiendo el mar. Un enorme elefante<<<image_7_10>>>cubierto con una hermosa tela roja apareció desde el lado derecho de la pantalla con un ritmo constante, ocupando la mayor parte de la pantalla.
12-15 segundos (penetración del espacio y rebobinado): en el momento en que la mujer y el elefante están a punto de chocar, la cámara se desliza hábilmente a través del estrecho espacio entre el elefante y la mujer, recirculando de regreso a su espalda. Los elefantes pasaban enormes y silenciosos, y los pilluelos los perseguían con alegría. Como campanas y risas, ni siquiera disminuyó la velocidad.
15-18 segundos (gradiente de luz ambiental y sombra): mientras camina, la luz y la sombra en el plano largo cambian mágicamente: la deslumbrante luz del sol en pleno verano se suaviza instantáneamente, una brisa enrolla las hojas doradas<<<video_2_2>>>0 en el cielo y la estación pasa sin problemas a finales de otoño en el mismo plano largo. Las hojas caídas le rozaron los hombros.
18-21 segundos (entorno inmersivo de 360 ​​grados): el frente cae repentinamente en una gran celebración callejera<<<video_2_2>>>1. Cintas de colores y papel triturado estallaron en el aire y los vendedores se inclinaron para vitorear. En ese momento, la cámara despliega un movimiento panorámico continuo de 360 ​​grados, creando un desgarro visual extremadamente fuerte entre el silencioso y solitario protagonista y el frenético entorno.
21-24 segundos (dando vueltas hacia un lado y hacia atrás): cuando la cámara dio vueltas y regresó a su lado y atrás, las cintas que caían se habían convertido silenciosamente en nieve por todo el cielo: era invierno en un instante<<<video_2_2>>>2. Los peatones sostenían paraguas o se pusieron capuchas, y las mujeres se encogieron ligeramente, se subieron el cuello de los abrigos, se pusieron<<<video_2_2>>>3 y continuaron caminando solas en la nieve.
24-26 segundos (empuje lento y ritmo): mientras caminaba hacia el final de la larga calle, el cielo se oscureció a una velocidad visible a simple vista y el día se hundió sin problemas en la noche. Las tenues luces de la calle a ambos lados y las bombillas de los puestos se encendieron una tras otra<<<video_2_2>>>4. Los vendedores estaban empacando sus mercancías. El ruido pareció ser absorbido lentamente y distante por la fuerte nieve, y sus pasos disminuyeron gradualmente. Grandes fuegos artificiales florecieron repentinamente en el cielo nocturno<<<video_2_2>>>5, el sonido de los fuegos artificiales floreciendo se refiere a<<<video_2_2>>>6. Puntos de luz de colores parpadeaban y saltaban en las paredes del edificio y en sus ojos. El mundo todavía está animado, pero ella mira hacia arriba en silencio, la cámara se aleja lentamente y termina aquí suavemente.
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

### Case 17: Rompiendo los límites de la narrativa-más entradas de referencia-video de referencia-1-1

[![Rompiendo los límites de la narrativa-más entradas de referencia-video de referencia-1-1](assets/thumbnails/17-reference-asset-17-multi-reference-input-group-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/reference1.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/reference1.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 17

**Prompt:**

```text
Instrucciones principales: un cortometraje narrativo de una sola toma de 26 segundos, con seguimiento y entrelazado estables, consulte<<<video_1_1>>>, y movimiento envolvente suave, consulte<<<video_2_2>>>. Sensación de viaje suave. La alternancia del día y la noche y el flujo de las cuatro estaciones se realizan dentro de la lente. La protagonista es una mujer europea<<<image_1_3>>>, situada en un mar de gente llena de fuegos artificiales, resaltando la máxima sensación de soledad y la calidad de la cinematografía.
Movimiento de cámara segmentado y descripción de la escena:
0-3 segundos (parte posterior suave): la vieja puerta de madera<<<image_2_4>>>se abre con un crujido y la cámara sigue la figura de una mujer europea vestida con<<<image_3_5>>>saliendo. Se detuvo levemente en el umbral. Las calles que había delante estaban moteadas de luces y sombras, y se acercaban sonidos de vendedores ambulantes y multitudes. Parecía distante y lentamente caminó hacia la calle.
3-6 segundos (toma de seguimiento posterior y lateral): la cámara mantiene un seguimiento fluido, ella camina hacia el concurrido mercado matutino, la atmósfera hace referencia a<<<video_3_6>>>. Los dos lados estaban llenos de coloridos puestos de frutas y tiendas de especias, y un grupo de malabaristas callejeros respiraban dragones de fuego, consulte<<<image_4_7>>>. La luz del fuego iluminó a la multitud, pero ella no entrecerró los ojos y caminó a paso firme.
6-9 segundos (envolvente suave desde el costado): la cámara comienza a girar suavemente hacia el costado y el frente, capturando la cara lateral del protagonista. Pasó por delante de la ruidosa carnicería<<<image_5_8>>>y una joven madre pasó junto a él con un bebé<<<image_6_9>>>en brazos. El bebé la miró con curiosidad, pero ella solo bajó un poco los ojos para evitar mirar, sin detenerse en absoluto.
9-12 segundos (disparo de seguimiento hacia adelante y hacia atrás): la cámara continúa dando vueltas directamente frente al protagonista y realiza disparos de seguimiento hacia atrás y hacia atrás. La multitud al frente de repente se retiró a ambos lados, naturalmente, como Moisés partiendo el mar. Un enorme elefante<<<image_7_10>>>cubierto con una hermosa tela roja apareció desde el lado derecho de la pantalla con un ritmo constante, ocupando la mayor parte de la pantalla.
12-15 segundos (penetración del espacio y rebobinado): en el momento en que la mujer y el elefante están a punto de chocar, la cámara se desliza hábilmente a través del estrecho espacio entre el elefante y la mujer, recirculando de regreso a su espalda. Los elefantes pasaban enormes y silenciosos, y los pilluelos los perseguían con alegría. Como campanas y risas, ni siquiera disminuyó la velocidad.
15-18 segundos (gradiente de luz ambiental y sombra): mientras camina, la luz y la sombra en el plano largo cambian mágicamente: la deslumbrante luz del sol en pleno verano se suaviza instantáneamente, una brisa enrolla las hojas doradas<<<video_2_2>>>0 en el cielo y la estación pasa sin problemas a finales de otoño en el mismo plano largo. Las hojas caídas le rozaron los hombros.
18-21 segundos (entorno inmersivo de 360 ​​grados): el frente cae repentinamente en una gran celebración callejera<<<video_2_2>>>1. Cintas de colores y papel triturado estallaron en el aire y los vendedores se inclinaron para vitorear. En ese momento, la cámara despliega un movimiento panorámico continuo de 360 ​​grados, creando un desgarro visual extremadamente fuerte entre el silencioso y solitario protagonista y el frenético entorno.
21-24 segundos (dando vueltas hacia un lado y hacia atrás): cuando la cámara dio vueltas y regresó a su lado y atrás, las cintas que caían se habían convertido silenciosamente en nieve por todo el cielo: era invierno en un instante<<<video_2_2>>>2. Los peatones sostenían paraguas o se pusieron capuchas, y las mujeres se encogieron ligeramente, se subieron el cuello de los abrigos, se pusieron<<<video_2_2>>>3 y continuaron caminando solas en la nieve.
24-26 segundos (empuje lento y ritmo): mientras caminaba hacia el final de la larga calle, el cielo se oscureció a una velocidad visible a simple vista y el día se hundió sin problemas en la noche. Las tenues luces de la calle a ambos lados y las bombillas de los puestos se encendieron una tras otra<<<video_2_2>>>4. Los vendedores estaban empacando sus mercancías. El ruido pareció ser absorbido lentamente y distante por la fuerte nieve, y sus pasos disminuyeron gradualmente. Grandes fuegos artificiales florecieron repentinamente en el cielo nocturno<<<video_2_2>>>5, el sonido de los fuegos artificiales floreciendo se refiere a<<<video_2_2>>>6. Puntos de luz de colores parpadeaban y saltaban en las paredes del edificio y en sus ojos. El mundo todavía está animado, pero ella mira hacia arriba en silencio, la cámara se aleja lentamente y termina aquí suavemente.
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

### Case 18: Rompiendo los límites de la narrativa-más entradas de referencia-video de referencia-1-2

[![Rompiendo los límites de la narrativa-más entradas de referencia-video de referencia-1-2](assets/thumbnails/18-reference-asset-18-multi-reference-input-group-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/reference2.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/reference2.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 17

**Prompt:**

```text
Instrucciones principales: un cortometraje narrativo de una sola toma de 26 segundos, con seguimiento y entrelazado estables, consulte<<<video_1_1>>>, y movimiento envolvente suave, consulte<<<video_2_2>>>. Sensación de viaje suave. La alternancia del día y la noche y el flujo de las cuatro estaciones se realizan dentro de la lente. La protagonista es una mujer europea<<<image_1_3>>>, situada en un mar de gente llena de fuegos artificiales, resaltando la máxima sensación de soledad y la calidad de la cinematografía.
Movimiento de cámara segmentado y descripción de la escena:
0-3 segundos (parte posterior suave): la vieja puerta de madera<<<image_2_4>>>se abre con un crujido y la cámara sigue la figura de una mujer europea vestida con<<<image_3_5>>>saliendo. Se detuvo levemente en el umbral. Las calles que había delante estaban moteadas de luces y sombras, y se acercaban sonidos de vendedores ambulantes y multitudes. Parecía distante y lentamente caminó hacia la calle.
3-6 segundos (toma de seguimiento posterior y lateral): la cámara mantiene un seguimiento fluido, ella camina hacia el concurrido mercado matutino, la atmósfera hace referencia a<<<video_3_6>>>. Los dos lados estaban llenos de coloridos puestos de frutas y tiendas de especias, y un grupo de malabaristas callejeros respiraban dragones de fuego, consulte<<<image_4_7>>>. La luz del fuego iluminó a la multitud, pero ella no entrecerró los ojos y caminó a paso firme.
6-9 segundos (envolvente suave desde el costado): la cámara comienza a girar suavemente hacia el costado y el frente, capturando la cara lateral del protagonista. Pasó por delante de la ruidosa carnicería<<<image_5_8>>>y una joven madre pasó junto a él con un bebé<<<image_6_9>>>en brazos. El bebé la miró con curiosidad, pero ella solo bajó un poco los ojos para evitar mirar, sin detenerse en absoluto.
9-12 segundos (disparo de seguimiento hacia adelante y hacia atrás): la cámara continúa dando vueltas directamente frente al protagonista y realiza disparos de seguimiento hacia atrás y hacia atrás. La multitud al frente de repente se retiró a ambos lados, naturalmente, como Moisés partiendo el mar. Un enorme elefante<<<image_7_10>>>cubierto con una hermosa tela roja apareció desde el lado derecho de la pantalla con un ritmo constante, ocupando la mayor parte de la pantalla.
12-15 segundos (penetración del espacio y rebobinado): en el momento en que la mujer y el elefante están a punto de chocar, la cámara se desliza hábilmente a través del estrecho espacio entre el elefante y la mujer, recirculando de regreso a su espalda. Los elefantes pasaban enormes y silenciosos, y los pilluelos los perseguían con alegría. Como campanas y risas, ni siquiera disminuyó la velocidad.
15-18 segundos (gradiente de luz ambiental y sombra): mientras camina, la luz y la sombra en el plano largo cambian mágicamente: la deslumbrante luz del sol en pleno verano se suaviza instantáneamente, una brisa enrolla las hojas doradas<<<video_2_2>>>0 en el cielo y la estación pasa sin problemas a finales de otoño en el mismo plano largo. Las hojas caídas le rozaron los hombros.
18-21 segundos (entorno inmersivo de 360 ​​grados): el frente cae repentinamente en una gran celebración callejera<<<video_2_2>>>1. Cintas de colores y papel triturado estallaron en el aire y los vendedores se inclinaron para vitorear. En ese momento, la cámara despliega un movimiento panorámico continuo de 360 ​​grados, creando un desgarro visual extremadamente fuerte entre el silencioso y solitario protagonista y el frenético entorno.
21-24 segundos (dando vueltas hacia un lado y hacia atrás): cuando la cámara dio vueltas y regresó a su lado y atrás, las cintas que caían se habían convertido silenciosamente en nieve por todo el cielo: era invierno en un instante<<<video_2_2>>>2. Los peatones sostenían paraguas o se pusieron capuchas, y las mujeres se encogieron ligeramente, se subieron el cuello de los abrigos, se pusieron<<<video_2_2>>>3 y continuaron caminando solas en la nieve.
24-26 segundos (empuje lento y ritmo): mientras caminaba hacia el final de la larga calle, el cielo se oscureció a una velocidad visible a simple vista y el día se hundió sin problemas en la noche. Las tenues luces de la calle a ambos lados y las bombillas de los puestos se encendieron una tras otra<<<video_2_2>>>4. Los vendedores estaban empacando sus mercancías. El ruido pareció ser absorbido lentamente y distante por la fuerte nieve, y sus pasos disminuyeron gradualmente. Grandes fuegos artificiales florecieron repentinamente en el cielo nocturno<<<video_2_2>>>5, el sonido de los fuegos artificiales floreciendo se refiere a<<<video_2_2>>>6. Puntos de luz de colores parpadeaban y saltaban en las paredes del edificio y en sus ojos. El mundo todavía está animado, pero ella mira hacia arriba en silencio, la cámara se aleja lentamente y termina aquí suavemente.
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

### Case 19: Rompiendo los límites de la narrativa-más entradas de referencia-video de referencia-1-6

[![Rompiendo los límites de la narrativa-más entradas de referencia-video de referencia-1-6](assets/thumbnails/19-reference-asset-19-multi-reference-input-group-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/reference6.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/reference6.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 17

**Prompt:**

```text
Instrucciones principales: un cortometraje narrativo de una sola toma de 26 segundos, con seguimiento y entrelazado estables, consulte<<<video_1_1>>>, y movimiento envolvente suave, consulte<<<video_2_2>>>. Sensación de viaje suave. La alternancia del día y la noche y el flujo de las cuatro estaciones se realizan dentro de la lente. La protagonista es una mujer europea<<<image_1_3>>>, situada en un mar de gente llena de fuegos artificiales, resaltando la máxima sensación de soledad y la calidad de la cinematografía.
Movimiento de cámara segmentado y descripción de la escena:
0-3 segundos (parte posterior suave): la vieja puerta de madera<<<image_2_4>>>se abre con un crujido y la cámara sigue la figura de una mujer europea vestida con<<<image_3_5>>>saliendo. Se detuvo levemente en el umbral. Las calles que había delante estaban moteadas de luces y sombras, y se acercaban sonidos de vendedores ambulantes y multitudes. Parecía distante y lentamente caminó hacia la calle.
3-6 segundos (toma de seguimiento posterior y lateral): la cámara mantiene un seguimiento fluido, ella camina hacia el concurrido mercado matutino, la atmósfera hace referencia a<<<video_3_6>>>. Los dos lados estaban llenos de coloridos puestos de frutas y tiendas de especias, y un grupo de malabaristas callejeros respiraban dragones de fuego, consulte<<<image_4_7>>>. La luz del fuego iluminó a la multitud, pero ella no entrecerró los ojos y caminó a paso firme.
6-9 segundos (envolvente suave desde el costado): la cámara comienza a girar suavemente hacia el costado y el frente, capturando la cara lateral del protagonista. Pasó por delante de la ruidosa carnicería<<<image_5_8>>>y una joven madre pasó junto a él con un bebé<<<image_6_9>>>en brazos. El bebé la miró con curiosidad, pero ella solo bajó un poco los ojos para evitar mirar, sin detenerse en absoluto.
9-12 segundos (disparo de seguimiento hacia adelante y hacia atrás): la cámara continúa dando vueltas directamente frente al protagonista y realiza disparos de seguimiento hacia atrás y hacia atrás. La multitud al frente de repente se retiró a ambos lados, naturalmente, como Moisés partiendo el mar. Un enorme elefante<<<image_7_10>>>cubierto con una hermosa tela roja apareció desde el lado derecho de la pantalla con un ritmo constante, ocupando la mayor parte de la pantalla.
12-15 segundos (penetración del espacio y rebobinado): en el momento en que la mujer y el elefante están a punto de chocar, la cámara se desliza hábilmente a través del estrecho espacio entre el elefante y la mujer, recirculando de regreso a su espalda. Los elefantes pasaban enormes y silenciosos, y los pilluelos los perseguían con alegría. Como campanas y risas, ni siquiera disminuyó la velocidad.
15-18 segundos (gradiente de luz ambiental y sombra): mientras camina, la luz y la sombra en el plano largo cambian mágicamente: la deslumbrante luz del sol en pleno verano se suaviza instantáneamente, una brisa enrolla las hojas doradas<<<video_2_2>>>0 en el cielo y la estación pasa sin problemas a finales de otoño en el mismo plano largo. Las hojas caídas le rozaron los hombros.
18-21 segundos (entorno inmersivo de 360 ​​grados): el frente cae repentinamente en una gran celebración callejera<<<video_2_2>>>1. Cintas de colores y papel triturado estallaron en el aire y los vendedores se inclinaron para vitorear. En ese momento, la cámara despliega un movimiento panorámico continuo de 360 ​​grados, creando un desgarro visual extremadamente fuerte entre el silencioso y solitario protagonista y el frenético entorno.
21-24 segundos (dando vueltas hacia un lado y hacia atrás): cuando la cámara dio vueltas y regresó a su lado y atrás, las cintas que caían se habían convertido silenciosamente en nieve por todo el cielo: era invierno en un instante<<<video_2_2>>>2. Los peatones sostenían paraguas o se pusieron capuchas, y las mujeres se encogieron ligeramente, se subieron el cuello de los abrigos, se pusieron<<<video_2_2>>>3 y continuaron caminando solas en la nieve.
24-26 segundos (empuje lento y ritmo): mientras caminaba hacia el final de la larga calle, el cielo se oscureció a una velocidad visible a simple vista y el día se hundió sin problemas en la noche. Las tenues luces de la calle a ambos lados y las bombillas de los puestos se encendieron una tras otra<<<video_2_2>>>4. Los vendedores estaban empacando sus mercancías. El ruido pareció ser absorbido lentamente y distante por la fuerte nieve, y sus pasos disminuyeron gradualmente. Grandes fuegos artificiales florecieron repentinamente en el cielo nocturno<<<video_2_2>>>5, el sonido de los fuegos artificiales floreciendo se refiere a<<<video_2_2>>>6. Puntos de luz de colores parpadeaban y saltaban en las paredes del edificio y en sus ojos. El mundo todavía está animado, pero ella mira hacia arriba en silencio, la cámara se aleja lentamente y termina aquí suavemente.
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

### Case 20: Ampliando los límites narrativos: más referencias Entrada-Salida-2

[![Ampliando los límites narrativos: más referencias Entrada-Salida-2](assets/thumbnails/20-narrative-control-20-multi-reference-input-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/output.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/output.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 7

**Prompt:**

```text
El estilo del comercial es brillante y colorido, con galletas frutales como protagonistas, incluidos cuatro sabores: fresa, manzana, uva y naranja. El sabor a fresa hace referencia a<<<image_1_1>>>. Las galletas y las frutas correspondientes están dispuestas en una disposición geométrica con un fuerte sentido de orden. El panorama general es limpio, avanzado y rítmico. La fruta inicial establece rápidamente un enfoque visual, haciendo referencia a la composición de<<<video_1_2>>>, y se vuelve a tocar la música. Luego, las galletas de diferentes sabores se organizan cuidadosamente y se cortan en primeros planos, haciendo referencia a la dinámica y los movimientos de cámara de<<<video_2_3>>>. Durante el clímax, una galleta se rompe y instantáneamente entra en cámara lenta. El sándwich de frutas explota, las migas vuelan y el jugo y el impacto de las partículas se magnifican y muestran. Consulte el impacto de<<<video_3_4>>>. La matriz horizontal forma una parábola rítmica, que hace referencia al movimiento de<<<video_4_5>>>, resaltando la belleza del orden y la riqueza del producto. Luego regrese rápidamente a la edición acelerada. El texto final en inglés Un bocado de frescura, un corazón lleno de deleite cambia rápidamente a la imagen, combinado con el fuerte movimiento rítmico del texto y el cuadro congelado del producto, consulte<<<video_5_6>>>, y finalmente el sentido de la marca se envuelve y las galletas y frutas se extienden en todas direcciones, consulte<<<video_6_7>>>. La imagen está llena de gente joven, enérgica, deliciosa y con ganas de compartir un ambiente publicitario.
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

### Case 21: Rompiendo los límites de la narrativa-más entradas de referencia-video de referencia-2-2

[![Rompiendo los límites de la narrativa-más entradas de referencia-video de referencia-2-2](assets/thumbnails/21-reference-asset-21-multi-reference-input-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference2.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference2.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 7

**Prompt:**

```text
El estilo del comercial es brillante y colorido, con galletas frutales como protagonistas, incluidos cuatro sabores: fresa, manzana, uva y naranja. El sabor a fresa hace referencia a<<<image_1_1>>>. Las galletas y las frutas correspondientes están dispuestas en una disposición geométrica con un fuerte sentido de orden. El panorama general es limpio, avanzado y rítmico. La fruta inicial establece rápidamente un enfoque visual, haciendo referencia a la composición de<<<video_1_2>>>, y se vuelve a tocar la música. Luego, las galletas de diferentes sabores se organizan cuidadosamente y se cortan en primeros planos, haciendo referencia a la dinámica y los movimientos de cámara de<<<video_2_3>>>. Durante el clímax, una galleta se rompe y instantáneamente entra en cámara lenta. El sándwich de frutas explota, las migas vuelan y el jugo y el impacto de las partículas se magnifican y muestran. Consulte el impacto de<<<video_3_4>>>. La matriz horizontal forma una parábola rítmica, que hace referencia al movimiento de<<<video_4_5>>>, resaltando la belleza del orden y la riqueza del producto. Luego regrese rápidamente a la edición acelerada. El texto final en inglés Un bocado de frescura, un corazón lleno de deleite cambia rápidamente a la imagen, combinado con el fuerte movimiento rítmico del texto y el cuadro congelado del producto, consulte<<<video_5_6>>>, y finalmente el sentido de la marca se envuelve y las galletas y frutas se extienden en todas direcciones, consulte<<<video_6_7>>>. La imagen está llena de gente joven, enérgica, deliciosa y con ganas de compartir un ambiente publicitario.
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

### Case 22: Rompiendo los límites de la narrativa-más entradas de referencia-video de referencia-2-3

[![Rompiendo los límites de la narrativa-más entradas de referencia-video de referencia-2-3](assets/thumbnails/22-reference-asset-22-multi-reference-input-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference3.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference3.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 7

**Prompt:**

```text
El estilo del comercial es brillante y colorido, con galletas frutales como protagonistas, incluidos cuatro sabores: fresa, manzana, uva y naranja. El sabor a fresa hace referencia a<<<image_1_1>>>. Las galletas y las frutas correspondientes están dispuestas en una disposición geométrica con un fuerte sentido de orden. El panorama general es limpio, avanzado y rítmico. La fruta inicial establece rápidamente un enfoque visual, haciendo referencia a la composición de<<<video_1_2>>>, y se vuelve a tocar la música. Luego, las galletas de diferentes sabores se organizan cuidadosamente y se cortan en primeros planos, haciendo referencia a la dinámica y los movimientos de cámara de<<<video_2_3>>>. Durante el clímax, una galleta se rompe y instantáneamente entra en cámara lenta. El sándwich de frutas explota, las migas vuelan y el jugo y el impacto de las partículas se magnifican y muestran. Consulte el impacto de<<<video_3_4>>>. La matriz horizontal forma una parábola rítmica, que hace referencia al movimiento de<<<video_4_5>>>, resaltando la belleza del orden y la riqueza del producto. Luego regrese rápidamente a la edición acelerada. El texto final en inglés Un bocado de frescura, un corazón lleno de deleite cambia rápidamente a la imagen, combinado con el fuerte movimiento rítmico del texto y el cuadro congelado del producto, consulte<<<video_5_6>>>, y finalmente el sentido de la marca se envuelve y las galletas y frutas se extienden en todas direcciones, consulte<<<video_6_7>>>. La imagen está llena de gente joven, enérgica, deliciosa y con ganas de compartir un ambiente publicitario.
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

### Case 23: Rompiendo los límites de la narrativa-más entradas de referencia-video de referencia-2-4

[![Rompiendo los límites de la narrativa-más entradas de referencia-video de referencia-2-4](assets/thumbnails/23-reference-asset-23-multi-reference-input-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference4.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference4.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 7

**Prompt:**

```text
El estilo del comercial es brillante y colorido, con galletas frutales como protagonistas, incluidos cuatro sabores: fresa, manzana, uva y naranja. El sabor a fresa hace referencia a<<<image_1_1>>>. Las galletas y las frutas correspondientes están dispuestas en una disposición geométrica con un fuerte sentido de orden. El panorama general es limpio, avanzado y rítmico. La fruta inicial establece rápidamente un enfoque visual, haciendo referencia a la composición de<<<video_1_2>>>, y se vuelve a tocar la música. Luego, las galletas de diferentes sabores se organizan cuidadosamente y se cortan en primeros planos, haciendo referencia a la dinámica y los movimientos de cámara de<<<video_2_3>>>. Durante el clímax, una galleta se rompe y instantáneamente entra en cámara lenta. El sándwich de frutas explota, las migas vuelan y el jugo y el impacto de las partículas se magnifican y muestran. Consulte el impacto de<<<video_3_4>>>. La matriz horizontal forma una parábola rítmica, que hace referencia al movimiento de<<<video_4_5>>>, resaltando la belleza del orden y la riqueza del producto. Luego regrese rápidamente a la edición acelerada. El texto final en inglés Un bocado de frescura, un corazón lleno de deleite cambia rápidamente a la imagen, combinado con el fuerte movimiento rítmico del texto y el cuadro congelado del producto, consulte<<<video_5_6>>>, y finalmente el sentido de la marca se envuelve y las galletas y frutas se extienden en todas direcciones, consulte<<<video_6_7>>>. La imagen está llena de gente joven, enérgica, deliciosa y con ganas de compartir un ambiente publicitario.
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

### Case 24: Rompiendo los límites de la narrativa-más entradas de referencia-video de referencia-2-5

[![Rompiendo los límites de la narrativa-más entradas de referencia-video de referencia-2-5](assets/thumbnails/24-reference-asset-24-multi-reference-input-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference5.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference5.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 7

**Prompt:**

```text
El estilo del comercial es brillante y colorido, con galletas frutales como protagonistas, incluidos cuatro sabores: fresa, manzana, uva y naranja. El sabor a fresa hace referencia a<<<image_1_1>>>. Las galletas y las frutas correspondientes están dispuestas en una disposición geométrica con un fuerte sentido de orden. El panorama general es limpio, avanzado y rítmico. La fruta inicial establece rápidamente un enfoque visual, haciendo referencia a la composición de<<<video_1_2>>>, y se vuelve a tocar la música. Luego, las galletas de diferentes sabores se organizan cuidadosamente y se cortan en primeros planos, haciendo referencia a la dinámica y los movimientos de cámara de<<<video_2_3>>>. Durante el clímax, una galleta se rompe y instantáneamente entra en cámara lenta. El sándwich de frutas explota, las migas vuelan y el jugo y el impacto de las partículas se magnifican y muestran. Consulte el impacto de<<<video_3_4>>>. La matriz horizontal forma una parábola rítmica, que hace referencia al movimiento de<<<video_4_5>>>, resaltando la belleza del orden y la riqueza del producto. Luego regrese rápidamente a la edición acelerada. El texto final en inglés Un bocado de frescura, un corazón lleno de deleite cambia rápidamente a la imagen, combinado con el fuerte movimiento rítmico del texto y el cuadro congelado del producto, consulte<<<video_5_6>>>, y finalmente el sentido de la marca se envuelve y las galletas y frutas se extienden en todas direcciones, consulte<<<video_6_7>>>. La imagen está llena de gente joven, enérgica, deliciosa y con ganas de compartir un ambiente publicitario.
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

### Case 25: Rompiendo los límites de la narrativa-más entradas de referencia-video de referencia-2-6

[![Rompiendo los límites de la narrativa-más entradas de referencia-video de referencia-2-6](assets/thumbnails/25-reference-asset-25-multi-reference-input-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference6.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference6.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 7

**Prompt:**

```text
El estilo del comercial es brillante y colorido, con galletas frutales como protagonistas, incluidos cuatro sabores: fresa, manzana, uva y naranja. El sabor a fresa hace referencia a<<<image_1_1>>>. Las galletas y las frutas correspondientes están dispuestas en una disposición geométrica con un fuerte sentido de orden. El panorama general es limpio, avanzado y rítmico. La fruta inicial establece rápidamente un enfoque visual, haciendo referencia a la composición de<<<video_1_2>>>, y se vuelve a tocar la música. Luego, las galletas de diferentes sabores se organizan cuidadosamente y se cortan en primeros planos, haciendo referencia a la dinámica y los movimientos de cámara de<<<video_2_3>>>. Durante el clímax, una galleta se rompe y instantáneamente entra en cámara lenta. El sándwich de frutas explota, las migas vuelan y el jugo y el impacto de las partículas se magnifican y muestran. Consulte el impacto de<<<video_3_4>>>. La matriz horizontal forma una parábola rítmica, que hace referencia al movimiento de<<<video_4_5>>>, resaltando la belleza del orden y la riqueza del producto. Luego regrese rápidamente a la edición acelerada. El texto final en inglés Un bocado de frescura, un corazón lleno de deleite cambia rápidamente a la imagen, combinado con el fuerte movimiento rítmico del texto y el cuadro congelado del producto, consulte<<<video_5_6>>>, y finalmente el sentido de la marca se envuelve y las galletas y frutas se extienden en todas direcciones, consulte<<<video_6_7>>>. La imagen está llena de gente joven, enérgica, deliciosa y con ganas de compartir un ambiente publicitario.
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

### Case 26: Rompiendo los límites de la narrativa-más entradas de referencia-video de referencia-2-7

[![Rompiendo los límites de la narrativa-más entradas de referencia-video de referencia-2-7](assets/thumbnails/26-reference-asset-26-multi-reference-input-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference7.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference7.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 7

**Prompt:**

```text
El estilo del comercial es brillante y colorido, con galletas frutales como protagonistas, incluidos cuatro sabores: fresa, manzana, uva y naranja. El sabor a fresa hace referencia a<<<image_1_1>>>. Las galletas y las frutas correspondientes están dispuestas en una disposición geométrica con un fuerte sentido de orden. El panorama general es limpio, avanzado y rítmico. La fruta inicial establece rápidamente un enfoque visual, haciendo referencia a la composición de<<<video_1_2>>>, y se vuelve a tocar la música. Luego, las galletas de diferentes sabores se organizan cuidadosamente y se cortan en primeros planos, haciendo referencia a la dinámica y los movimientos de cámara de<<<video_2_3>>>. Durante el clímax, una galleta se rompe y instantáneamente entra en cámara lenta. El sándwich de frutas explota, las migas vuelan y el jugo y el impacto de las partículas se magnifican y muestran. Consulte el impacto de<<<video_3_4>>>. La matriz horizontal forma una parábola rítmica, que hace referencia al movimiento de<<<video_4_5>>>, resaltando la belleza del orden y la riqueza del producto. Luego regrese rápidamente a la edición acelerada. El texto final en inglés Un bocado de frescura, un corazón lleno de deleite cambia rápidamente a la imagen, combinado con el fuerte movimiento rítmico del texto y el cuadro congelado del producto, consulte<<<video_5_6>>>, y finalmente el sentido de la marca se envuelve y las galletas y frutas se extienden en todas direcciones, consulte<<<video_6_7>>>. La imagen está llena de gente joven, enérgica, deliciosa y con ganas de compartir un ambiente publicitario.
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

### Case 27: Rompiendo los límites de la narrativa-segundo nivel de control de pantalla-salida-1

[![Rompiendo los límites de la narrativa-segundo nivel de control de pantalla-salida-1](assets/thumbnails/27-narrative-control-27-second-level-frame-control-group-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab3/group1/output.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab3/group1/output.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 1

**Prompt:**

```text
El estilo publicitario de animación 3D, los colores brillantes y transparentes, y la pulpa y el jugo deben tener una fuerte sensación de frescura e impacto. El temperamento general es como el de un cortometraje de animación comercial de alta calidad con un poco de humor exagerado. El personaje del lagarto cornudo del desierto es lindo, inteligente y expresivo. Consulte<<<image_1_1>>>. La textura de la imagen se refiere a la suave luz natural, la fina textura de la piel y la pelusa, la macro profundidad de campo de ensueño y una sensación realmente infantil en la imagen.
0-3 segundos: la imagen muestra un desierto expuesto al sol abrasador. El aire estaba distorsionado por el calor, la arena estaba caliente y parecía que el humo se elevaba a lo lejos. Un lagarto cornudo del desierto yacía sobre la arena caliente, con la lengua ligeramente colgando y los ojos desenfocados, casi secándose al sol. Dio dos pasos y se balanceó, y todo el lagarto cornudo del desierto estuvo a punto de "evaporarse".
Los efectos de sonido incluyen el zumbido de las olas de calor y un crujido seco ligeramente exagerado.
3-6 segundos: El lagarto cornudo del desierto se detiene repentinamente y mueve la nariz. Miró hacia abajo y vio un pomelo frío y regordete con gotas de agua enterradas en la arena. El pomelo brilla intensamente al sol, con una piel delicada, como un milagro aparecido de repente en el desierto.
Los ojos del lagarto actor se abrieron instantáneamente, como si viera una pajita que le salvara la vida.
El efecto de sonido "ding" es un efecto de sonido de descubrimiento.
6-8 segundos: el lagarto cornudo del desierto se abalanza, abraza el pomelo con ambas manos y presiona toda su cara contra la cáscara. Tiene una expresión feliz de "por fin vivo". La imagen se congela durante 1 segundo, formando un punto de recuerdo publicitario exagerado y divertido.
El efecto de sonido desapareció y luego quedó en silencio durante medio segundo.
Segundos 8-11: Captura de pantalla de un lagarto cornudo del desierto agarrando una toronja. La piel del pomelo está abierta y la pulpa del interior brilla de forma translúcida. Al momento siguiente, el jugo no salió, sino que salió como un tsunami.
El efecto de sonido es un sonido de "clic" al abrir un mordisco, seguido de un sonido exagerado de jugo al estallar.
11-16 segundos: La pantalla muestra jugo de toronja de color rosa anaranjado, claro y brillante, derramándose locamente, cayendo por las dunas de arena e inundando rápidamente todo el desierto. La arena amarilla seca se transforma instantáneamente en un océano de verano fresco, chispeante y afrutado. Los cactus, las piedras y las pequeñas dunas de arena del desierto quedan engullidos por las olas de jugo, y la imagen es exagerada y soñadora.
La actuación del Lagarto Cornudo del Desierto fue muy emocionante al principio, pero al segundo siguiente me di cuenta de que algo andaba mal y mi expresión cambió de la sorpresa al horror.
16-20 segundos: el lagarto cornudo del desierto está casi sumergido en el "mar de pomelo". Rápidamente abraza la mitad del pomelo y flota en el mar como un aro salvavidas. Sacó la cabeza húmeda, con expresión confusa. La superficie del mar brilla, el color es como el jugo iluminado por el sol.
Los efectos de sonido exageran el sonido de los aleteos y las olas, con un sentido de comedia.
20-23 segundos: la pantalla cambia repentinamente a una pantalla blanca. En el centro de la pantalla aparecía el nombre de la marca y el eslogan: "Pomelo sembrado, lo que se muerde es la pulpa, lo que sale es verano".
El narrador lee la frase completa: "Siembra pomelo, lo que muerdes es la pulpa, lo que sale es verano".
Tono de marca con sonido limpio y refrescante.
23-29 segundos: la pantalla vuelve a la pantalla blanca. El lagarto cornudo del desierto ya está sentado tranquilamente sobre una toronja flotante, con un par de pequeñas gafas de sol, sosteniendo una taza para sorber y flotando lentamente en el "mar de jugo" para pasar las vacaciones. Pulpa de naranja, pequeños cubitos de hielo y salpicaduras de agua fría flotaban, el cielo se volvió azul y la atmósfera cambió repentinamente de "supervivencia" a "vacaciones". Al final, el lagarto cornudo del desierto descansó contento sobre la toronja y la cámara se alejó, congelándose en una escena de verano refrescante, brillante y divertida.
Efectos de sonido relajantes, música de verano, el sonido de las olas.
Los subtítulos sólo pueden conservar el nombre de la marca, sin añadir demasiadas palabras.
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

### Case 28: Rompiendo los límites de la narrativa-control de pantalla de segundo nivel-salida-2

[![Rompiendo los límites de la narrativa-control de pantalla de segundo nivel-salida-2](assets/thumbnails/28-narrative-control-28-second-level-frame-control-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab3/group2/output.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab3/group2/output.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 1

**Prompt:**

```text
Cortometraje cinematográfico de carreras juveniles de 30 segundos, estilo animación 2d. El protagonista es un joven conductor que conduce una motocicleta para participar en competiciones de alto nivel. El estilo general es apasionado, juvenil, emocionalmente intenso y cinematográfico, con un comienzo, una transición y un arco emocional claros y completos. En toda la película sólo se utilizan dos tipos de movimientos de cámara: seguimiento de alta velocidad y sonido envolvente en cámara lenta. Hay muy pocas líneas y aparecen naturalmente como fragmentos de memoria. El tono es sincero, gentil y comedido, sin gritar consignas ni sensacionalismo excesivo. No sientas un desastre, no te expreses negativamente y no exageres la ciencia ficción. Se centra en el amor, el apoyo, el contraataque y el crecimiento en la carrera de la juventud.
0 segundos a 5 segundos
La pista comienza al anochecer con carreras intensas y de alta velocidad. La cámara sigue la motocicleta del joven a gran velocidad hasta el suelo. Los neumáticos rozan el borde de la pista. La moto ruge, el viento sopla con fuerza y ​​el ambiente es tenso y fogoso. El joven estaba concentrado y el sol poniente dibujaba reflejos nítidos en la carrocería metálica del coche.
5 segundos a 9 segundos
Después de entrar en una esquina clave, el niño fue repentinamente superado por su oponente. El seguimiento a alta velocidad continuó y la imagen mostraba la sensación opresiva de que la clasificación descendía y el ritmo se interrumpía. En la vista de cerca del casco, se observa una pérdida temporal de concentración, dificultad para respirar y ligeros temblores. El niño susurró: "¿Aún puedo ponerme al día ..."
9 segundos a 14 segundos
El niño se quedó atrás, su respiración se volvió más pesada y su estado de ánimo llegó a un punto bajo. La carrera no se detuvo y la locomotora seguía avanzando a gran velocidad. La escena comenzó a recordar cálidos fragmentos de recuerdos mientras conducía a alta velocidad: cuando estaba aprendiendo a conducir cuando era niño, alguien lo apoyó por detrás; su padre le arregló el casco, sus movimientos eran meticulosos y silenciosos; antes de la meta, una suave sonrisa lo miró; y las figuras de atrás caminando una al lado de la otra por la pendiente al anochecer. Estos recuerdos se presentan con retroiluminación dorada, cámara suave y lenta y sentimientos fragmentados.
14 segundos a 18 segundos
La música gradualmente pasa de depresiva a edificante. Una voz contenida y suave surgió del recuerdo: "No tengas miedo, siempre estaré aquí". "Manténgase firme. Y mire hacia adelante". Los ojos del joven se volvieron a enfocar, su respiración se estabilizó lentamente y su estado de ánimo cambió de vacilante a firme.
18 segundos a 23 segundos
El joven recuperó la confianza, aceleró con todas sus fuerzas y contraatacó con precisión. Las tomas de seguimiento a alta velocidad muestran la potencia y el control de la motocicleta al tomar curvas, al salir de ellas y al acercarse al coche de delante. El niño dijo en voz baja pero firme: "No me detendré aquí".
23 segundos a 27 segundos
Más adelante apareció una pista ascendente y el niño corrió a toda velocidad contra el sol poniente. La imagen sólo conserva el sonido de la respiración, los sonidos del motor y la música que aumenta continuamente, sin añadir líneas innecesarias. La locomotora se elevó por los aires gracias a la inercia y entró en una velocidad sorprendentemente lenta. Una voz suave con una sonrisa vino desde lo más profundo de mi memoria: "Continúa".
27 segundos a 30 segundos
La cámara rodea la locomotora en el aire para obtener un primer plano panorámico en cámara lenta. Empuja las emociones de pasión, ternura, libertad y salto hacia el clímax. Las flores florecen detrás de ti, seguidas de un baile de semillas, consulta<<<image_1_1>>>
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

## Ampliar la presentación multilingüe

### Case 29: Expandir presentación multilingüe-expresión multilingüe-salida-1

[![Expandir presentación multilingüe-expresión multilingüe-salida-1](assets/thumbnails/29-multilingual-expression-29-group-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part3/group1/output.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part3/group1/output.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 11

**Prompt:**

```text
Vídeo en primera persona de un dron FPV de una sola toma, 33 segundos de toma larga continua, sin edición, sin saltos ni transiciones. La cámara comienza desde el interior de las nubes a gran altitud y forma una línea de vuelo descendente continua a lo largo de las nubes, la niebla, la luz y la sombra, los valles, las cascadas, los lagos, los campos de flores, los edificios urbanos y las plazas cercanas al suelo. 11 bloques de visualización de idiomas claros e independientes aparecen en secuencia durante todo el proceso. Cada bloque sólo muestra el texto correspondiente a un único idioma. No se pueden mezclar, superponer ni agregar otros idiomas.
0 a 3 segundos, las nubes<<<image_1_1>>>forman naturalmente "Hola" en chino;
3–6 segundos,<<<image_2_2>>>Niebla y luz volumétrica en inglés “Hello”;
6 a 9 segundos,<<<image_3_3>>>Proyección de luz solar y vapor de agua a gran altitud del "Hola" español (México);
9 a 12 segundos,<<<image_4_4>>>Cinta en el cielo formando la palabra indonesia “Halo”;
12 a 15 segundos, formación de cometas<<<image_5_5>>>formando “Hai” en malayo;
15 a 18 segundos,<<<image_6_6>>>La niebla matutina del valle forma el “สวัสดี” tailandés;
18–21 segundos<<<image_7_7>>>Cascada de niebla que forma árabe مرحبا
21-24 segundos,<<<image_8_8>>>El reflejo en el lago y las ondas forman la palabra portuguesa "Olá";
24–27 segundos,<<<image_9_9>>>Los campos de flores y prados están dispuestos de forma natural en el “Xin chào” vietnamita;
27 a 30 segundos,<<<image_10_10>>>Los edificios de cristal de la ciudad reflejan luces y sombras para formar la palabra japonesa "こんにちは";
30–33 segundos,<<<image_2_2>>>0 La niebla de agua de la fuente cercana, el pavimento del piso y las tiras de luz forman la palabra coreana "안녕하세요".
La atmósfera general es la de un amanecer temprano en la mañana, con luz de fondo dorada, luz volumétrica suave, nubes y niebla reales, desenfoque de movimiento natural y realismo a nivel de película. La velocidad de la cámara comienza lentamente entre 3 y 5 m/s, se acelera gradualmente hasta 14-16 m/s en todo el paisaje natural y luego se reduce hasta 2-3 m/s para flotar de manera estable en el cuadrado cercano a la Tierra. Parámetros de la lente: lente gran angular, 24 fps, movimiento suave del dron FPV, el tono cambia gradualmente de -5° a -18° y finalmente regresa a 0°; ligera guiñada ±10°, balanceo controlado de 0 a 10°, lo que garantiza una sensación de vuelo continua, estable y realista de un disparo a otro.
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

### Case 30: Expandir presentación multilingüe-expresión multilingüe-salida-2

[![Expandir presentación multilingüe-expresión multilingüe-salida-2](assets/thumbnails/30-multilingual-expression-30-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part3/group2/output.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part3/group2/output.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 9

**Prompt:**

```text
Estilo de acción en vivo, edición rápida, sensación cinematográfica, 4K, 24 fps, luz natural cálida, interpretaciones de personajes reales, sincronización de labios natural, sin subtítulos. Tomando la entrega de una flor como pista visual central de todo el vídeo, la flor se propaga rápidamente de un país a otro, conectando diferentes regiones y personas de todo el mundo. En cada escena, un personaje toma las flores, sonríe sinceramente y dice "gracias" en el idioma local. El ritmo general es enérgico y suave, y las tomas son dinámicas, enfatizando la atmósfera real de la vida callejera, las cálidas conexiones interculturales y la transmisión de buena voluntad entre las personas.
Método de transición: en la toma anterior, un personaje entregó la flor fuera de la pantalla y en la siguiente toma, otro personaje atrapó la flor en la nueva escena.
O utilice panorámicas rápidas, desenfoque de movimiento u oclusión de primer plano para completar transiciones fluidas
Mantenga la continuidad visual de las flores en la imagen para crear la sensación de "una toma extendiéndose por todo el mundo".
Estilo de lente: disparo de seguimiento manual, ligero movimiento de la lente, empujar y tirar rápido, combinación de primer plano y plano medio, atmósfera de sonido ambiental real y textura de toma callejera a nivel de película. La música de fondo es cálida, enérgica y tiene una sensación de viaje por el mundo, y el final se desvanece suavemente.
Escena 1<<<image_1_1>>>En una florería china, una escena de la vida real. La niña tomó una rosa, miró a la cámara, sonrió y dijo con naturalidad: "¡Gracias!". La cámara siguió las flores desde el lado derecho de la pantalla y la niña levantó suavemente el ramo después de recibir las flores.
Escena 2<<<image_2_2>>>Las calles de Inglaterra, clima ligeramente fresco, escena callejera natural. El hombre tomó un clavel, sonrió, asintió y dijo: "¡Gracias!". A través de la transición, la flor fue arrojada desde la escena anterior a esta escena.
Escena 3<<<image_3_3>>>Mercado mexicano, rico en color y lleno de fuegos artificiales. La tía tomó el ramo de caléndulas, juntó las manos y dijo cálidamente: "¡Gracias!" La cámara pasó rápidamente por encima del puesto y de la multitud, y el momento de recibir las flores quedó congelado.
Escena 4<<<image_4_4>>>Campo indonesio, brilla la luz del sol natural. El niño tomó una plumeria, sonrió alegremente, se inclinó levemente y dijo: "¡Terima kasih!" La cámara tenía la sensación de estar corriendo y la atmósfera era pura y natural.
Escena 5<<<image_5_5>>>Las calles de Tailandia están llenas de gente. El vendedor tomó un ramo de guirnaldas de jazmines, juntó las manos y dijo amablemente: "¡ขอบคุณค่ะ!" La cámara avanzó rápidamente y las guirnaldas se balancearon ligeramente a la luz del sol.
Escena 6<<<image_6_6>>>Patio árabe, luces y sombras suaves, ambiente elegante. La señora tomó una rosa del desierto, le acarició el pecho, sonrió y dijo: "¡شكراً!" La imagen era tranquila y cálida, y la expresión del personaje era sincera.
Escena 7<<<image_7_7>>>Comunidad brasileña, el ambiente es cálido y animado. El niño tomó una gerbera y se puso muy feliz y dijo: "¡Obrigado!" El plano es rítmico y lleno de vida.
Escena 8<<<image_8_8>>>En una calle japonesa, un oficinista tomó una pequeña flor de la lonchera, se inclinó cortésmente y dijo: "¡ありがとう!" La toma fue corta y clara, conservando la sensación de ritmo urbano.
Escena 9<<<image_9_9>>>Calles coreanas, ambiente urbano moderno. La joven tomó una rama de azalea, naturalmente cruzó las manos, sonrió y dijo: "¡감사합니다!" La cámara se detuvo por un momento mientras ella sonreía y luego la escena se desvaneció suavemente.
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

## Edición controlable más profunda

### Case 31: Edición controlada 1 salida

[![Edición controlada 1 salida](assets/thumbnails/31-controllable-editing-31-edited-output.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group1/output.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group1/output.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 2

**Prompt:**

```text
Mantén los personajes, el entorno de la jungla, el movimiento de la cámara, la composición, el ritmo de acción y la duración de<<<video_1_1>>>sin cambios.
Un arco de energía azul-blanco y una flecha luminosa<<<image_1_2>>>aparecen lentamente en la mano del personaje. El cuerpo del arco se forma gradualmente mediante la polimerización de arcos y partículas débiles, con una delicada textura de corriente que fluye, una ligera luz volumétrica y un contorno de energía estable. Durante el proceso de tensar el arco, la flecha se condensa en una flecha de energía de alto brillo en el centro de la cuerda del arco. En el momento en que el personaje se suelta, la flecha se dispara a gran velocidad, dejando una trayectoria de energía brillante, esbelta, continua y nítida.
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

### Case 32: Edición controlada 1 Referencia

[![Edición controlada 1 Referencia](assets/thumbnails/32-controllable-editing-32-reference.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group1/reference1.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group1/reference1.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 2

**Prompt:**

```text
Mantén los personajes, el entorno de la jungla, el movimiento de la cámara, la composición, el ritmo de acción y la duración de<<<video_1_1>>>sin cambios.
Un arco de energía azul-blanco y una flecha luminosa<<<image_1_2>>>aparecen lentamente en la mano del personaje. El cuerpo del arco se forma gradualmente mediante la polimerización de arcos y partículas débiles, con una delicada textura de corriente que fluye, una ligera luz volumétrica y un contorno de energía estable. Durante el proceso de tensar el arco, la flecha se condensa en una flecha de energía de alto brillo en el centro de la cuerda del arco. En el momento en que el personaje se suelta, la flecha se dispara a gran velocidad, dejando una trayectoria de energía brillante, esbelta, continua y nítida.
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

### Case 33: Salida de edición controlada 2

[![Salida de edición controlada 2](assets/thumbnails/33-controllable-editing-33-edited-output.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group2/output.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group2/output.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 1

**Prompt:**

```text
Elimine el dron en la pantalla<<<video_1_1>>>y el borde de la pista/carrocería en primer plano en la esquina inferior izquierda y, naturalmente, complete el área eliminada.
Mantenga el grupo de jirafas, las ramas de los árboles, los pastizales distantes, la luz de fondo dorada del atardecer, la perspectiva aérea y la composición de la toma completamente sin cambios. El fondo completo debe ser coherente con el entorno circundante, generando cielo natural, huecos entre ramas de árboles y detalles de césped sin manchas, parpadeos, deformaciones, imágenes fantasma o golpes. Asegúrese de que la sincronización de los fotogramas frontal y posterior del video sea consistente, que el movimiento sea continuo, que las transiciones de los bordes sean naturales y que la imagen general sea como la imagen real original.
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

### Case 34: Edición controlada 2 Referencia

[![Edición controlada 2 Referencia](assets/thumbnails/34-controllable-editing-34-reference.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group2/reference1.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group2/reference1.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 1

**Prompt:**

```text
Elimine el dron en la pantalla<<<video_1_1>>>y el borde de la pista/carrocería en primer plano en la esquina inferior izquierda y, naturalmente, complete el área eliminada.
Mantenga el grupo de jirafas, las ramas de los árboles, los pastizales distantes, la luz de fondo dorada del atardecer, la perspectiva aérea y la composición de la toma completamente sin cambios. El fondo completo debe ser coherente con el entorno circundante, generando cielo natural, huecos entre ramas de árboles y detalles de césped sin manchas, parpadeos, deformaciones, imágenes fantasma o golpes. Asegúrese de que la sincronización de los fotogramas frontal y posterior del video sea consistente, que el movimiento sea continuo, que las transiciones de los bordes sean naturales y que la imagen general sea como la imagen real original.
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

### Case 35: Salida de edición 3 controlada

[![Salida de edición 3 controlada](assets/thumbnails/35-controllable-editing-35-edited-output.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group3/output.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group3/output.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 4

**Prompt:**

```text
Se reemplazó la versión original del video de artes marciales para dos personas<<<video_1_1>>>con una prueba de viento con las manos vacías antes de un duelo con armas frías.
La escena se reemplaza con una plataforma de castillo de piedra medieval, un antiguo patio, una plataforma exterior de fortaleza de montaña o un simple campo de duelo de ladrillos de piedra. El fondo es la antigua muralla del castillo, el viento, la niebla, la línea montañosa distante y el suelo es plano y de piedra<<<image_1_2>>>.
La ropa del hombre con ropa oscura en el video se reemplaza por<<<image_2_3>>>, y la ropa del hombre con ropa clara en el video se reemplaza por<<<image_3_4>>>. La acción sigue siendo la misma, sin cambiar el ritmo original.
Los efectos especiales de la IA solo mejoran el entorno y la textura: ropa arrastrada por el viento, niebla ligera, una pequeña cantidad de polvo en los puntos de contacto, textura metálica reflectante en frío, partículas ligeras y una paleta de colores épica. El estilo general es sobrio, realista y una atmósfera clásica de duelo incondicional. Música de fondo atascada
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

### Case 36: Edición controlada 3 Referencia

[![Edición controlada 3 Referencia](assets/thumbnails/36-controllable-editing-36-reference.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group3/reference1.mp4)

[Reproducir video](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group3/reference1.mp4) · Haz clic en la miniatura para reproducir el video.

**Recursos de referencia:** 4

**Prompt:**

```text
Se reemplazó la versión original del video de artes marciales para dos personas<<<video_1_1>>>con una prueba de viento con las manos vacías antes de un duelo con armas frías.
La escena se reemplaza con una plataforma de castillo de piedra medieval, un antiguo patio, una plataforma exterior de fortaleza de montaña o un simple campo de duelo de ladrillos de piedra. El fondo es la antigua muralla del castillo, el viento, la niebla, la línea montañosa distante y el suelo es plano y de piedra<<<image_1_2>>>.
La ropa del hombre con ropa oscura en el video se reemplaza por<<<image_2_3>>>, y la ropa del hombre con ropa clara en el video se reemplaza por<<<image_3_4>>>. La acción sigue siendo la misma, sin cambiar el ritmo original.
Los efectos especiales de la IA solo mejoran el entorno y la textura: ropa arrastrada por el viento, niebla ligera, una pequeña cantidad de polvo en los puntos de contacto, textura metálica reflectante en frío, partículas ligeras y una paleta de colores épica. El estilo general es sobrio, realista y una atmósfera clásica de duelo incondicional. Música de fondo atascada
```

> [!NOTE]
> Este caso oficial también incluye recursos de referencia listados en el manifest.

---

## 📁 Estructura del repositorio

```text
.
├── README.md
├── README.<lang>.md
├── assets/
│   ├── banner.png
│   └── thumbnails/
├── data/
│   ├── seedance-2-5-manifest.json
│   └── seedance-2-5-prompt-translations.json
└── use-cases/
    ├── README.md
    ├── en/
    │   ├── README.md
    │   ├── 01-consistency.md
    │   └── official-seedance-2-5-guide.md
    └── <lang>/
        ├── README.md
        └── official-seedance-2-5-guide.md
```

## 🙏 Reconocimiento

EvoLink mantiene este repositorio como guía pública para Seedance 2.5 early access.

- Official early access: [Get Seedance 2.5 Early Access](https://evolink.ai/seedream-5-0?utm_source=github&utm_medium=readme&utm_campaign=awesome-seedance-2.5-guide)
- Current API key path: [EvoLink signup](https://evolink.ai/signup?utm_source=github&utm_medium=readme&utm_campaign=awesome-seedance-2.5-guide)
- Current API examples: [Seedance 2.5 Gateway Service](https://github.com/EvoLinkAI/Seedance-2.5-Gateway-Service)
