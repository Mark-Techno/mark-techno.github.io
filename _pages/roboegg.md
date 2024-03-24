---
layout: single
read_time: false
comments: false
share: false
author_profile: false
title: <br><br><br><br><br>RoboEgg in AR
permalink: /AR-RoboEgg/
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/AR-eggrobo-screencap.jpg
feature_row:
  - image_path: /assets/images/outside/ar-mechanic.jpg
    alt: "Facilitating Mechanical Design with 
Augmented Reality"
    title: "Facilitating Mechanical Design with 
Augmented Reality"
    url: "https://dspace.mit.edu/bitstream/handle/1721.1/7448/IMST009.pdf;sequence=1"
    btn_label: "Paper"
    btn_class: "btn--inverse"
  - image_path: /assets/images/outside/what-is-ar.jpg
    alt: "What Is Augmented Reality?"
    title: "What Is Augmented Reality?"
    url: "https://builtin.com/machine-learning/augmented-reality"
    btn_label: "Blog"
    btn_class: "btn--inverse"
---

# Virtueel en realiteit smelten samen
Naast VR (Virtual Reality) hebben we ook AR (Augmented Reality) tijdens de cursus behandeld. In tegenstelling tot VR waarbij je zintuigen enigzins afgesloten worden van de buitenwereld en je je volledig in een virtuele omgeving bevind, is AR een mix waarbij virtuele elementen bovenop de realiteit worden geplaatst (denk aan Google glasses of de filters op snapchat). Tijdens de avond bijeenkomst hebben wij gewerkt met platformen die je in staat stellen om 3D objecten te projecteren bovenop de camera beeld van een mobieltje. Dit vond ik interessant waardoor ik verder ben gegaan met deze technologie.

# RoboEgg vliegt rond in een ruimte
Uiteindelijk heb ik in de web applicatie en mobiele app [CoSpaces](https://www.cospaces.io/) een wereld gemaakt waarbij een 3D ingescande robot, geprojecteerd wordt op het beeld van de camera en een rondje vliegt. Het leuke is dat, met behulp van verschillende sensoren in het mobieltje, de positie van de robot enigzins bewaart wordt. Ook al loop je rond of draai je om de robot heen, de robot kan op dezelfde positie terug gevonden worden, al dan niet opgeschoven omdat de tracking niet perfect is en de robot natuurlijk een rondje vliegt.

{% include video id="8T8D_Zt-x-E" provider="youtube" %}

# Kan ik ook deze robot in mijn ruimte bekijken?
Dat kan, deze "space" staat openbaar beschikbaar in de CoSpaces app. Je hebt hiervoor dus de CoSpaces app op je mobieltje nodig waarbij je de QR-code onder deze tekst kan inscannen of de code "MNYZCV invult. Dan zodra je in de space zit, tik je op het scherm om de robot te plaatsen.

![Cospaces QR code naar EggRobo applicatie](/assets/images/eggrobo-%20cospaces-AR-QR.png)

# Hoe is dit gemaakt?
## 3D scan
Dit project begon met mijn interesse in de 3D scanner, dat beschikbaar is in het HUB-lab. Doordeweeks was ik langs gekomen om deze te proberen te gebruiken met een klein figuurtje dat ik had meegenomen. Nadat het figuurtje een tijdje had gedraaid op de schijf langs de scanner, kwam een verassend gedetaileerde 3D model met al toegevoegde textures eruit. Dit 3D object bestond echter uit veel polygons waardoor het object duur zou zijn om te verwerken/visualiseren op een apparaat. Om deze reden had ik het object geimporteerd in Blender en verder geoptimaliseerd. Waarbij de totale bestandsgrootte van het 3D object werd terug gebracht van +100mb naar ~5mb. Vooral het aantal polygons was flink terug gebracht, wat op zich niet heel erg opvalt in het eindresultaat.

{% include video id="wlD69OwzI4M" provider="youtube" %}

## Cospaces
De Cospaces wereld heb ik vrij eenvoudig gehouden waarbij de robot is geimporteerd met de correcte animatie laag (het op en neer bewegen en rond kijken van de robot is geanimeerd in Blender). In de CoSpaces project ruimte is een cirkel toegevoegd met een script dat de instructie geeft aan de EggRobo om deze cirkel te volgen. Verder is een vuur particle vast gemaakt aan de achterkant van de raket uitlaat.

![Playground project in Cospaces](/assets/images/cospaces.jpg)

# Verdere interessante artikelen over AR
<div id='featured'></div>

{% include feature_row %}