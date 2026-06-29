<div align="center">

<a href="https://evolink.ai/launch/seedance-2-5?utm_source=github&utm_medium=banner&utm_campaign=awesome-seedance-2.5-guide"><img src="assets/banner.png" alt="Seedance 2.5 Early Access guide" width="100%"></a>

# Guide officiel Seedance 2.5

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](LICENSE)
[![Get Seedance 2.5 Early Access](https://img.shields.io/badge/Get_Seedance_2.5-Early_Access-black)](https://evolink.ai/launch/seedance-2-5?utm_source=github&utm_medium=badge&utm_campaign=awesome-seedance-2.5-guide)
[![Official Guide](https://img.shields.io/badge/Official_Guide-36_Media_Assets-7C3AED)](data/seedance-2-5-manifest.json)
[![API Key](https://img.shields.io/badge/API_Key-EvoLink-orange)](https://evolink.ai/signup?utm_source=github&utm_medium=badge&utm_campaign=awesome-seedance-2.5-guide)

[English](README.md) · [Español](README.es.md) · [Português](README.pt.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Deutsch](README.de.md) · **Français** · [Türkçe](README.tr.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Русский](README.ru.md)

</div>

## 🍌 Introduction

Seedance 2.5 early access est ouvert via EvoLink. Ce dépôt transforme les matériaux officiels de lancement en guide natif GitHub pour créateurs, développeurs et équipes vidéo IA.

Le guide couvre 36 médias officiels: demos, showcases, contrôle narratif, expression multilingue et édition contrôlable. Comme ce sont des cas officiels, nous n’ajoutons pas d’auteur ni de source par case.

[Get Seedance 2.5 Early Access](https://evolink.ai/launch/seedance-2-5?utm_source=github&utm_medium=readme&utm_campaign=awesome-seedance-2.5-guide) · [Obtenir une clé API](https://evolink.ai/signup?utm_source=github&utm_medium=readme&utm_campaign=awesome-seedance-2.5-guide) · [Exemples API Seedance actuels](https://github.com/EvoLinkAI/Seedance-2.5-Gateway-Service)

> [!NOTE]
> Les snippets API exécutables utilisent encore le chemin stable de Seedance 2 pendant le rollout de Seedance 2.5 early access. Ne remplacez pas les model IDs vérifiés `seedance-2.0-*` par des IDs 2.5 non vérifiés.

## 📑 Menu

- Introduction
- Démarrage rapide
- Guide Seedance 2 original
- Guide officiel Seedance 2.5
- Structure du dépôt
- Remerciements

## 🚀 Démarrage rapide

Utilisez ce dépôt pour inspecter les exemples officiels 2.5, copier des structures de prompt et rejoindre le rollout 2.5.

> [!NOTE]
> Ce démarrage rapide conserve volontairement le model ID vérifié `seedance-2.0-text-to-video` et le chemin API Seedance 2 actuel. Seedance 2.5 API access arrive via early access; ne remplacez pas cet ID 2.0 exécutable par un ID 2.5 non vérifié.

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

## 🧭 Guide Seedance 2 original

Le nouveau guide officiel Seedance 2.5 est placé en premier. Le guide Seedance 2 d'origine complet reste conservé comme cible legacy pour le chemin API actuel, les patterns de cas d'usage, les modèles de prompt, les notes de paramètres et le workflow multimodal.

- [Ouvrir le guide original complet Seedance 2](seedance-2-guide/README.fr.md)
- [Ouvrir l’index original des 55 cas](use-cases/README.md)
- [Use cases Seedance 2 en anglais](use-cases/en/README.md)
- [Use cases Seedance 2 en chinois simplifié](use-cases/zh-CN/README.md)
- [Use cases Seedance 2 en chinois traditionnel](use-cases/zh-TW/README.md)
- [Exemples API Seedance actuels](https://github.com/EvoLinkAI/Seedance-2.5-Gateway-Service)

## 🎬 Guide officiel Seedance 2.5

## Vidéo au-dessus de la ligne de flottaison

### Case 1: Vidéo au-dessus de la ligne de flottaison 1

[![Vidéo au-dessus de la ligne de flottaison 1](assets/thumbnails/01-hero-demo-1-official-launch-film-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/firstScreen/group2/2.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/firstScreen/group2/2.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Prompt:**

```text
Une séquence graphique animée 3D cinématographique haut de gamme de 30 secondes, utilisant des styles de paysages miniatures steampunk et rétro exquis, avec des mouvements de caméra environnants et pénétrants continus et fluides.
[0-10 secondes] : gros plan macro d'un cadran d'horloge en laiton antique, se déployant miraculeusement en anneaux d'engrenages rotatifs entrelacés et en brouillard volumétrique. La caméra pénètre vers le bas à travers les engrenages et un ornithoptère mécanique plane dans le ciel depuis un canyon miniature fait de piles de vieux livres anciens.
[10-20 secondes] : La caméra suit la trajectoire de l'ornithoptère alors qu'il glisse vers l'avant, pénétrant de manière transparente dans une boîte fantôme en laiton ornée de rotation à grande vitesse (Zoetrope), qui projette la lumière et l'ombre dynamiques d'un cheval mécanique au galop. La lumière et l'ombre sont sorties de la boîte et la scène s'est instantanément transformée en un téléphérique suspendu à la texture de laiton, qui voyageait à travers la forêt d'engrenages mécaniques le long des rails de cuivre scintillants, baigné dans une lumière dorée digne d'un film.
[20-30 secondes] : La caméra effectue un panoramique gracieux vers le bas et un magnifique voilier mécanique en bois apparaît sous le téléphérique, traversant les vagues ondulantes en verre bleu foncé. La fin des vagues s'est progressivement transformée en une lune géante et brillante, et les silhouettes d'un groupe d'explorateurs tenant des lanternes oscillantes marchaient le long de la crête de la mine de cristal sous les étoiles. La caméra effectue un zoom arrière en spirale douce, à travers des nuages ​​éthérés, et revient au grand cadran de l'horloge en laiton.
Spécifications techniques : textures mécaniques hyperréalistes, riches tons de laiton et d'or et faible profondeur de champ cinématographique. Mouvement de navette fluide et cohérent, un fort sentiment d'atmosphère d'aventure épique et fantastique.
```

---

### Case 2: Vidéo au-dessus de la ligne de flottaison 2

[![Vidéo au-dessus de la ligne de flottaison 2](assets/thumbnails/02-hero-demo-2-official-launch-film-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/firstScreen/group1/1.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/firstScreen/group1/1.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Prompt:**

```text
Un court métrage de transition cinématographique rapide et fluide (match-cut) avec des rythmes électroniques dynamiques. Une boule de cristal impeccable est toujours fixée au centre du tableau, avec le logo lumineux « seedance » gravé à l’intérieur. La boule de cristal maintient une concentration extrême et, avec le puissant rythme du tambour musical, l'arrière-plan change de manière transparente à grande vitesse :
Scène 1 : Macro gros plan, de l'eau semblable à un film éclaboussant autour de la boule de cristal, réfractant la lumière et l'ombre complexes.
Scène 2 : Un café rétro le matin. La boule de cristal est posée sur la table en bois. L’arrière-plan est la vapeur montante du café et le flux flou des navetteurs devant la fenêtre.
Scène 3 : A l'heure dorée de la soirée, un jeune skateur lance une boule de cristal d'une main. L’arrière-plan est la scène de rue en régression rapide et le magnifique contre-jour du coucher de soleil.
Scène 4 : Au Frenzy Music Festival, les gens brandissent des boules de cristal, reflétant le laser de la scène sur un magnifique arrière-plan.
Scène 5 : Une table de fête familiale animée, avec une boule de cristal au centre et des personnages flous en arrière-plan célébrant un toast et prenant de la nourriture.
Scène 6 : Dans un cinéma sombre, les deux mains tiennent une boule de cristal, et la faible lumière de l'immense écran coule à sa surface.
Scène 7 : La boule de cristal est placée sur le diaphragme sonore fortement vibrant et passe de manière transparente au centre du lecteur DJ rotatif avec le point culminant de la musique.
Scène 8 : Nuit de camping en plein air, l'arrière-plan se transforme en un feu de joie chaleureux et des points lumineux oscillants (Bokeh).
Lancer et terminer : Avec l'accent final de la musique, la boule de cristal a été lancée bien au-dessus de l'écran ; il est instantanément passé à un fond noir pur, et le mot blanc minimaliste « seedance » sur fond noir est apparu au centre de l'écran.
Suivez de près le montage dynamique du rythme BGM (transition bloquée), l'étalonnage des couleurs cinématographique de premier ordre (Cinematic Color Grading). Matériaux de réfraction et de transmission du verre réalistes, traçage de rayons complexe et éclairage global. Le sujet est extrêmement clair, l'arrière-plan présente un fort flou dynamique et l'impact visuel est extrêmement fort.
```

---

### Case 3: Vidéo au-dessus de la ligne de flottaison 3

[![Vidéo au-dessus de la ligne de flottaison 3](assets/thumbnails/03-hero-demo-3-official-launch-film-3.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/firstScreen/group3/output.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/firstScreen/group3/output.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 5

**Prompt:**

```text
Court métrage de concept de marque cinématographique.<<<image_1_1>>>est la première image, l'écran tremble légèrement, la caméra zoome progressivement et arrive à l'ombre de l'arbre qui s'éloigne rapidement à l'extérieur de la fenêtre. L'ombre de l'arbre recule de plus en plus vite et passe soudainement à<<<image_2_2>>>, la vitesse ralentit soudainement, la caméra se déplace lentement le long du ruisseau, les oiseaux chantent et les fleurs sont parfumées.
La caméra descendit vers l'eau. L'effet sonore comprenait le bruit des bulles dans l'eau. Un groupe de méduses orange nageait gracieusement devant la caméra. JETONPLACEHOLDER2. La caméra recula lentement. Un groupe de petits poissons est passé devant la caméra et a traversé l’eau jusqu’à la fenêtre. JETONPLACEHOLDER3. La jeune fille regarda à gauche et à droite, observant le petit poisson.
La caméra recule lentement et l'image est floue, puis se recentre et l'image devient claire, passant au rythme de la musique : fenêtre de jardin chinois<<<image_5_5>>>cercles lumineux, vitraux d'église, hublots d'avion, lucarnes en forme de dôme, baies vitrées, stores, lucarnes européennes, yeux de chat sur les portes, viseurs de caméra, yeux d'oiseaux et gros plans d'yeux humains.
L'écran reste sur un gros plan d'yeux humains, puis les yeux sont fermés et l'écran devient noir. Puis soudain les yeux s'ouvrent, et le mot « seedance » avec un accent apparaît au centre des yeux.
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

## L'utilisateur travaille

### Case 4: effets visuels 1

[![effets visuels 1](assets/thumbnails/04-official-showcase-4-visual-effects.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/16-9/169-1.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/16-9/169-1.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Prompt:**

```text
Une vidéo d'animation de texte créatif en boucle transparente de 15 secondes, 4K, 30 ips. Chaque langue prend environ 1,2 seconde et la transition s'effectue par dissolution du texte, déformation ou diffusion de particules, sans coupures brutales. La musique de fond a un rythme évident et un fort décalage
0-1,2s "Création" chinoise·Op illusion d'optique fond noir pur, cercles concentriques noirs et blancs s'étalant à partir du centre pour former un tunnel visuel. Le caractère chinois tridimensionnel blanc « Création » dépasse lentement du centre du cercle vers la caméra. Il est audacieux et sans empattement avec des ombres subtiles sur les bords. Les cercles concentriques créent des ondulations et des distorsions à mesure que le texte avance, comme des ondulations sur l’eau. Le texte s'est arrêté après avoir complètement dépassé, puis s'est dissous en particules de crayon bleu et s'est envolé.
1,2-2,4 s Anglais "CREATE" · Crayon peint à la main, fond de texture de papier kraft jaune chaud, traits de crayon bleu rugueux écrivent les majuscules anglais "CREATE" un par un. Les coups de pinceau présentent un grain pastel évident et des marques qui se chevauchent, et la dernière ligne horizontale du E est légèrement surélevée. Après l'écriture, la surface des lettres présente un léger éclat cireux et de légères lignes auxiliaires au crayon apparaissent sur l'arrière-plan. Le texte est ensuite aspiré dans les lignes de balayage CRT et disparaît.
2,4-3,6 s "CREAR" espagnol · Cadre d'arcade sombre rétro, l'écran CRT central présente des lignes de balayage subtiles et un grain de poudre de phosphore. Le mot pixel tridimensionnel « CREAR » avec un dégradé bleu et violet s'élève du bas. La surface des lettres présente une animation d'ondulation blanche comme les vagues de l'océan, et le bord émet une lumière bleu néon. Il y a « CREDIT 00 » dans le coin supérieur gauche de l'écran et « INSERT COIN » clignote dans le coin inférieur droit. Le texte s’est ensuite pixellisé et désintégré en un motif batik indigo.
3,6-4,8s "CIPTAKAN" indonésien · Tissu Batik. Fond en tissu batik indonésien traditionnel bleu indigo foncé, avec de fins motifs paraboliques sur la surface du tissu. La police à empattement blanche « CIPTAKAN » s'élève lentement du bas du tissu, comme un marquage à chaud, et le tissu crée de véritables rides et fluctuations à mesure que le texte émerge. Après que les mots soient apparus, le tissu a été soufflé par le vent et les débris dorés ont volé, se transformant en motifs géométriques islamiques.
4,8-6,0 s malais "CIPTA"·Géométrie islamique. Fond en velours vert foncé, motifs géométriques arabesques dorés s'étalant des quatre coins jusqu'au centre. Le mot empattement classique blanc « CIPTA » tourne et émerge du centre. Les lettres sont entourées de motifs d'étoiles et des particules de poudre d'or tombent. Les mots ont ensuite été gravés textuellement sur la plaque de métal noir avec un couteau à graver en or.
6,0-7,2s Thai "สร้างสรรค์" · Gravure sur feuille d'or sur fond noir, Thai "สร้างสรรค์" est présenté en or, comme s'il était sculpté dans une ancienne plaque de temple. Il y a une subtile animation de feuille d'or qui se décolle de la surface du texte, révélant l'apprêt rouge foncé en dessous, avec des éclats dorés volant autour. Une fois la gravure terminée, les mots fondent en gouttes de mercure argenté et s'égouttent.
7,2-8,4 s Arabe "إبداع" · Tournage mécanique des pages. L'affichage tournant les pages en métal noir occupe tout l'écran et les lames mécaniques cliquent et tournent à leur tour. Le texte arabe « إبداع » composé de grilles de pixels blancs apparaît une à une de droite à gauche, et chaque retournement de lettre est accompagné d'un mouvement mécanique précis et d'une légère vibration. Une fois la page tournée, le texte est emporté par une tempête de plumes de samba colorées.
8,4-9,6 s "CRIAR" portugais · Plumes de carnaval. Sur un fond noir, des plumes de samba colorées convergent du bord de l’image vers le centre pour former un immense éventail de plumes. Les lettres blanches en gras « CRIAR » ont jailli du centre de l'éventail de plumes, et les plumes ont volé sous l'impact des mots. La surface des mots était reflétée par les paillettes du Carnaval et les points verts, jaunes et bleus du drapeau brésilien brillaient. Le texte a ensuite été lavé à l’encre noire.
9,6-10,8s "SÁNG TẠO" vietnamien · Soie à l'encre. Sur un fond de soie blanc cassé, de l'encre noire coule lentement du haut de l'image, formant progressivement le mot vietnamien « SÁNG TẠO ». L'encre crée un bord taché naturel sur la soie et certaines gouttelettes d'encre s'égouttent pour former des perles d'encre suspendues. Une fois terminée, la soie a été soufflée par le vent, révélant le motif sombre du lotus en dessous, et le texte s'est condensé en une boule de verre transparente.
10.8-12.0s "Création" en japonais · Verre optique Une boule de verre optique transparente parfaite est suspendue au centre d'un fond noir pur. La balle reflète un astigmatisme de couleur arc-en-ciel. Derrière la boule de verre, le caractère chinois japonais « Création » est présenté dans une projection de dispersion arc-en-ciel. Lorsque la boule de verre tourne lentement, le texte produit une distorsion optique qui se tord, s'étire et se sépare. De fines particules de poussière se trouvent à la surface de la sphère de verre, qui fondent ensuite en un métal liquide argenté.
12,0-13,2s Coréen 「창조」 · Métal liquide. Sur fond de ciel étoilé profond, du mercure liquide argenté s'égoutte du haut de l'image et se condense naturellement dans l'air pour former le mot coréen « 창조 ». La surface des caractères liquides présente une forte réflexion spéculaire, reflétant les étoiles environnantes. Une fois les mots formés, une partie du mercure liquide a continué à couler vers le bas, formant des perles métalliques suspendues. Finalement, tout le liquide métallique s’est rassemblé en une énorme sphère d’argent.
```

---

### Case 5: Film 2

[![Film 2](assets/thumbnails/05-official-showcase-5-cinematic-film.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/3-4/34-1.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/3-4/34-1.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Prompt:**

```text
【Réglage du style général】
Un blockbuster visuel haut de gamme de 30 secondes au niveau de la marque avec une forte sensation cinématographique et une texture haut de gamme. L’image met l’accent sur des points lumineux de rêve (Bokeh), des transitions de flou de mouvement soyeuses (Flou de mouvement), un éclairage volumétrique et une expression ultra-réaliste des détails des matériaux.
[Description du scénario]
[0-5 secondes] : Prologue de rêve et gros plan macro
Gros plans macro de très haute qualité. Une main fine s’étendait dans les airs et ses doigts touchaient des points colorés aussi brillants et scintillants que des étoiles. Avec le flux de lumière et d'ombre, la scène passe de manière fluide et fluide à une femme élégante vêtue d'une jupe en tulle blanc pur, qui joue d'un piano vintage en état d'ébriété. Faible profondeur de champ, l’arrière-plan devient flou dans un magnifique ton bleu-vert.
[5-15 secondes] : Puis passage à un plan de suivi fluide : une femme portant un chapeau de paille français à larges bords et une jupe blanche fluide, courant légèrement dans le chemin de fleurs dense rempli de roses rose-orange et d'hortensias bleus. La lumière projette une lumière et des ombres tachetées à travers les feuilles, montrant parfaitement la douce brise, la physique réaliste du tissu de la jupe flottant et la texture ultra-réaliste des pétales.
[15-24 secondes] : esthétique silencieuse et réfraction de la lumière et des ombres
Le rythme de la caméra ralentit et entre dans le magnifique ralenti ultime (Slow-motion). Une fille est assise à une table en fer forgé noir à côté d'une fontaine dorée rétro européenne et lit tranquillement. Il y a des bulles de savon cristallines flottant dans l'air, et la surface des bulles reflète parfaitement les fleurs environnantes et la chaleur du soleil. Le moment où les gouttelettes d'eau éclaboussent est clairement visible, démontrant les capacités de rendu de haut niveau du modèle pour les matériaux transparents, la réfraction de l'eau et l'éclairage complexe.
```

---

### Case 6: Effets de post-production 3

[![Effets de post-production 3](assets/thumbnails/06-official-showcase-6-post-production-vfx.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/1-1/11-1.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/1-1/11-1.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Prompt:**

```text
Une scène de récif corallien en eaux profondes, un monde sous-marin tropical dominé par le bleu, avec une vaste zone de coraux vivants colorés, sains et prospères, y compris des coraux branches, des coraux cérébraux, des coraux disques et des coraux mous, avec un grand nombre de poissons tropicaux faisant naturellement la navette entre eux. La vue rapprochée est claire et vive, tandis que la vue lointaine devient progressivement plus bleue et plus grise et le contraste s'affaiblit. La lumière naturelle au-dessus est filtrée par l’eau de mer pour former une douce lumière volumétrique. Il y a de petites particules en suspension et une légère sensation d’écoulement dans l’eau de mer. 8 à 12 de différentes tailles. Le corps en forme de parapluie a un doux effet de bioluminescence, les tentacules flottent doucement avec les vagues et il y a de faibles taches lumineuses violettes aux extrémités des tentacules. La taille des méduses est proportionnelle aux coraux et aux poissons, et l'effet lumineux est doux et non éblouissant, formant des points de lumière oniriques sur le fond sombre de l'eau de mer. Le mouvement de l'essaim de méduses est naturel, dans une spirale qui s'élève lentement, et certaines méduses nagent devant l'objectif, créant un léger effet de lumière parasite. En conservant l'éclairage bleu sous l'eau, la lueur des méduses coexiste harmonieusement avec les faibles reflets des coraux environnants. Pendant le processus de nage du groupe de méduses, des bulles ont été générées et les bulles ont flotté, formant le mot « Seedance » dans la mer.
```

---

### Case 7: Film 4

[![Film 4](assets/thumbnails/07-official-showcase-7-cinematic-film.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/1-1/11-2.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/1-1/11-2.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Prompt:**

```text
Texture cinématographique, sens haut de gamme, désert doré le matin, bâtiment minimaliste d'un musée d'art blanc flottant au-dessus des dunes de sable, avec de fines textures de pierre et de doux reflets sur la surface du bâtiment. La lumière du soleil traverse le sable et la poussière pour former une lumière volumétrique, et les dunes au loin sont clairement superposées. La caméra part d'un panorama désertique ultra grand angle, avance lentement, traverse le sable volant et pénètre à l'intérieur du bâtiment flottant. L'intérieur présente des sculptures suspendues, des installations en soie translucide et un personnage vêtu d'une robe blanche, dont le tissu se balance naturellement au vent. La caméra se déplace en douceur autour des personnages et finalement les murs du bâtiment s'ouvrent lentement pour révéler une vaste étendue de ciel et de désert. Style publicitaire artistique haut de gamme, éclairage réel, matériaux exquis, composition de niveau film, mouvement élégant, surréaliste mais authentique.
```

---

### Case 8: Publicité 5

[![Publicité 5](assets/thumbnails/08-official-showcase-8-advertising.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/16-9/169-2.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/16-9/169-2.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Prompt:**

```text
Un court métrage de 30 secondes sur un concept de marque de haut niveau avec une grande tension visuelle. L’ouverture adopte une perspective inversée surréaliste. La caméra se retourne avec gravité, montrant les pieds du mannequin portant des bottes en daim rétro marchant légèrement sur les dunes de sable rouge ondulantes. L'objectif macro ferme la texture de velours givré de la surface des bottes et les particules de sable rouge rugueuses qui y sont tachées. Ensuite, on passe à une série de montages pleins d'apesanteur et de couleurs oniriques : de jeunes modèles masculins et féminins tombent légèrement en arrière au milieu du vent et du sable ambrés déferlants et de la lumière froide du bord ; la caméra passe rapidement à un gros plan très net du visage - le vent et le sable soufflent à travers les cils tachés de minuscules sables dorés, et le modèle porte des lunettes de soleil à monture métallique rétro, le soleil brûlant et la tempête de la nature se reflètent clairement dans les lentilles incurvées. Puis, les doigts portant de vieilles et épaisses bagues en argent effleurèrent doucement les parois rocheuses rugueuses et les roseaux dansant au vent.
Les images utilisent largement le langage de l'objectif très expressif : grâce à un objectif macro à très faible angle, à travers les cristaux minéraux naturels flous et clairs, le ciel étoilé profond et vaste et les explorateurs voyageant sans raison sont capturés d'en haut. La grande scène est densément entrecoupée de gros plans de haute qualité : la texture de la chemise en lin flammé bruissant au vent, la mâchoire serrée et froide du mannequin et l'éclat de la sueur sur la peau du cou qui brille sous le contre-jour. Combinant des objectifs fisheye, des mouvements de caméra à rotation rapide et des transitions de dislocation visuelle soyeuses, il crée une dynamique mystérieuse, avant-gardiste et pleine de tension sauvage.
Au point culminant du court métrage, la caméra effectue un zoom arrière spectaculaire, brisant le « quatrième mur », révélant qu'il s'agit en fait d'un studio virtuel avancé avec un auvent circulaire géant à piste d'étoiles LED et un véritable réseau de sable rouge, en collision parfaite avec l'immensité de la nature sauvage et le sentiment d'un studio industriel pionnier. A la fin, le rythme ralentit et revient à un gros plan de textures délicates : une femme aux cheveux ébouriffés s'appuie contre un tout-terrain rétro. La caméra balaie lentement la peinture métallique marbrée et écaillée du véhicule. La femme laisse nonchalamment le sable fin dans sa paume glisser de ses doigts. La lumière latérale froide et lumineuse au clair de lune décrit avec précision les pores du tissu rugueux de la veste en cuir vieilli, la lumière froide réfléchie par la fermeture éclair en métal lourd et le contour froid du visage tridimensionnel de la femme. La conception globale présente une esthétique de couleur rétro au niveau d’un film, avec un bleu nuit profond entrelacé d’orange minéral ardent. L'image est atmosphérique, libre et pleine de tension de marque de haute qualité. Enfin, le texte « seedance » apparaît gracieusement au centre de l’image.
```

---

### Case 9: Film 6

[![Film 6](assets/thumbnails/09-official-showcase-9-cinematic-film.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/3-4/34-2.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/3-4/34-2.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Prompt:**

```text
Court métrage sur le patrimoine culturel immatériel de l'Opéra de Pékin, avec une ambiance cinématographique, une esthétique orientale, de la chaleur et de la retenue. Dans les coulisses des troupes de théâtre traditionnel et des ateliers d'artisanat, des maîtres artisans fabriquent tranquillement des coiffes d'opéra de Pékin, arrangent les costumes et dessinent le maquillage du visage. Les détails de leurs mains sont délicats et les fils de soie, les perles, les peintures et les motifs de broderie sont tous de haute qualité. Un jeune apprenti observait attentivement, puis prenait soigneusement les outils et accomplissait les petites étapes sous la direction du maître. Le vieux maître redressa la tête et redressa ses vêtements, comme s'il remettait doucement un métier et une émotion entre ses mains. Finalement, le jeune homme était bien habillé et se tenait à côté de la scène où il s'apprêtait à monter sur scène. La faible lumière illuminait son costume et son profil, et le vieux maître regardait tranquillement derrière lui. L'atmosphère générale est calme, affectueuse et a un sentiment d'héritage, avec peu de sous-titres et de lignes appropriées intercalées.
```

---

### Case 10: Jeu 7

[![Jeu 7](assets/thumbnails/10-official-showcase-10-game-trailer.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/16-9/169-3.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/16-9/169-3.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Prompt:**

```text
"Civilisation océanique"
(Science-fiction épique / Dune × Interstellaire / Aucune personne réelle / Forme de vie sculptée)
[0 à 5 secondes | Ouverture cosmique·L'océan comme mémoire planétaire]
L'océan d'un bleu profond occupe toute la scène et les plans d'eau extrêmement profonds présentent une structure en couches, tout comme l'univers liquide à l'intérieur de la planète.
La caméra descend lentement verticalement d'une haute altitude, traverse les nuages ​​et le brouillard marin et entre dans la mer.
La surface de la mer fluctue comme un film métallique, réfractant les fissures irrégulières des rayons du soleil, créant une lumière volumétrique épique.
[5 à 10 secondes | Entrer dans la faille de la civilisation des grands fonds]
La lentille pénètre la surface de la mer et pénètre dans les profondeurs marines.
L'immense « structure de civilisation sous-marine » a progressivement émergé :
Mégastructures fracturées en forme d'anneau, dômes de pierre engloutis et plates-formes de ruines géométriques flottantes.
Le style structurel combine des temples anciens + le sens de la technologie de la civilisation extraterrestre (similaire au langage des ruines de Dune).
Il y a des particules scintillantes en suspension dans l’eau, comme de la poussière d’étoiles qui dérive lentement dans l’eau.
[10 à 15 secondes | Une forme de vie sculptée apparaît (non humaine)]
Au centre du théâtre se dresse une sculpture géante représentant une forme de vie :
Une "statue humanoïde" faite de pierre blanche et de minéraux translucides, mais sans détails de vie (pas de peau, pas de véritables traits humains).
Sa posture ressemble à une ancienne structure rituelle et son corps a une structure géométrique segmentée, semblable au porteur de mémoire de la civilisation.
La surface de la sculpture a été érodée par l'eau pendant longtemps et est recouverte de structures cristallines d'algues et de coraux.
La caméra fait lentement le tour de la sculpture, créant une « impression de l'arrivée des dieux ».
[15–20 secondes｜La civilisation est réveillée·Flux optique activé]
Les ruines sous-marines entières ont commencé à « se réveiller ».
De faibles motifs lumineux circulant d’énergie apparaissent à l’intérieur de la sculpture, s’éclairant comme un réseau neuronal.
Les piliers de pierre brisés s'élèvent lentement et se réorganisent pour former une structure de théâtre annulaire.
Le plan d'eau a commencé à montrer un « écoulement ordonné », comme si l'espace était en train d'être recalculé.
La caméra est entourée d'une rotation statique → légèrement accélérée.
[20 à 24 secondes | Inversion de la surface de la mer · percée croissante]
La caméra accélère soudainement vers le haut et sort de la mer.
L’eau de mer s’est séparée des deux côtés, formant un rideau d’eau géant.
La coque d'un vaisseau spatial/temple géant d'une ancienne civilisation s'élève du fond de la mer :
Il ressemble à un croisement entre un temple de pierre et un navire de science-fiction, avec sa surface recouverte de coraux et de structures minéralisées.
La coque du navire s'élève comme une cascade avec l'eau de mer.
[24-27 secondes | Plan rotatif épique (climax visuel)]
La caméra tourne autour du vaisseau géant à grande vitesse (prise de vue en orbite spirale).
Le soleil pénètre à travers les fissures des nuages, formant un pilier de lumière sacré.
Le flux d’eau tourne et prend la forme d’une spirale, comme une structure galactique.
La coque se retourne lentement, révélant sa structure massive :
Semblable aux « reliques de civilisation mobiles » plutôt qu'au transport.
【27–30 secondes｜Vision ultime · Révéler l'échelle de la civilisation】
La caméra effectue un zoom arrière très rapidement dans une perspective au niveau de l'espace.
L'océan, les ruines, les navires géants qui s'élèvent et les temples sculptés sont disposés verticalement sur le même écran :
Formant la structure cosmique en trois sections de la « couche de lumière civilisation sous-marine-surface de la mer-ciel ».
Le monde entier est comme un système de mémoire éveillé d’une ancienne planète.
À la fin, l’image s’est lentement estompée pour devenir un écran noir, ne laissant que de faibles points lumineux.
Esthétique épique de science-fiction / Structure de la civilisation des dunes, du vent et de la mer de sable / Échelle spatiale au niveau interstellaire / Récit sans caractère / Ruines de la civilisation sculptée / Structure du temple extraterrestre / Lumière volumétrique pénétrant l'eau de mer / Effondrement et réorganisation de bâtiments géants / Plans rituels sacrés / Mouvement du miroir en spirale / Océan de particules de poussière d'étoile / Réalité au niveau du film à plage dynamique élevée
```

---

### Case 11: Cinéma et télévision 8

[![Cinéma et télévision 8](assets/thumbnails/11-official-showcase-11-cinematic-film.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/1-1/11-3.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/1-1/11-3.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Prompt:**

```text
Le thème est « Fleur mécanique en fleurs ». L'image doit mettre en évidence les avantages du modèle vidéo généré en termes de lumière et d'ombre, de détails artistiques, de réalisme, de mouvement de caméra et de sensation cinématographique des personnages. Le style général est celui d’une publicité de marque technologique haut de gamme avec un fort impact visuel. La vidéo utilise une prise de vue macro unique, commençant par les boutons floraux métalliques dans l'obscurité, entrant progressivement dans la structure mécanique précise à l'intérieur des pétales, et se terminant enfin par la fleur mécanique pleinement épanouie et la lumière se propageant vers l'extérieur comme point culminant. Nécessite un véritable éclairage physique, des matériaux métalliques et en verre exquis, un mouvement mécanique délicat, une composition stable, un étalonnage des couleurs au niveau du film et aucun sous-titre.
```

---

### Case 12: Science populaire 9

[![Science populaire 9](assets/thumbnails/12-official-showcase-12-educational-film.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/3-4/34-3.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/ugc/3-4/34-3.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Prompt:**

```text
Exigences générales de style : animation de plan de couleur rocheuse, esthétique décorative orientale et de la Route de la Soie, texture de pigment minéral, rouge cinabre, ocre, vert pierre, outremer, embellissements dorés, textures de papier et murales, superposition plane, pas de vraie photographie, pas de réalisme 3D. Le rythme de l'image passe de l'immobilité au mouvement, puis du mouvement retour à l'immobilité, soulignant le sentiment de voyage et la richesse de « de la terre à la tasse ». La musique est joyeuse et de style occidental.
Plan 1 : Les branches commencent à apparaître, et la richesse commence (0-4 secondes)
Des blocs d'ocre et de vermillon fleurissent sur le papier du tableau de la Route de la Soie, et une branche de grenade s'étend du côté droit du tableau. Les feuilles sont épaisses et présentent des couches évidentes de pigments minéraux. Une grenade dodue apparut lentement sur la branche. Sa coquille était rouge avec de l'or et son contour était rond et calme. La lumière du soleil tombe sur la peau avec des taches rondes dorées et des points dorés. La surface de la grenade a un éclat chaleureux, comme un fruit mûri avec le temps. Le tempérament d'ouverture est riche mais sobre.
Shot 2 : Enlevez-le délicatement et le voyage commence (4-7 secondes)
La grenade a été délicatement cueillie par une servante des régions occidentales avec des mouvements doux et élégants. Des motifs d'herbes frisées, des motifs anciens et de longues compositions décoratives en volutes émergent progressivement en arrière-plan, suggérant qu'ils proviennent d'un pays lointain. L’image passe naturellement des branches statiques au déroulement du voyage. Les montagnes, les routes et les villes commencent à s'étendre à l'arrière-plan, comme une longue route de la soie qui se déroule lentement.
Plan 3 : Traverser des routes anciennes et traverser des montagnes et des rivières (7-13 secondes)
Les silhouettes de l'attelage de chameaux avancent lentement, les cloches représentent le rythme avec de minuscules points dorés et des grenades apparaissent dans le sac à dos du chameau. L'ancienne route traverse des dunes de sable, des oasis et des portes de la ville. Le vent et le sable passent selon des schémas fluides, et la route délimitée par la ligne dorée continue de s'étendre au loin. Les couleurs sont fortes et haut de gamme, comme une fusion de peintures murales de la Route de la Soie et d'illustrations aux couleurs rock. La grenade a toujours été brillante et pleine pendant le long voyage, comme si elle avait conservé jusqu'à ce jour le soleil, la chaleur et la richesse d'une terre lointaine.
Plan 4 : Transition entre les temps anciens et modernes, arrivée au moment présent (13-16 secondes)
Les motifs anciens et les contours architecturaux en arrière-plan sont progressivement simplifiés et le temps passe tranquillement à l'espace moderne. La grenade est placée sur un comptoir moderne, et le plateau et les ustensiles sont présentés avec une géométrie plane simple. Les visions anciennes et modernes sont reliées dans la même image, et le rythme de l'image passe du « voyage » à « l'arrivée ».
Plan 5 : Couper la grenade, point culminant visuel (16-20 secondes)
Coupez délicatement la grenade d'une seule main, en effectuant des mouvements lents et retenus. Le moment où la peau s’ouvre est très rituel.
Shot 6 : Pressé dans du jus qui coule abondamment (20-24 secondes)
Les graines entrent dans le récipient et sont pressées dans un riche jus de grenade. Le liquide s'écoule avec une texture rouge foncé et transparente, avec de fines particules couleur roche. Le jus de grenade est versé lentement dans un verre moderne. Le contour du verre est clair et concis. Le liquide rouge monte dans le verre, avec de légères ondulations et reflets en surface. Quelques glaçons tombèrent dans la tasse, et le blanc froid et le rouge profond contrastaient fortement. De fines gouttelettes d'eau sont apparues sur la paroi de la tasse et la sensation rafraîchissante a été comblée.
Plan 7 : Boire moderne, parcours jusqu'à l'achèvement (24-27 secondes)
L'arrière-plan est découpé dans une scène de vie moderne, et la lumière des fenêtres, le dessus de table, les tissus et les plantes conservent des éléments décoratifs plats et des couleurs chaudes. La tasse de jus est placée au centre de l'image, avec des motifs de routes anciennes, de caravanes de chameaux et de portes de la ville vaguement superposés autour d'elle, suggérant que cette tasse de jus provient d'un long voyage. L'atmosphère est riche, chaleureuse et calme.
Plan 8 : Le temps converge, fin en forme d'affiche (27-30 secondes)
Les anciennes routes en arrière-plan se fondent progressivement dans l’espace moderne, comme le temps converge dans ce verre de jus. L'image revient brièvement sur la grenade sur la branche, l'ombre du chameau sur l'ancienne route et les graines rouges, formant un circuit complet « du sol à la coupe ». Enfin, il est rassemblé dans une composition semblable à une affiche publicitaire : du jus de grenade rouge foncé est placé au centre, avec une grenade concassée à côté de la tasse, entourée d'anciens modèles de routes, de points lumineux dorés et d'éléments de la vie moderne. L’image est calme mais pleine de vitalité, comme un voyage à travers le temps et le territoire qui arrive enfin au moment présent. Le slogan publicitaire est « la semence, un cadeau des régions de l'Ouest ».
```

---

## Repousser les limites narratives

### Case 13: Briser les frontières du récit - 30 secondes de continuité - sortie - 1

[![Briser les frontières du récit - 30 secondes de continuité - sortie - 1](assets/thumbnails/13-narrative-control-13-30-second-continuous-output-group-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab1/group1/output.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab1/group1/output.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 8

**Prompt:**

```text
De gauche à droite, la caméra suit régulièrement un homme en manteau noir (voir<<<image_1_1>>>) à travers six pièces connectées de couleurs et d'atmosphères différentes. La structure de chaque pièce est la même : murs blancs, parquet en bois clair à chevrons, doubles baies vitrées et rideaux de gaze blanche, font référence à<<<image_2_2>>>, mais le paysage à l'extérieur de la fenêtre et l'atmosphère intérieure sont complètement différents. Le protagoniste se déplace à une vitesse constante tout au long du jeu, passant par toutes les portes ouvertes sur le mur.
0-5 secondes, la première salle, le thème est le combat de bande dessinée américaine, le protagoniste entre dans la pièce et combat le personnage (<<<image_3_3>>>), le personnage perd ;
5-10 secondes, la deuxième pièce, le thème est chaleureux, style feutre, la scène à l'extérieur de la fenêtre est un champ de tournesols (<<<image_4_4>>>), la lumière intérieure est orange chaude et douce, et un peintre peint des tournesols (<<<image_5_5>>>). Le protagoniste se transforme également en feutre après être entré ;
10-15 secondes, la troisième pièce, le thème est la tristesse, l'image entière est dans le style d'une animation stop-motion comique en noir et blanc, il pleut devant la fenêtre, la lumière à l'intérieur est froide et grise, une personne est assise seule par terre au centre de la pièce vide, baissant la tête et serrant ses genoux, et un téléphone portable à côté de lui allume l'interface d'appel sans que personne ne réponde. Une fois que le protagoniste est entré dans la pièce, il éteint les lumières de la pièce et les allume immédiatement. La pièce devient colorée et les fleurs poussent partout dans la maison en un instant ;
15-20 secondes, la quatrième salle, le thème est la joie, toute la scène est une pièce trempée dans la mer, référez-vous à<<<image_6_6>>>, le protagoniste nage dans la pièce, avec de magnifiques récifs coralliens et des bancs de poissons à côté de lui ;
20-25 secondes, la cinquième pièce, le thème est la surprise, la scène à l'extérieur de la fenêtre est pleine de feux d'artifice dans le ciel nocturne, référez-vous à<<<image_7_7>>>, la lumière intérieure est colorée et vacillante et le protagoniste est impliqué dans l'atmosphère joyeuse.
Après 25 à 30 secondes, le protagoniste arrive enfin dans une pièce vide, se tient au centre et claque des doigts. En même temps, l'effet sonore est un claquement, tout l'écran est noir et le mot « seedance » apparaît au milieu, reportez-vous à<<<image_8_8>>>.
La qualité globale du film est un style publicitaire de mode haut de gamme. La lumière est entièrement déterminée par la scène à l’extérieur de la fenêtre, créant ainsi un fort contraste émotionnel. Il n'y a pas de texte dans l'image.
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

### Case 14: Briser les frontières du récit - 30 secondes de continuité - sortie - 2

[![Briser les frontières du récit - 30 secondes de continuité - sortie - 2](assets/thumbnails/14-narrative-control-14-30-second-continuous-output-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab1/group2/output.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab1/group2/output.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 3

**Prompt:**

```text
Produire une courte vidéo scientifique de vulgarisation de 30 secondes sur les trois mille ans d’évolution du football. Tout le film utilise la même balle comme ligne visuelle principale. La balle roule, voyage et se déforme depuis les temps anciens, reliant différentes civilisations et époques. Le rythme général est compact, les graphismes sont haut de gamme, le court métrage scientifique historique se combine avec des transitions artistiques pour mettre en valeur la sensation d'un bal s'étendant sur trois mille ans, et la diffusion orale est simple et puissante.
Au début, une boule ancienne est apparue lentement sur le fond noir avec une texture du temps à la surface, puis a roulé dans une scène Cuju de la période des Royaumes combattants en Chine. L'image s'est transformée en un style à l'encre, faisant référence au style de<<<image_1_1>>>. Les anciens vêtus de costumes anciens jouaient au Cuju dans la cour avec des mouvements élégants et la balle rebondissait sous leurs pieds. Diffusion orale : Histoire de football, à commencer par Cuju.
Ensuite, la balle continue de rouler vers l'avant et l'image passe naturellement à une scène de jeu de balle grecque antique. L'image est dans le style d'une peinture à l'huile classique et le style fait référence à<<<image_2_2>>>. L'arrière-plan des piliers carrés et en pierre est évident, et les gens portant des robes grecques anciennes jouent au football. L’image est épaisse et historique. Bouche à oreille : les Grecs aiment aussi les jeux de ballon.
Ensuite, le bal a roulé dans l’Europe médiévale, et le tableau a toujours conservé le style de la peinture à l’huile. Les villages, les champs de boue et les gens ordinaires couraient après le ballon. L’atmosphère était chaleureuse et rude, tout comme le football folklorique ancien continuant le feu. Diffusion orale : les Européens continuent le match de football.
Ensuite, le ballon a été expulsé et l'écran est passé à un style documentaire en noir et blanc. En parlant de<<<image_3_3>>>, nous sommes arrivés en Angleterre en 1863. Petit à petit, les gentlemen, les clubs et les terrains en herbe sont apparus, symbolisant la naissance officielle du football moderne. Ce ballon a montré pour la première fois l’apparence standard du football moderne. Parlées : 1863, le football moderne prend forme.
Ensuite, la scène entre rapidement dans l’ère moderne, avec la balle tournant dans les airs, faisant apparaître à leur tour des nœuds clés du développement. Les lumières, le stade, les spectateurs, les trophées et les différentes scènes du monde s'entremêlent, montrant que le football a évolué d'un sport local à un sport mondial.
À la fin, le ballon se trouve au centre d'un stade moderne, et les foules et les acclamations du monde entier se fondent en arrière-plan, formant le sentiment d'un « ballon reliant le monde ». L'image est grandiose et épique. Diffusion orale : Désormais, le football connecte le monde entier.
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

### Case 15: Briser les frontières du récit - 30 secondes de continuité - sortie - 3

[![Briser les frontières du récit - 30 secondes de continuité - sortie - 3](assets/thumbnails/15-narrative-control-15-30-second-continuous-output-group-3.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab1/group3/output.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab1/group3/output.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 6

**Prompt:**

```text
Une vidéo tutorielle de 30 secondes sur l'installation et l'utilisation d'une machine à café à capsules.
0-2 secondes, le texte du titre au début est : tutoriel d'installation et d'utilisation de la machine à café à capsules seedance
2 à 5 secondes, étape 1 : installez le réservoir d'eau, reportez-vous à<<<image_1_1>>>Objectif : Plan moyen, vue légèrement aérienne Position : Action sur l'arrière du fuselage : Alignez le réservoir d'eau avec la fente à l'arrière du fuselage, poussez-le verticalement vers le bas et entendez un « clic » pour le verrouiller en place. Exigences : affichez clairement la relation d'alignement entre la boucle au bas du réservoir d'eau et la fente sur le fuselage, et la ligne de niveau d'eau est visible dans la partie transparente du réservoir d'eau.
Narrateur : « Tout d’abord, installez le réservoir d’eau. »
5 à 9 secondes, étape 2 : installez le bac d'égouttement, reportez-vous à<<<image_2_2>>>Objectif : Gros plan, vue de face, Position : Devant le bas du fuselage, Action : Poussez le bac d'égouttage dans le rail de guidage au bas du fuselage en parallèle, poussez-le jusqu'à ce que le fond soit complètement ajusté, Exigences : Montrez le processus d'alignement du rail de guidage, mettez en évidence la douceur de l'action de glissement.
Narrateur : « Ensuite, alignez la palette avec les rails inférieurs. »
9-13 secondes, étape 3 : Installez la boîte de collecte des capsules de déchets, reportez-vous à<<<image_3_3>>>Objectif : Gros plan, angle de vue légèrement surélevé, Position : Cavité sous le bac collecteur, Action : Aligner le bac de récupération avec la rainure et l'enfoncer, au ras du bac collecteur. Exigences : montrer la relation d'ajustement entre la boîte de collecte et le fuselage et confirmer qu'elle est installée en place
Narrateur : « Ensuite, mettez-le dans la boîte de collecte des capsules. »
13-18 secondes, étape 4 : première injection d'eau, reportez-vous à<<<image_4_4>>>Objectif : gros plan, vue latérale, position : réservoir d'eau sur le dessus/à l'arrière du fuselage, action : ouvrir le couvercle du réservoir d'eau, verser de l'eau jusqu'au niveau d'eau MAX, fermer le couvercle du réservoir d'eau, exigences : mettre en évidence la marque de niveau d'eau et le versement de l'eau est clairement visible
Narrateur : « Ouvrez le couvercle du réservoir d'eau et versez de l'eau propre. Faites attention à ne pas dépasser le niveau d'eau maximum. »
L'écran met en évidence le niveau d'eau maximum.
18-25 secondes, étape 5 : mise sous tension, reportez-vous à<<<image_5_5>>>Plan : Plan moyen, vue de face, Position : Avant du fuselage, Action : Branchez le cordon d'alimentation, appuyez sur le bouton d'alimentation, le voyant passe de clignotant à fixe (préchauffage terminé), Conditions requises : Gros plan sur les changements d'état du bouton d'alimentation et du voyant, reflétant le processus d'attente jusqu'à ce que vous soyez prêt.
Narrateur : « Branchez l'alimentation et appuyez sur le bouton d'alimentation. »
25-30 secondes, étape 6 : premier rinçage (sans placer la capsule), se référer à<<<image_6_6>>>Objectif : plan moyen en gros plan, vue de face, position : avant du fuselage, tasse sous la sortie d'eau, action : appuyer directement sur le bouton d'extraction sans insérer la capsule, l'eau chaude s'écoule du tuyau de rinçage, et l'eau s'écoule dans la tasse. Exigences : Insistez sur la marque d'invite « Pas besoin de mettre une capsule » et montrez l'ensemble du processus d'évacuation de l'eau.
Narrateur : "La dernière étape consiste à rincer une première fois. Pas besoin de mettre la capsule, il suffit d'appuyer sur le bouton d'extraction. Votre machine à café est prête à être utilisée officiellement."
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

### Case 16: Repousser les limites narratives-Plus de références Entrée-Sortie-1

[![Repousser les limites narratives-Plus de références Entrée-Sortie-1](assets/thumbnails/16-narrative-control-16-multi-reference-input-group-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/output.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/output.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 17

**Prompt:**

```text
Instructions de base : Un court métrage narratif unique de 26 secondes, avec un suivi et un entrelacement stables, voir<<<video_1_1>>>, et un mouvement surround fluide, voir<<<video_2_2>>>. Sensation de voyage douce. L'alternance du jour et de la nuit et le flux des quatre saisons sont réalisés dans l'objectif. Le protagoniste est une femme européenne<<<image_1_3>>>, placée dans une mer de gens pleine de feux d'artifice, soulignant le sentiment ultime de solitude et la qualité de la cinématographie.
Mouvement de caméra segmenté et description de la scène :
0-3 secondes (dos lisse) : La vieille porte en bois<<<image_2_4>>>s'ouvre avec un grincement, et la caméra suit la silhouette d'une Européenne portant<<<image_3_5>>>qui sort. Il s'arrêta légèrement sur le seuil. Les rues devant étaient tachetées de lumière et d'ombre, et les bruits des colportages et des foules approchaient. Elle avait l'air distante et marchait lentement dans la rue.
3-6 secondes (tracking arrière et latéral) : La caméra assure un suivi fluide, elle entre dans le marché matinal bondé, l'ambiance fait référence à<<<video_3_6>>>. Les deux côtés étaient remplis d'étals de fruits colorés et de magasins d'épices, et un groupe de jongleurs de rue crachait des dragons de feu, voir<<<image_4_7>>>. La lueur du feu illuminait la foule, mais elle ne louchait pas et marchait à un rythme régulier.
6 à 9 secondes (Smooth Surround from the Side) : La caméra commence à s'enrouler en douceur sur le côté et à l'avant, capturant le visage latéral du protagoniste. Elle est passée devant la boucherie bruyante<<<image_5_8>>>, et une jeune maman est passée à côté de lui tenant un bébé<<<image_6_9>>>. Le bébé la regarda avec curiosité, mais elle baissa juste légèrement les yeux pour éviter de regarder, sans s'arrêter du tout.
9 à 12 secondes (prise de vue de suivi avant et arrière) : la caméra continue de tourner directement devant le protagoniste et effectue une prise de vue en arrière et en suivi. La foule devant lui s'est soudainement retirée des deux côtés, naturellement, comme Moïse séparant la mer. Un énorme éléphant<<<image_7_10>>>recouvert d'un magnifique tissu rouge est apparu du côté droit de l'écran à un rythme régulier, occupant la majeure partie de l'écran.
12-15 secondes (pénétration de l'espace et rembobinage) : Au moment où la femme et l'éléphant sont sur le point d'entrer en collision, la caméra glisse intelligemment à travers l'étroit espace entre l'éléphant et la femme, recirculant vers son dos. Les éléphants passaient massivement et silencieusement, et les oursins les poursuivaient avec joie. Comme les cloches et les rires, elle n'a même pas ralenti.
15 à 18 secondes (dégradé de lumière ambiante et d'ombre) : au fur et à mesure qu'elle marche, la lumière et l'ombre dans le plan long changent comme par magie : la lumière du soleil éblouissante du milieu de l'été s'adoucit instantanément, une brise enroule les feuilles dorées<<<video_2_2>>>0 dans le ciel et la saison passe en douceur à la fin de l'automne dans le même plan long. Les feuilles mortes lui effleuraient les épaules.
18-21 secondes (surround immersif à 360 degrés) : La façade se transforme soudainement en une grande fête de rue<<<video_2_2>>>1. Des rubans colorés et du papier déchiqueté ont jailli dans les airs et les vendeurs se sont penchés pour applaudir. A ce moment, la caméra déploie un mouvement panoramique continu à 360 degrés, créant une déchirure visuelle extrêmement forte entre le protagoniste calme et solitaire et l'environnement frénétique.
21-24 secondes (tournant d'un côté à l'autre) : Lorsque la caméra a fait un tour et est revenue à ses côtés et à l'arrière, les rubans qui tombaient s'étaient tranquillement transformés en neige partout dans le ciel - c'était l'hiver en un instant<<<video_2_2>>>2. Les piétons brandissaient des parapluies ou enfilaient des cagoules, et les femmes rétrécissaient légèrement, relevaient le col de leur manteau, se changeaient en<<<video_2_2>>>3 et continuaient à marcher seules dans la neige.
24-26 secondes (poussée et battement lents) : Alors qu'elle marchait vers la fin de la longue rue, le ciel s'est assombri à une vitesse visible à l'œil nu et le jour s'est enfoncé harmonieusement dans la nuit. Les lampadaires tamisés des deux côtés et les ampoules des stands se sont allumés l'une après l'autre<<<video_2_2>>>4. Les vendeurs emballaient leurs marchandises. Le bruit semblait être lentement absorbé et éloigné par la neige abondante, et ses pas ralentissaient progressivement. De grands feux d'artifice ont soudainement fleuri dans le ciel nocturne<<<video_2_2>>>5, le bruit des feux d'artifice en fleurs fait référence à<<<video_2_2>>>6. Des points lumineux colorés clignotaient et sautaient sur les murs du bâtiment et dans ses yeux. Le monde est toujours vivant, mais elle lève les yeux tranquillement, la caméra fait un zoom arrière lentement et se termine ici doucement.
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

### Case 17: Briser les frontières de la narration-plus de référence entrée-référence vidéo-1-1

[![Briser les frontières de la narration-plus de référence entrée-référence vidéo-1-1](assets/thumbnails/17-reference-asset-17-multi-reference-input-group-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/reference1.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/reference1.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 17

**Prompt:**

```text
Instructions de base : Un court métrage narratif unique de 26 secondes, avec un suivi et un entrelacement stables, voir<<<video_1_1>>>, et un mouvement surround fluide, voir<<<video_2_2>>>. Sensation de voyage douce. L'alternance du jour et de la nuit et le flux des quatre saisons sont réalisés dans l'objectif. Le protagoniste est une femme européenne<<<image_1_3>>>, placée dans une mer de gens pleine de feux d'artifice, soulignant le sentiment ultime de solitude et la qualité de la cinématographie.
Mouvement de caméra segmenté et description de la scène :
0-3 secondes (dos lisse) : La vieille porte en bois<<<image_2_4>>>s'ouvre avec un grincement, et la caméra suit la silhouette d'une Européenne portant<<<image_3_5>>>qui sort. Il s'arrêta légèrement sur le seuil. Les rues devant étaient tachetées de lumière et d'ombre, et les bruits des colportages et des foules approchaient. Elle avait l'air distante et marchait lentement dans la rue.
3-6 secondes (tracking arrière et latéral) : La caméra assure un suivi fluide, elle entre dans le marché matinal bondé, l'ambiance fait référence à<<<video_3_6>>>. Les deux côtés étaient remplis d'étals de fruits colorés et de magasins d'épices, et un groupe de jongleurs de rue crachait des dragons de feu, voir<<<image_4_7>>>. La lueur du feu illuminait la foule, mais elle ne louchait pas et marchait à un rythme régulier.
6 à 9 secondes (Smooth Surround from the Side) : La caméra commence à s'enrouler en douceur sur le côté et à l'avant, capturant le visage latéral du protagoniste. Elle est passée devant la boucherie bruyante<<<image_5_8>>>, et une jeune maman est passée à côté de lui tenant un bébé<<<image_6_9>>>. Le bébé la regarda avec curiosité, mais elle baissa juste légèrement les yeux pour éviter de regarder, sans s'arrêter du tout.
9 à 12 secondes (prise de vue de suivi avant et arrière) : la caméra continue de tourner directement devant le protagoniste et effectue une prise de vue en arrière et en suivi. La foule devant lui s'est soudainement retirée des deux côtés, naturellement, comme Moïse séparant la mer. Un énorme éléphant<<<image_7_10>>>recouvert d'un magnifique tissu rouge est apparu du côté droit de l'écran à un rythme régulier, occupant la majeure partie de l'écran.
12-15 secondes (pénétration de l'espace et rembobinage) : Au moment où la femme et l'éléphant sont sur le point d'entrer en collision, la caméra glisse intelligemment à travers l'étroit espace entre l'éléphant et la femme, recirculant vers son dos. Les éléphants passaient massivement et silencieusement, et les oursins les poursuivaient avec joie. Comme les cloches et les rires, elle n'a même pas ralenti.
15 à 18 secondes (dégradé de lumière ambiante et d'ombre) : au fur et à mesure qu'elle marche, la lumière et l'ombre dans le plan long changent comme par magie : la lumière du soleil éblouissante du milieu de l'été s'adoucit instantanément, une brise enroule les feuilles dorées<<<video_2_2>>>0 dans le ciel et la saison passe en douceur à la fin de l'automne dans le même plan long. Les feuilles mortes lui effleuraient les épaules.
18-21 secondes (surround immersif à 360 degrés) : La façade se transforme soudainement en une grande fête de rue<<<video_2_2>>>1. Des rubans colorés et du papier déchiqueté ont jailli dans les airs et les vendeurs se sont penchés pour applaudir. A ce moment, la caméra déploie un mouvement panoramique continu à 360 degrés, créant une déchirure visuelle extrêmement forte entre le protagoniste calme et solitaire et l'environnement frénétique.
21-24 secondes (tournant d'un côté à l'autre) : Lorsque la caméra a fait un tour et est revenue à ses côtés et à l'arrière, les rubans qui tombaient s'étaient tranquillement transformés en neige partout dans le ciel - c'était l'hiver en un instant<<<video_2_2>>>2. Les piétons brandissaient des parapluies ou enfilaient des cagoules, et les femmes rétrécissaient légèrement, relevaient le col de leur manteau, se changeaient en<<<video_2_2>>>3 et continuaient à marcher seules dans la neige.
24-26 secondes (poussée et battement lents) : Alors qu'elle marchait vers la fin de la longue rue, le ciel s'est assombri à une vitesse visible à l'œil nu et le jour s'est enfoncé harmonieusement dans la nuit. Les lampadaires tamisés des deux côtés et les ampoules des stands se sont allumés l'une après l'autre<<<video_2_2>>>4. Les vendeurs emballaient leurs marchandises. Le bruit semblait être lentement absorbé et éloigné par la neige abondante, et ses pas ralentissaient progressivement. De grands feux d'artifice ont soudainement fleuri dans le ciel nocturne<<<video_2_2>>>5, le bruit des feux d'artifice en fleurs fait référence à<<<video_2_2>>>6. Des points lumineux colorés clignotaient et sautaient sur les murs du bâtiment et dans ses yeux. Le monde est toujours vivant, mais elle lève les yeux tranquillement, la caméra fait un zoom arrière lentement et se termine ici doucement.
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

### Case 18: Briser les frontières du récit-plus de référence entrée-référence vidéo-1-2

[![Briser les frontières du récit-plus de référence entrée-référence vidéo-1-2](assets/thumbnails/18-reference-asset-18-multi-reference-input-group-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/reference2.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/reference2.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 17

**Prompt:**

```text
Instructions de base : Un court métrage narratif unique de 26 secondes, avec un suivi et un entrelacement stables, voir<<<video_1_1>>>, et un mouvement surround fluide, voir<<<video_2_2>>>. Sensation de voyage douce. L'alternance du jour et de la nuit et le flux des quatre saisons sont réalisés dans l'objectif. Le protagoniste est une femme européenne<<<image_1_3>>>, placée dans une mer de gens pleine de feux d'artifice, soulignant le sentiment ultime de solitude et la qualité de la cinématographie.
Mouvement de caméra segmenté et description de la scène :
0-3 secondes (dos lisse) : La vieille porte en bois<<<image_2_4>>>s'ouvre avec un grincement, et la caméra suit la silhouette d'une Européenne portant<<<image_3_5>>>qui sort. Il s'arrêta légèrement sur le seuil. Les rues devant étaient tachetées de lumière et d'ombre, et les bruits des colportages et des foules approchaient. Elle avait l'air distante et marchait lentement dans la rue.
3-6 secondes (tracking arrière et latéral) : La caméra assure un suivi fluide, elle entre dans le marché matinal bondé, l'ambiance fait référence à<<<video_3_6>>>. Les deux côtés étaient remplis d'étals de fruits colorés et de magasins d'épices, et un groupe de jongleurs de rue crachait des dragons de feu, voir<<<image_4_7>>>. La lueur du feu illuminait la foule, mais elle ne louchait pas et marchait à un rythme régulier.
6 à 9 secondes (Smooth Surround from the Side) : La caméra commence à s'enrouler en douceur sur le côté et à l'avant, capturant le visage latéral du protagoniste. Elle est passée devant la boucherie bruyante<<<image_5_8>>>, et une jeune maman est passée à côté de lui tenant un bébé<<<image_6_9>>>. Le bébé la regarda avec curiosité, mais elle baissa juste légèrement les yeux pour éviter de regarder, sans s'arrêter du tout.
9 à 12 secondes (prise de vue de suivi avant et arrière) : la caméra continue de tourner directement devant le protagoniste et effectue une prise de vue en arrière et en suivi. La foule devant lui s'est soudainement retirée des deux côtés, naturellement, comme Moïse séparant la mer. Un énorme éléphant<<<image_7_10>>>recouvert d'un magnifique tissu rouge est apparu du côté droit de l'écran à un rythme régulier, occupant la majeure partie de l'écran.
12-15 secondes (pénétration de l'espace et rembobinage) : Au moment où la femme et l'éléphant sont sur le point d'entrer en collision, la caméra glisse intelligemment à travers l'étroit espace entre l'éléphant et la femme, recirculant vers son dos. Les éléphants passaient massivement et silencieusement, et les oursins les poursuivaient avec joie. Comme les cloches et les rires, elle n'a même pas ralenti.
15 à 18 secondes (dégradé de lumière ambiante et d'ombre) : au fur et à mesure qu'elle marche, la lumière et l'ombre dans le plan long changent comme par magie : la lumière du soleil éblouissante du milieu de l'été s'adoucit instantanément, une brise enroule les feuilles dorées<<<video_2_2>>>0 dans le ciel et la saison passe en douceur à la fin de l'automne dans le même plan long. Les feuilles mortes lui effleuraient les épaules.
18-21 secondes (surround immersif à 360 degrés) : La façade se transforme soudainement en une grande fête de rue<<<video_2_2>>>1. Des rubans colorés et du papier déchiqueté ont jailli dans les airs et les vendeurs se sont penchés pour applaudir. A ce moment, la caméra déploie un mouvement panoramique continu à 360 degrés, créant une déchirure visuelle extrêmement forte entre le protagoniste calme et solitaire et l'environnement frénétique.
21-24 secondes (tournant d'un côté à l'autre) : Lorsque la caméra a fait un tour et est revenue à ses côtés et à l'arrière, les rubans qui tombaient s'étaient tranquillement transformés en neige partout dans le ciel - c'était l'hiver en un instant<<<video_2_2>>>2. Les piétons brandissaient des parapluies ou enfilaient des cagoules, et les femmes rétrécissaient légèrement, relevaient le col de leur manteau, se changeaient en<<<video_2_2>>>3 et continuaient à marcher seules dans la neige.
24-26 secondes (poussée et battement lents) : Alors qu'elle marchait vers la fin de la longue rue, le ciel s'est assombri à une vitesse visible à l'œil nu et le jour s'est enfoncé harmonieusement dans la nuit. Les lampadaires tamisés des deux côtés et les ampoules des stands se sont allumés l'une après l'autre<<<video_2_2>>>4. Les vendeurs emballaient leurs marchandises. Le bruit semblait être lentement absorbé et éloigné par la neige abondante, et ses pas ralentissaient progressivement. De grands feux d'artifice ont soudainement fleuri dans le ciel nocturne<<<video_2_2>>>5, le bruit des feux d'artifice en fleurs fait référence à<<<video_2_2>>>6. Des points lumineux colorés clignotaient et sautaient sur les murs du bâtiment et dans ses yeux. Le monde est toujours vivant, mais elle lève les yeux tranquillement, la caméra fait un zoom arrière lentement et se termine ici doucement.
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

### Case 19: Briser les frontières de la narration-plus de référence entrée-référence vidéo-1-6

[![Briser les frontières de la narration-plus de référence entrée-référence vidéo-1-6](assets/thumbnails/19-reference-asset-19-multi-reference-input-group-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/reference6.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group1/reference6.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 17

**Prompt:**

```text
Instructions de base : Un court métrage narratif unique de 26 secondes, avec un suivi et un entrelacement stables, voir<<<video_1_1>>>, et un mouvement surround fluide, voir<<<video_2_2>>>. Sensation de voyage douce. L'alternance du jour et de la nuit et le flux des quatre saisons sont réalisés dans l'objectif. Le protagoniste est une femme européenne<<<image_1_3>>>, placée dans une mer de gens pleine de feux d'artifice, soulignant le sentiment ultime de solitude et la qualité de la cinématographie.
Mouvement de caméra segmenté et description de la scène :
0-3 secondes (dos lisse) : La vieille porte en bois<<<image_2_4>>>s'ouvre avec un grincement, et la caméra suit la silhouette d'une Européenne portant<<<image_3_5>>>qui sort. Il s'arrêta légèrement sur le seuil. Les rues devant étaient tachetées de lumière et d'ombre, et les bruits des colportages et des foules approchaient. Elle avait l'air distante et marchait lentement dans la rue.
3-6 secondes (tracking arrière et latéral) : La caméra assure un suivi fluide, elle entre dans le marché matinal bondé, l'ambiance fait référence à<<<video_3_6>>>. Les deux côtés étaient remplis d'étals de fruits colorés et de magasins d'épices, et un groupe de jongleurs de rue crachait des dragons de feu, voir<<<image_4_7>>>. La lueur du feu illuminait la foule, mais elle ne louchait pas et marchait à un rythme régulier.
6 à 9 secondes (Smooth Surround from the Side) : La caméra commence à s'enrouler en douceur sur le côté et à l'avant, capturant le visage latéral du protagoniste. Elle est passée devant la boucherie bruyante<<<image_5_8>>>, et une jeune maman est passée à côté de lui tenant un bébé<<<image_6_9>>>. Le bébé la regarda avec curiosité, mais elle baissa juste légèrement les yeux pour éviter de regarder, sans s'arrêter du tout.
9 à 12 secondes (prise de vue de suivi avant et arrière) : la caméra continue de tourner directement devant le protagoniste et effectue une prise de vue en arrière et en suivi. La foule devant lui s'est soudainement retirée des deux côtés, naturellement, comme Moïse séparant la mer. Un énorme éléphant<<<image_7_10>>>recouvert d'un magnifique tissu rouge est apparu du côté droit de l'écran à un rythme régulier, occupant la majeure partie de l'écran.
12-15 secondes (pénétration de l'espace et rembobinage) : Au moment où la femme et l'éléphant sont sur le point d'entrer en collision, la caméra glisse intelligemment à travers l'étroit espace entre l'éléphant et la femme, recirculant vers son dos. Les éléphants passaient massivement et silencieusement, et les oursins les poursuivaient avec joie. Comme les cloches et les rires, elle n'a même pas ralenti.
15 à 18 secondes (dégradé de lumière ambiante et d'ombre) : au fur et à mesure qu'elle marche, la lumière et l'ombre dans le plan long changent comme par magie : la lumière du soleil éblouissante du milieu de l'été s'adoucit instantanément, une brise enroule les feuilles dorées<<<video_2_2>>>0 dans le ciel et la saison passe en douceur à la fin de l'automne dans le même plan long. Les feuilles mortes lui effleuraient les épaules.
18-21 secondes (surround immersif à 360 degrés) : La façade se transforme soudainement en une grande fête de rue<<<video_2_2>>>1. Des rubans colorés et du papier déchiqueté ont jailli dans les airs et les vendeurs se sont penchés pour applaudir. A ce moment, la caméra déploie un mouvement panoramique continu à 360 degrés, créant une déchirure visuelle extrêmement forte entre le protagoniste calme et solitaire et l'environnement frénétique.
21-24 secondes (tournant d'un côté à l'autre) : Lorsque la caméra a fait un tour et est revenue à ses côtés et à l'arrière, les rubans qui tombaient s'étaient tranquillement transformés en neige partout dans le ciel - c'était l'hiver en un instant<<<video_2_2>>>2. Les piétons brandissaient des parapluies ou enfilaient des cagoules, et les femmes rétrécissaient légèrement, relevaient le col de leur manteau, se changeaient en<<<video_2_2>>>3 et continuaient à marcher seules dans la neige.
24-26 secondes (poussée et battement lents) : Alors qu'elle marchait vers la fin de la longue rue, le ciel s'est assombri à une vitesse visible à l'œil nu et le jour s'est enfoncé harmonieusement dans la nuit. Les lampadaires tamisés des deux côtés et les ampoules des stands se sont allumés l'une après l'autre<<<video_2_2>>>4. Les vendeurs emballaient leurs marchandises. Le bruit semblait être lentement absorbé et éloigné par la neige abondante, et ses pas ralentissaient progressivement. De grands feux d'artifice ont soudainement fleuri dans le ciel nocturne<<<video_2_2>>>5, le bruit des feux d'artifice en fleurs fait référence à<<<video_2_2>>>6. Des points lumineux colorés clignotaient et sautaient sur les murs du bâtiment et dans ses yeux. Le monde est toujours vivant, mais elle lève les yeux tranquillement, la caméra fait un zoom arrière lentement et se termine ici doucement.
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

### Case 20: Repousser les limites narratives-Plus de références Entrée-Sortie-2

[![Repousser les limites narratives-Plus de références Entrée-Sortie-2](assets/thumbnails/20-narrative-control-20-multi-reference-input-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/output.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/output.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 7

**Prompt:**

```text
Le style de la publicité est lumineux et coloré, avec des biscuits fruités comme protagonistes, comprenant quatre saveurs : fraise, pomme, raisin et orange. La saveur fraise fait référence à<<<image_1_1>>>. Les biscuits et les fruits correspondants sont disposés selon un agencement géométrique avec un fort sens de l'ordre. L’image globale est claire, avancée et rythmée. Le fruit d'ouverture établit rapidement le focus visuel, faisant référence à la composition de<<<video_1_2>>>, et la musique est ré-battue. Ensuite, les biscuits aux différentes saveurs sont soigneusement disposés et découpés en gros plans, faisant référence à la dynamique et aux mouvements de caméra de<<<video_2_3>>>. Pendant l'apogée, un biscuit se brise et passe instantanément au ralenti. Le sandwich fruité explose, les miettes volent et l'impact du jus et des particules est amplifié et affiché. Reportez-vous à l’impact de<<<video_3_4>>>. Le réseau horizontal forme une parabole rythmique, faisant référence au mouvement de<<<video_4_5>>>, soulignant la beauté de l'ordre et la richesse des produits. Puis revenez rapidement au montage rapide. Le texte anglais final Une bouchée de croustillant, un cœur plein de délice est rapidement intégré à l'image, combiné avec le mouvement du texte au rythme fort et l'arrêt sur image du produit, se référer à<<<video_5_6>>>, et enfin le sens de la marque est enveloppé, et les biscuits et les fruits sont étalés dans toutes les directions, se référer à<<<video_6_7>>>. L'image est pleine de jeunes, énergiques, délicieux et veulent partager une atmosphère publicitaire.
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

### Case 21: Briser les frontières du récit-plus de référence entrée-référence vidéo-2-2

[![Briser les frontières du récit-plus de référence entrée-référence vidéo-2-2](assets/thumbnails/21-reference-asset-21-multi-reference-input-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference2.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference2.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 7

**Prompt:**

```text
Le style de la publicité est lumineux et coloré, avec des biscuits fruités comme protagonistes, comprenant quatre saveurs : fraise, pomme, raisin et orange. La saveur fraise fait référence à<<<image_1_1>>>. Les biscuits et les fruits correspondants sont disposés selon un agencement géométrique avec un fort sens de l'ordre. L’image globale est claire, avancée et rythmée. Le fruit d'ouverture établit rapidement le focus visuel, faisant référence à la composition de<<<video_1_2>>>, et la musique est ré-battue. Ensuite, les biscuits aux différentes saveurs sont soigneusement disposés et découpés en gros plans, faisant référence à la dynamique et aux mouvements de caméra de<<<video_2_3>>>. Pendant l'apogée, un biscuit se brise et passe instantanément au ralenti. Le sandwich fruité explose, les miettes volent et l'impact du jus et des particules est amplifié et affiché. Reportez-vous à l’impact de<<<video_3_4>>>. Le réseau horizontal forme une parabole rythmique, faisant référence au mouvement de<<<video_4_5>>>, soulignant la beauté de l'ordre et la richesse des produits. Puis revenez rapidement au montage rapide. Le texte anglais final Une bouchée de croustillant, un cœur plein de délice est rapidement intégré à l'image, combiné avec le mouvement du texte au rythme fort et l'arrêt sur image du produit, se référer à<<<video_5_6>>>, et enfin le sens de la marque est enveloppé, et les biscuits et les fruits sont étalés dans toutes les directions, se référer à<<<video_6_7>>>. L'image est pleine de jeunes, énergiques, délicieux et veulent partager une atmosphère publicitaire.
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

### Case 22: Briser les limites du récit-plus de référence entrée-référence vidéo-2-3

[![Briser les limites du récit-plus de référence entrée-référence vidéo-2-3](assets/thumbnails/22-reference-asset-22-multi-reference-input-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference3.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference3.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 7

**Prompt:**

```text
Le style de la publicité est lumineux et coloré, avec des biscuits fruités comme protagonistes, comprenant quatre saveurs : fraise, pomme, raisin et orange. La saveur fraise fait référence à<<<image_1_1>>>. Les biscuits et les fruits correspondants sont disposés selon un agencement géométrique avec un fort sens de l'ordre. L’image globale est claire, avancée et rythmée. Le fruit d'ouverture établit rapidement le focus visuel, faisant référence à la composition de<<<video_1_2>>>, et la musique est ré-battue. Ensuite, les biscuits aux différentes saveurs sont soigneusement disposés et découpés en gros plans, faisant référence à la dynamique et aux mouvements de caméra de<<<video_2_3>>>. Pendant l'apogée, un biscuit se brise et passe instantanément au ralenti. Le sandwich fruité explose, les miettes volent et l'impact du jus et des particules est amplifié et affiché. Reportez-vous à l’impact de<<<video_3_4>>>. Le réseau horizontal forme une parabole rythmique, faisant référence au mouvement de<<<video_4_5>>>, soulignant la beauté de l'ordre et la richesse des produits. Puis revenez rapidement au montage rapide. Le texte anglais final Une bouchée de croustillant, un cœur plein de délice est rapidement intégré à l'image, combiné avec le mouvement du texte au rythme fort et l'arrêt sur image du produit, se référer à<<<video_5_6>>>, et enfin le sens de la marque est enveloppé, et les biscuits et les fruits sont étalés dans toutes les directions, se référer à<<<video_6_7>>>. L'image est pleine de jeunes, énergiques, délicieux et veulent partager une atmosphère publicitaire.
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

### Case 23: Briser les frontières de la narration-plus de référence entrée-référence vidéo-2-4

[![Briser les frontières de la narration-plus de référence entrée-référence vidéo-2-4](assets/thumbnails/23-reference-asset-23-multi-reference-input-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference4.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference4.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 7

**Prompt:**

```text
Le style de la publicité est lumineux et coloré, avec des biscuits fruités comme protagonistes, comprenant quatre saveurs : fraise, pomme, raisin et orange. La saveur fraise fait référence à<<<image_1_1>>>. Les biscuits et les fruits correspondants sont disposés selon un agencement géométrique avec un fort sens de l'ordre. L’image globale est claire, avancée et rythmée. Le fruit d'ouverture établit rapidement le focus visuel, faisant référence à la composition de<<<video_1_2>>>, et la musique est ré-battue. Ensuite, les biscuits aux différentes saveurs sont soigneusement disposés et découpés en gros plans, faisant référence à la dynamique et aux mouvements de caméra de<<<video_2_3>>>. Pendant l'apogée, un biscuit se brise et passe instantanément au ralenti. Le sandwich fruité explose, les miettes volent et l'impact du jus et des particules est amplifié et affiché. Reportez-vous à l’impact de<<<video_3_4>>>. Le réseau horizontal forme une parabole rythmique, faisant référence au mouvement de<<<video_4_5>>>, soulignant la beauté de l'ordre et la richesse des produits. Puis revenez rapidement au montage rapide. Le texte anglais final Une bouchée de croustillant, un cœur plein de délice est rapidement intégré à l'image, combiné avec le mouvement du texte au rythme fort et l'arrêt sur image du produit, se référer à<<<video_5_6>>>, et enfin le sens de la marque est enveloppé, et les biscuits et les fruits sont étalés dans toutes les directions, se référer à<<<video_6_7>>>. L'image est pleine de jeunes, énergiques, délicieux et veulent partager une atmosphère publicitaire.
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

### Case 24: Briser les limites du récit-plus de référence entrée-référence vidéo-2-5

[![Briser les limites du récit-plus de référence entrée-référence vidéo-2-5](assets/thumbnails/24-reference-asset-24-multi-reference-input-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference5.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference5.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 7

**Prompt:**

```text
Le style de la publicité est lumineux et coloré, avec des biscuits fruités comme protagonistes, comprenant quatre saveurs : fraise, pomme, raisin et orange. La saveur fraise fait référence à<<<image_1_1>>>. Les biscuits et les fruits correspondants sont disposés selon un agencement géométrique avec un fort sens de l'ordre. L’image globale est claire, avancée et rythmée. Le fruit d'ouverture établit rapidement le focus visuel, faisant référence à la composition de<<<video_1_2>>>, et la musique est ré-battue. Ensuite, les biscuits aux différentes saveurs sont soigneusement disposés et découpés en gros plans, faisant référence à la dynamique et aux mouvements de caméra de<<<video_2_3>>>. Pendant l'apogée, un biscuit se brise et passe instantanément au ralenti. Le sandwich fruité explose, les miettes volent et l'impact du jus et des particules est amplifié et affiché. Reportez-vous à l’impact de<<<video_3_4>>>. Le réseau horizontal forme une parabole rythmique, faisant référence au mouvement de<<<video_4_5>>>, soulignant la beauté de l'ordre et la richesse des produits. Puis revenez rapidement au montage rapide. Le texte anglais final Une bouchée de croustillant, un cœur plein de délice est rapidement intégré à l'image, combiné avec le mouvement du texte au rythme fort et l'arrêt sur image du produit, se référer à<<<video_5_6>>>, et enfin le sens de la marque est enveloppé, et les biscuits et les fruits sont étalés dans toutes les directions, se référer à<<<video_6_7>>>. L'image est pleine de jeunes, énergiques, délicieux et veulent partager une atmosphère publicitaire.
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

### Case 25: Briser les limites du récit-plus de référence entrée-référence vidéo-2-6

[![Briser les limites du récit-plus de référence entrée-référence vidéo-2-6](assets/thumbnails/25-reference-asset-25-multi-reference-input-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference6.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference6.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 7

**Prompt:**

```text
Le style de la publicité est lumineux et coloré, avec des biscuits fruités comme protagonistes, comprenant quatre saveurs : fraise, pomme, raisin et orange. La saveur fraise fait référence à<<<image_1_1>>>. Les biscuits et les fruits correspondants sont disposés selon un agencement géométrique avec un fort sens de l'ordre. L’image globale est claire, avancée et rythmée. Le fruit d'ouverture établit rapidement le focus visuel, faisant référence à la composition de<<<video_1_2>>>, et la musique est ré-battue. Ensuite, les biscuits aux différentes saveurs sont soigneusement disposés et découpés en gros plans, faisant référence à la dynamique et aux mouvements de caméra de<<<video_2_3>>>. Pendant l'apogée, un biscuit se brise et passe instantanément au ralenti. Le sandwich fruité explose, les miettes volent et l'impact du jus et des particules est amplifié et affiché. Reportez-vous à l’impact de<<<video_3_4>>>. Le réseau horizontal forme une parabole rythmique, faisant référence au mouvement de<<<video_4_5>>>, soulignant la beauté de l'ordre et la richesse des produits. Puis revenez rapidement au montage rapide. Le texte anglais final Une bouchée de croustillant, un cœur plein de délice est rapidement intégré à l'image, combiné avec le mouvement du texte au rythme fort et l'arrêt sur image du produit, se référer à<<<video_5_6>>>, et enfin le sens de la marque est enveloppé, et les biscuits et les fruits sont étalés dans toutes les directions, se référer à<<<video_6_7>>>. L'image est pleine de jeunes, énergiques, délicieux et veulent partager une atmosphère publicitaire.
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

### Case 26: Briser les frontières de la narration-plus de référence entrée-référence vidéo-2-7

[![Briser les frontières de la narration-plus de référence entrée-référence vidéo-2-7](assets/thumbnails/26-reference-asset-26-multi-reference-input-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference7.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab2/group2/reference7.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 7

**Prompt:**

```text
Le style de la publicité est lumineux et coloré, avec des biscuits fruités comme protagonistes, comprenant quatre saveurs : fraise, pomme, raisin et orange. La saveur fraise fait référence à<<<image_1_1>>>. Les biscuits et les fruits correspondants sont disposés selon un agencement géométrique avec un fort sens de l'ordre. L’image globale est claire, avancée et rythmée. Le fruit d'ouverture établit rapidement le focus visuel, faisant référence à la composition de<<<video_1_2>>>, et la musique est ré-battue. Ensuite, les biscuits aux différentes saveurs sont soigneusement disposés et découpés en gros plans, faisant référence à la dynamique et aux mouvements de caméra de<<<video_2_3>>>. Pendant l'apogée, un biscuit se brise et passe instantanément au ralenti. Le sandwich fruité explose, les miettes volent et l'impact du jus et des particules est amplifié et affiché. Reportez-vous à l’impact de<<<video_3_4>>>. Le réseau horizontal forme une parabole rythmique, faisant référence au mouvement de<<<video_4_5>>>, soulignant la beauté de l'ordre et la richesse des produits. Puis revenez rapidement au montage rapide. Le texte anglais final Une bouchée de croustillant, un cœur plein de délice est rapidement intégré à l'image, combiné avec le mouvement du texte au rythme fort et l'arrêt sur image du produit, se référer à<<<video_5_6>>>, et enfin le sens de la marque est enveloppé, et les biscuits et les fruits sont étalés dans toutes les directions, se référer à<<<video_6_7>>>. L'image est pleine de jeunes, énergiques, délicieux et veulent partager une atmosphère publicitaire.
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

### Case 27: Briser les limites du contrôle d'écran de deuxième niveau narratif-sortie-1

[![Briser les limites du contrôle d'écran de deuxième niveau narratif-sortie-1](assets/thumbnails/27-narrative-control-27-second-level-frame-control-group-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab3/group1/output.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab3/group1/output.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 1

**Prompt:**

```text
Le style publicitaire d'animation 3D, les couleurs vives et transparentes, ainsi que la pulpe et le jus doivent avoir une forte sensation de fraîcheur et d'impact. Le tempérament général ressemble à celui d'un court métrage d'animation commercial de haute qualité avec un peu d'humour exagéré. Le personnage du lézard à cornes du désert est mignon, intelligent et expressif. Veuillez vous référer à<<<image_1_1>>>. La texture de l'image fait référence à la douce lumière naturelle, à la texture fine des peluches/peau, à la profondeur de champ macro de rêve et à une véritable sensation enfantine dans l'image.
0-3 secondes : La photo montre un désert exposé au soleil brûlant. L'air était déformé par la chaleur, le sable était chaud et de la fumée semblait s'élever au loin. Un lézard à cornes du désert gisait sur le sable chaud, la langue légèrement pendante, les yeux flous, presque desséchés par le soleil. Il fit deux pas et se balança, et tout le lézard à cornes du désert était sur le point de « s'évaporer ».
Les effets sonores incluent le vrombissement des vagues de chaleur et un crépitement sec légèrement exagéré.
3-6 secondes : Le lézard à cornes du désert s'arrête soudainement et bouge son nez. Il baissa les yeux et vit un pamplemousse froid et dodu avec des gouttes d'eau enfouies dans le sable. Le pamplemousse brille de mille feux au soleil, avec une peau délicate, comme un miracle apparu soudainement dans le désert.
Les yeux du lézard performant s'écarquillèrent instantanément, comme s'il voyait une paille qui sauve des vies.
L'effet sonore "ding" est un effet sonore de découverte.
6-8 secondes : Le lézard à cornes du désert fond, serre le pamplemousse à deux mains et appuie tout son visage contre la peau. Il a une joyeuse expression de « enfin vivant ». L'image se fige pendant 1 seconde, formant un point mémoire publicitaire exagéré et drôle.
L’effet sonore s’est effondré, puis est resté silencieux pendant une demi-seconde.
Secondes 8 à 11 : capture d'écran d'un lézard à cornes du désert attrapant un pamplemousse. La peau du pamplemousse est ouverte et la chair charnue à l’intérieur brille de manière translucide. L'instant d'après, le jus ne s'est pas écoulé, mais a été craché comme un tsunami.
L'effet sonore est un « clic » de morsure ouvert, suivi d'un bruit exagéré de jus éclatant.
11-16 secondes : L'écran montre du jus de pamplemousse rose orangé, clair et brillant, qui s'écoule follement, se déverse sur les dunes de sable et inonde rapidement tout le désert. Le sable jaune sec se transforme instantanément en un océan d’été frais, pétillant et fruité. Les cactus, les pierres et les petites dunes de sable du désert sont engloutis par les vagues de jus, et l'image est exagérée et rêveuse.
La performance du Lézard à Cornes du Désert était très excitante au début, mais la seconde suivante, j'ai réalisé que quelque chose n'allait pas et mon expression est passée de la surprise à l'horreur.
16-20 secondes : Le lézard à cornes du désert est presque immergé dans la « mer de pamplemousse ». Il serre précipitamment la moitié du pamplemousse et flotte sur la mer comme une bouée de sauvetage. Il sortit la tête mouillée, avec une expression confuse. La surface de la mer est scintillante, la couleur est comme le jus illuminé par le soleil.
Les effets sonores exagèrent le bruit des battements et des vagues, avec un sentiment de comédie.
20-23 secondes : l'écran passe soudainement à un écran blanc. Le nom de la marque et le slogan apparaissaient au centre de l'écran : « Pamplemousse Seedance, ce qu'on mord c'est la pulpe, ce qui sort c'est l'été ».
Le narrateur lit la phrase entière : « Pamplemousse Seedance, ce que vous mordez, c'est la pulpe, ce qui sort, c'est l'été.
Tonalité de marque avec un son clair et rafraîchissant.
23-29 secondes : L'écran revient à l'écran blanc. Le lézard à cornes du désert est déjà assis tranquillement sur un pamplemousse flottant, portant une paire de petites lunettes de soleil, tenant une tasse à bec et flottant lentement sur la « mer de jus » pour les vacances. De la pulpe d'orange, des petits glaçons et des éclaboussures d'eau fraîche flottaient, le ciel est devenu bleu et l'atmosphère est soudainement passée de « survie » à « vacances ». À la fin, le lézard à cornes du désert s'est posé avec contentement sur le pamplemousse et la caméra a effectué un zoom arrière, se figeant dans une scène estivale rafraîchissante, lumineuse et amusante.
Effets sonores, musique d'été relaxante, bruit des vagues.
Les sous-titres ne peuvent conserver que le nom de la marque, sans ajouter trop de mots.
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

### Case 28: Briser les limites du contrôle d'écran de deuxième niveau narratif-sortie-2

[![Briser les limites du contrôle d'écran de deuxième niveau narratif-sortie-2](assets/thumbnails/28-narrative-control-28-second-level-frame-control-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab3/group2/output.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part1/tab3/group2/output.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 1

**Prompt:**

```text
Court métrage cinématographique de 30 secondes sur les courses de jeunes, style d'animation 2D. Le protagoniste est un jeune pilote qui conduit une moto pour participer à des compétitions de haut niveau. Le style général est passionné, jeune, émotionnellement intense et cinématographique, avec un début complet, une transition et un arc émotionnel clair. Seuls deux types de mouvements de caméra sont utilisés dans l'ensemble du film : le suivi à grande vitesse et le surround au ralenti. Il y a très peu de lignes et elles apparaissent naturellement comme des fragments de mémoire. Le ton est sincère, doux et retenu, sans crier de slogans ni trop sensationnalisme. Ne ressentez pas le désastre, ne vous exprimez pas négativement et n’exagérez pas la science-fiction. Il se concentre sur l'amour, le soutien, la contre-attaque et la croissance dans la course de la jeunesse.
0 seconde à 5 secondes
La piste commence au crépuscule avec des courses rapides et intenses. La caméra suit au ras du sol la moto du jeune homme à grande vitesse. Les pneus effleurent le bord de la piste. La moto rugit, le vent souffle violemment et l’ambiance est tendue et enflammée. Le jeune homme était concentré et le soleil couchant dessinait des reflets nets sur la coque métallique de la voiture.
5 secondes à 9 secondes
Après être entré dans un virage clé, le garçon a été soudainement dépassé par son adversaire. Le suivi à grande vitesse s'est poursuivi et l'image montrait le sentiment oppressant de la baisse du classement et de la perturbation du rythme. En vue rapprochée du casque, on constate une perte temporaire de concentration, une respiration difficile et de légers tremblements. Le garçon murmura : "Puis-je encore rattraper mon retard..."
9 secondes à 14 secondes
Le garçon a pris du retard, sa respiration est devenue plus lourde et son humeur a atteint un point bas. La course ne s'est pas arrêtée et la locomotive avançait toujours à grande vitesse. La scène a commencé à rappeler des fragments de mémoire chaleureux lors d'une conduite à grande vitesse : alors qu'il apprenait à conduire étant enfant, quelqu'un l'a soutenu par derrière ; son père lui a arrangé son casque, ses mouvements étaient méticuleux et silencieux ; avant la ligne d'arrivée, un doux sourire le regardait ; et les personnages de dos marchant côte à côte sur la pente au crépuscule. Ces souvenirs sont présentés avec un rétroéclairage doré, un ralenti doux et des sentiments fragmentés.
14 secondes à 18 secondes
La musique passe progressivement de dépressive à édifiante. Une voix retenue et douce sortit du souvenir : « N'ayez pas peur, je suis toujours là. "Restez stable. Et regardez vers l'avant." Les yeux du jeune homme se recentrèrent, sa respiration se stabilisa lentement et son humeur passa d'hésitante à ferme.
18 secondes à 23 secondes
Le jeune homme reprit confiance, accéléra de toutes ses forces et contre-attaqua avec précision. Les travellings à grande vitesse montrent la puissance et le contrôle de la moto dans les virages, à la sortie des virages et à l'approche de la voiture qui précède. Le garçon dit doucement mais fermement : « Je ne m'arrêterai pas là.
23 secondes à 27 secondes
Une piste ascendante apparut devant nous et le garçon sprinta à toute vitesse contre le soleil couchant. L'image ne conserve que le bruit de la respiration, les bruits du moteur et la musique qui monte continuellement, sans ajouter de lignes inutiles. La locomotive s'est envolée dans les airs grâce à l'inertie et est entrée au ralenti choquant. Une voix douce avec un sourire est venue du plus profond de ma mémoire : « Continue.
27 secondes à 30 secondes
La caméra fait le tour de la locomotive dans les airs pour un gros plan panoramique au ralenti. Poussez les émotions de passion, de tendresse, de liberté et de saut vers le haut jusqu'au point culminant. Les fleurs s'épanouissent derrière vous, suivies d'une semence, reportez-vous à<<<image_1_1>>>
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

## Développer la présentation multilingue

### Case 29: Développer la présentation multilingue-expression multilingue-sortie-1

[![Développer la présentation multilingue-expression multilingue-sortie-1](assets/thumbnails/29-multilingual-expression-29-group-1.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part3/group1/output.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part3/group1/output.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 11

**Prompt:**

```text
Vidéo à la première personne du drone FPV One-shot, 33 secondes de plan long continu, pas de montage, pas de sauts, pas de transitions. La caméra part de l'intérieur des nuages ​​de haute altitude et forme une ligne de vol descendante continue le long des nuages, du brouillard, de la lumière et de l'ombre, des vallées, des cascades, des lacs, des champs de fleurs, des bâtiments urbains et des places proches du sol. 11 blocs d'affichage de langage clairs et indépendants apparaissent en séquence tout au long du processus. Chaque bloc affiche uniquement le texte correspondant à une seule langue. Il n’y a pas de mélange, de chevauchement ou d’ajout d’autres langues.
0 à 3 secondes, les nuages ​​<<<image_1_1>>>forment naturellement « Bonjour » en chinois ;
3 à 6 secondes,<<<image_2_2>>>Brume et lumière volumétrique forment l'anglais « Hello » ;
6 à 9 secondes,<<<image_3_3>>>Projection de vapeur d'eau et de lumière du soleil à haute altitude formant le « Hola » espagnol (Mexique) ;
9 à 12 secondes,<<<image_4_4>>>Ruban dans le ciel formant le mot indonésien « Halo » ;
12 à 15 secondes, formation de cerfs-volants<<<image_5_5>>>formant « Hai » en malais ;
15 à 18 secondes, la brume matinale de<<<image_6_6>>>Valley forme un « สวัสดี » thaïlandais ;
18–21 secondes<<<image_7_7>>>Brume de cascade formant l'arabe مرحبا
21-24 secondes,<<<image_8_8>>>Le reflet sur le lac et les ondulations forment le mot portugais « Olá » ;
24–27 secondes,<<<image_9_9>>>Les champs de fleurs et les prairies sont naturellement disposés en « Xin chào » vietnamien ;
27 à 30 secondes,<<<image_10_10>>>Les bâtiments en verre de la ville reflètent la lumière et l'ombre pour former le mot japonais « こんにちは » ;
30 à 33 secondes,<<<image_2_2>>>0 Le brouillard d'eau de la fontaine à proximité, le revêtement de sol et les bandes lumineuses forment le mot coréen « 안녕하세요 ».
L'atmosphère générale est celle d'un lever de soleil tôt le matin, avec un rétroéclairage doré, une lumière volumétrique douce, de vrais nuages ​​et brouillard, un flou de mouvement naturel et un réalisme de niveau film. La vitesse de la caméra commence lentement de 3 à 5 m/s, accélère progressivement jusqu'à 14 à 16 m/s à travers le paysage naturel, puis ralentit jusqu'à 2 à 3 m/s pour planer de manière stable dans le carré proche de la Terre. Paramètres de l'objectif : objectif grand angle, 24 ips, mouvement fluide du drone FPV, transition progressive de -5° à -18°, et revient finalement à 0° ; léger lacet ±10°, roulis contrôlé entre 0 et 10°, assurant une sensation de vol continue, stable et réaliste d'un tir à l'autre.
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

### Case 30: Développer la présentation multilingue-expression-sortie multilingue-2

[![Développer la présentation multilingue-expression-sortie multilingue-2](assets/thumbnails/30-multilingual-expression-30-group-2.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part3/group2/output.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part3/group2/output.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 9

**Prompt:**

```text
Style d'action en direct, montage rapide, sensation cinématographique, 4K, 24 ips, lumière naturelle chaude, performances réelles des personnages, synchronisation labiale naturelle, pas de sous-titres. Prenant la livraison d'une fleur comme indice visuel principal de toute la vidéo, la fleur se propage rapidement d'un pays à l'autre, reliant différentes régions et personnes à travers le monde. Dans chaque scène, un personnage prend les fleurs, sourit sincèrement et dit « merci » dans la langue locale. Le rythme général est vif et fluide, et les plans sont dynamiques, mettant l'accent sur la véritable atmosphère de la rue et de la vie, les liens interculturels chaleureux et la transmission de la bonne volonté entre les gens.
Méthode de transition : Dans le plan précédent, un personnage a tendu la fleur hors de l'écran, et dans le plan suivant, un autre personnage a attrapé la fleur dans la nouvelle scène.
Ou utilisez le panoramique rapide, le flou de mouvement ou l'occlusion du premier plan pour effectuer des transitions fluides.
Maintenez la continuité visuelle des fleurs dans l'image pour créer le sentiment d'un « one shot se propageant à travers le monde ».
Style d'objectif : prise de vue de suivi à main levée, léger tremblement de l'objectif, poussée et traction rapides, combinaison de gros plans et de plans moyens, atmosphère sonore ambiante réelle et texture de prise de vue de rue au niveau du film. La musique de fond est chaleureuse, vive et donne une impression de voyage dans le monde, et la fin s'estompe doucement.
Scène 1<<<image_1_1>>>Dans un magasin de fleurs chinois, une scène réelle. La fille a pris une rose, a regardé la caméra, a souri et a dit naturellement : « Merci ! La caméra a suivi les fleurs depuis le côté droit de l'écran et la jeune fille a doucement soulevé le bouquet après avoir reçu les fleurs.
Scène 2<<<image_2_2>>>Les rues d'Angleterre, temps légèrement frais, scène de rue naturelle. L'homme a pris un œillet, a souri, a hoché la tête et a dit : « Merci ! Lors de la transition, la fleur a été projetée de la scène précédente vers cette scène.
Scène 3<<<image_3_3>>>Marché mexicain, riche en couleurs et plein de feux d'artifice. La tante prit le bouquet de soucis, joignit les mains et dit chaleureusement : « ¡Gracias ! La caméra a rapidement survolé le stand et la foule, et le moment de la réception des fleurs a été figé.
Scène 4<<<image_4_4>>>Campagne indonésienne, la lumière naturelle du soleil brille. L'enfant a pris un plumeria, a souri joyeusement, s'est légèrement incliné et a dit : « Terima kasih ! La caméra avait l'impression de courir et l'atmosphère était pure et naturelle.
Scène 5<<<image_5_5>>>Les rues de Thaïlande regorgent de monde. Le vendeur prit un bouquet de guirlandes de jasmin, joignit les mains et dit gentiment : « ขอบคุณค่ะ ! » La caméra avançait vivement et les guirlandes se balançaient légèrement au soleil.
Scène 6<<<image_6_6>>>Cour arabe, lumière et ombre douces, environnement élégant. La dame a pris une rose du désert, lui a caressé la poitrine, a souri et a dit : « شكراً ! L'image était calme et chaleureuse, et l'expression du personnage était sincère.
Scène 7<<<image_7_7>>>Communauté brésilienne, l'ambiance est chaleureuse et animée. Le garçon a pris un gerbera et était très heureux et a dit : "Obrigado !" Le plan est rythmé et plein de vie.
Scène 8<<<image_8_8>>>Dans une rue japonaise, un employé de bureau a pris une petite fleur dans la boîte à lunch, s'est incliné poliment et a dit : "ありがとう !" Le plan était court et soigné, conservant le sens du rythme urbain.
Scène 9<<<image_9_9>>>Rues coréennes, ambiance urbaine moderne. La jeune femme a pris une branche d'azalée, a naturellement croisé les mains, a souri et a dit : « 감사합니다 ! La caméra s'est arrêtée un instant alors qu'elle souriait, puis la scène s'est doucement estompée.
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

## Édition contrôlable plus approfondie

### Case 31: Sortie d'édition 1 contrôlée

[![Sortie d'édition 1 contrôlée](assets/thumbnails/31-controllable-editing-31-edited-output.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group1/output.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group1/output.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 2

**Prompt:**

```text
Gardez les personnages, l'environnement de la jungle, le mouvement de la caméra, la composition, le rythme de l'action et la durée de<<<video_1_1>>>inchangés.
Un arc énergétique bleu-blanc et une flèche lumineuse<<<image_1_2>>>apparaissent lentement dans la main du personnage. Le corps de l'arc est progressivement formé par la polymérisation d'arcs et de particules faibles, avec une texture de courant délicate, une légère lumière volumétrique et un contour énergétique stable. Pendant le processus de tirage de l'arc, la flèche se condense en une flèche d'énergie très lumineuse au centre de la corde de l'arc. Au moment où le personnage lâche prise, la flèche jaillit à grande vitesse, laissant une trajectoire énergétique lumineuse, fine, continue et nette.
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

### Case 32: Édition contrôlée 1 Référence

[![Édition contrôlée 1 Référence](assets/thumbnails/32-controllable-editing-32-reference.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group1/reference1.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group1/reference1.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 2

**Prompt:**

```text
Gardez les personnages, l'environnement de la jungle, le mouvement de la caméra, la composition, le rythme de l'action et la durée de<<<video_1_1>>>inchangés.
Un arc énergétique bleu-blanc et une flèche lumineuse<<<image_1_2>>>apparaissent lentement dans la main du personnage. Le corps de l'arc est progressivement formé par la polymérisation d'arcs et de particules faibles, avec une texture de courant délicate, une légère lumière volumétrique et un contour énergétique stable. Pendant le processus de tirage de l'arc, la flèche se condense en une flèche d'énergie très lumineuse au centre de la corde de l'arc. Au moment où le personnage lâche prise, la flèche jaillit à grande vitesse, laissant une trajectoire énergétique lumineuse, fine, continue et nette.
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

### Case 33: Sortie d'édition 2 contrôlée

[![Sortie d'édition 2 contrôlée](assets/thumbnails/33-controllable-editing-33-edited-output.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group2/output.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group2/output.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 1

**Prompt:**

```text
Supprimez le drone dans l'écran<<<video_1_1>>>et le bord de la piste/de la carrosserie au premier plan dans le coin inférieur gauche, et complétez naturellement la zone supprimée.
Gardez le groupe de girafes, les branches d'arbres, les prairies lointaines, le rétroéclairage doré du coucher de soleil, la perspective aérienne et la composition de la prise de vue complètement inchangés. L'arrière-plan terminé doit être cohérent avec l'environnement environnant, générant le ciel naturel, les espaces entre les branches d'arbres et les détails de l'herbe sans bavures, scintillement, déformation, images fantômes ou battements. Assurez-vous que le timing des images avant et arrière de la vidéo est cohérent, que le mouvement est continu, que les transitions de bord sont naturelles et que l'image globale ressemble à l'image réelle d'origine.
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

### Case 34: Référence de l'édition contrôlée 2

[![Référence de l'édition contrôlée 2](assets/thumbnails/34-controllable-editing-34-reference.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group2/reference1.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group2/reference1.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 1

**Prompt:**

```text
Supprimez le drone dans l'écran<<<video_1_1>>>et le bord de la piste/de la carrosserie au premier plan dans le coin inférieur gauche, et complétez naturellement la zone supprimée.
Gardez le groupe de girafes, les branches d'arbres, les prairies lointaines, le rétroéclairage doré du coucher de soleil, la perspective aérienne et la composition de la prise de vue complètement inchangés. L'arrière-plan terminé doit être cohérent avec l'environnement environnant, générant le ciel naturel, les espaces entre les branches d'arbres et les détails de l'herbe sans bavures, scintillement, déformation, images fantômes ou battements. Assurez-vous que le timing des images avant et arrière de la vidéo est cohérent, que le mouvement est continu, que les transitions de bord sont naturelles et que l'image globale ressemble à l'image réelle d'origine.
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

### Case 35: Sortie d'édition 3 contrôlée

[![Sortie d'édition 3 contrôlée](assets/thumbnails/35-controllable-editing-35-edited-output.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group3/output.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group3/output.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 4

**Prompt:**

```text
Remplacement de la version originale de la vidéo d'arts martiaux à deux<<<video_1_1>>>par un test du vent les mains vides avant un duel d'armes froides.
La scène est remplacée par une plate-forme de château médiéval en pierre, une ancienne cour d'appartement, une plate-forme extérieure de forteresse de montagne ou un simple champ de duel en briques de pierre. L'arrière-plan est l'ancien mur du château, le vent, le brouillard, la ligne de montagne lointaine, et le sol est plat et en pierre<<<image_1_2>>>.
Les vêtements de l'homme en vêtements sombres dans la vidéo sont remplacés par<<<image_2_3>>>, et les vêtements de l'homme en vêtements clairs dans la vidéo sont remplacés par<<<image_3_4>>>. L'action reste la même, sans changer le rythme original.
Les effets spéciaux de l'IA ne font qu'améliorer l'environnement et la texture : vêtements soufflés par le vent, léger brouillard, une petite quantité de poussière aux points de contact, texture métallique réfléchissante à froid, légères particules et palette de couleurs épique. Le style général est sobre, réaliste et offre une atmosphère de duel hardcore classique. Musique de fond bloquée
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

### Case 36: Référence de l'édition contrôlée 3

[![Référence de l'édition contrôlée 3](assets/thumbnails/36-controllable-editing-36-reference.jpg)](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group3/reference1.mp4)

[Lire la vidéo](https://ark-common-storage-prod-cn-beijing.tos-cn-beijing.volces.com/presets/experience/gen_video/model-promotion/seedance-2-5/part2/group3/reference1.mp4) · Cliquez sur la miniature pour lire la vidéo.

**Ressources de référence:** 4

**Prompt:**

```text
Remplacement de la version originale de la vidéo d'arts martiaux à deux<<<video_1_1>>>par un test du vent les mains vides avant un duel d'armes froides.
La scène est remplacée par une plate-forme de château médiéval en pierre, une ancienne cour d'appartement, une plate-forme extérieure de forteresse de montagne ou un simple champ de duel en briques de pierre. L'arrière-plan est l'ancien mur du château, le vent, le brouillard, la ligne de montagne lointaine, et le sol est plat et en pierre<<<image_1_2>>>.
Les vêtements de l'homme en vêtements sombres dans la vidéo sont remplacés par<<<image_2_3>>>, et les vêtements de l'homme en vêtements clairs dans la vidéo sont remplacés par<<<image_3_4>>>. L'action reste la même, sans changer le rythme original.
Les effets spéciaux de l'IA ne font qu'améliorer l'environnement et la texture : vêtements soufflés par le vent, léger brouillard, une petite quantité de poussière aux points de contact, texture métallique réfléchissante à froid, légères particules et palette de couleurs épique. Le style général est sobre, réaliste et offre une atmosphère de duel hardcore classique. Musique de fond bloquée
```

> [!NOTE]
> Ce cas officiel inclut aussi des ressources de référence listées dans le manifest.

---

## 📁 Structure du dépôt

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

## 🙏 Remerciements

Ce dépôt est maintenu par EvoLink comme guide public pour Seedance 2.5 early access.

- Official early access: [Get Seedance 2.5 Early Access](https://evolink.ai/launch/seedance-2-5?utm_source=github&utm_medium=readme&utm_campaign=awesome-seedance-2.5-guide)
- Current API key path: [EvoLink signup](https://evolink.ai/signup?utm_source=github&utm_medium=readme&utm_campaign=awesome-seedance-2.5-guide)
- Current API examples: [Seedance 2.5 Gateway Service](https://github.com/EvoLinkAI/Seedance-2.5-Gateway-Service)
