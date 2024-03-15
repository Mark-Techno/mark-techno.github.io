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
  overlay_image: /assets/images/GunCupido.PNG
---

# Virtueel en realiteit smelten samen
Naast VR (Virtual Reality) hebben we ook AR (Augmented Reality) tijdens de cursus behandeld. In tegenstelling tot VR waarbij je zintuigen enigzins afgesloten worden van de buitenwereld en je je volledig in een virtuele omgeving bevind, is AR een mix waarbij virtuele elementen bovenop de realiteit worden geplaatst (denk aan Google glasses of de filters op snapchat). Tijdens de avond bijeenkomst hebben wij gewerkt met platformen die je in staat stellen om 3D objecten te projecteren bovenop de beeld van een mobieltje camera. Dit vond ik interessant waardoor ik verder ben gegaan met deze technologie.

# RoboEgg vliegt rond in een ruimte
Uiteindelijk heb ik in de web applicatie en mobiele app "CoSpaces" een wereld gemaakt waarbij een 3D gescande robot geprojecteerd wordt op het beeld van de camera en een rondje vliegt. Het leuke is dat, met behulp van verschillende sensoren in het mobieltje, behoudt de robot enigzins zijn positie in de driedimensionale ruimte. Ook al loop je rond of draai je om de robot heen je kan de robot op dezelfde positie terug vinden, al dan niet opgeschoven omdat de tracking niet perfect is en omdat de robot natuurlijk een rondje vliegt.

__Voeg video toe van RoboEgg die rond vliegt__

# Kan ik ook deze robot in mijn ruimte bekijken?
Dat kan, deze "space" staat openbaar beschikbaar in de CoSpaces app. Je hebt hiervoor dus CoSpaces app nodig waarmee je de volgende link kan invullen of simpelweg de QR-code onder deze tekst kan inscannen. Dan zodra je in de space zit, tik je op het scherm om de robot te plaatsen.

![Cospaces QR code naar EggRobo applicatie](/assets/images/eggrobo-%20cospaces-AR-QR.png)

# Hoe is dit gemaakt?
## 3D scan
Dit project begon met mijn interesse in de 3D scanner beschikbaar in het HUB-lab. Doordeweeks was ik langs gekomen om deze te proberen te gebruiken met een klein figuurtje dat ik had meegenomen. Nadat het figuurtje een tijdje had gedraaid op de schijf langs de scanner, kwam een verassend gedetaileerde 3D model met al toegevoegde textures eruit. Dit 3D object bestond echter uit veel polygons waardoor het object duur zou zijn om te verwerken op een apparaat. Om deze reden had ik het object geimporteerd in Blender en verder geoptimaliseerd. Waarbij de totale bestandsgrootte van het 3D object werd terug gebracht van +100mb naar ~5mb. Vooral het aantal polygons was flink terug gebracht, wat op zich niet heel erg opvalt.

__Voeg video toe van scanner en beeld__

## Cospace
De cospace wereld heb ik vrij eenvoudig gehouden waarbij de robot is geimporteerd met de correcte animatie laag (het op en neer bewegen van de robot en heen en weer kijken is geanimeerd in Blender). In de CoSpaces project ruimte is een cirkel toegevoegd met een script dat zegt dat de EggRobo dit cirkel moet volgen. Verder is een vuur particle vast gemaakt aan de achterkant van de raket uitlaat.

__Voeg plaatje toe van Cospaces project__