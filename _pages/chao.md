---
layout: single
read_time: false
comments: false
share: false
author_profile: false
title: <br><br><br><br><br>Chao Garden in VR
permalink: /VR-Chao-Garden/
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/egg-carrier-chao-garden-thumbnail.png
feature_row:
  - image_path: /assets/images/outside/vr-brain.jpg
    alt: "Brain and Virtual Reality"
    title: "Brain and Virtual Reality"
    url: "https://www.researchgate.net/profile/Brenda-Wiederhold/publication/332341918_Brain_and_Virtual_Reality_What_Do_they_Have_in_Common_and_How_to_Exploit_their_Potential_Paper_in_Annual_Review_of_Cybertherapy_and_Telemedicine_2018/links/5cae9b51a6fdcc1d498c1157/Brain-and-Virtual-Reality-What-Do-they-Have-in-Common-and-How-to-Exploit-their-Potential-Paper-in-Annual-Review-of-Cybertherapy-and-Telemedicine-2018.pdf?_sg%5B0%5D=started_experiment_milestone&origin=journalDetail&_rtd=e30%3D"
    btn_label: "Paper"
    btn_class: "btn--inverse"
  - image_path: /assets/images/outside/vr-market.jpg
    alt: "Brain and Virtual Reality"
    title: "VR market report"
    url: "https://www.fortunebusinessinsights.com/industry-reports/virtual-reality-market-101378"
    btn_label: "Report"
    btn_class: "btn--inverse"
---
# Een virtuele omgeving in VR

Ik heb tijdens de honours cursus het meeste met VR (Virtual Reality) gedaan, daar was ik altijd wel geintereseerd in maar ik had verder geen contact gehad met de apparatuur. Tijdens de thema avond kregen we een introductie met VR technologie door een presentatie bijeenkomst te houden binnen de Metaverse, daarna hebben we verschillende applicaties met deze technologie uitgeprobeerd. Een goede introductie en ik besloot om verder te gaan met VR technologie. In eerste instantie had ik een demo game project in Unity werkend gekregen op de headset maar uiteindelijk heb ik mijn tijd besteed aan het ontwikkelen van een VR omgeving.

{% include video id="3sOHRzDN4SI" provider="youtube" %}

# Wat is dit?
Wat je ziet is in essentie één grote 3D object met ingebakken textures (plaatjes) en animaties dat uitgevoerd wordt op het VR apparaat (in dit geval de Meta Quest-2). Het leuke aan dit eind resultaat is dat de wereld niet een spel applicatie is, nee het is een environment apk dat herkend wordt door de OS die op de headset draait. Hierdoor zit je niet "vast" in een spel, maar wordt je omgeving in het hoofd menu aangepast. Waardoor je in deze wereld nog steeds toegang hebt tot alle menu opties zoals: je account, instellingen of een andere app.

{% include video id="OunEt3b-hCM" provider="youtube" %}

# Kan ik ook in deze wereld stappen?
Dat kan zeker, ik heb [de apk bestanden op mijn Github account gedeeld](https://github.com/Mark-Shun/VR-Egg-Carrier-Chao-Garden-Home-Environment), dus die zouden gedownload en dan handmatig op een Quest-2 headset geupload kunnen worden.
Daarnaast heb ik op het moment van schrijven een aanvraag voor deze environment op SideQuest (applicatie voor "sideloading" op de Meta headsets) gedaan en is de app momenteel "pre-approved", maar het lijkt nog niet publiekelijk op de store te staan.

# Hoe is deze VR wereld gemaakt?
## 3D wereld
De 3D wereld is bijna volledig met de gratis software Blender gemaakt. Het 3D model van het eiland is uit een bestaand spel gehaald, waarbij het materiaal op de polygons en geometrie opnieuw gemaakt/toegevoegd moesten worden. De animaties van de chao's (kleine blauwe poppetjes) heb ik in Blender gemaakt. Verder was het animeren van het water knap lastig, waarbij ik uiteindelijk ervoor gekozen heb om een doorzichtige plaatje om de 2 frames van positie te verwisselen. Een aardig grote hack (veel standaard methoden werken niet in de benodigde geexporteerde bestandstype) wat uiteindelijk enigzins het gewenste effect geeft.

![Screenshot of Blender project file](/assets/images/blender-chao-garden-screenshot.jpg)

## APK voor de VR headset
Maar met alleen een 3D wereld in Blender zijn we er nog niet. Ik heb een gespecialiseerde tool gebruikt om het 3D bestand (.gltf is benodigd) om te zetten naar een bruikbaar bestand voor de headset. Via de ["Quest Home Environments Converter/Builder" tool](https://github.com/VinceCrusty/Quest-Homes-Environment-Converter/releases) (nieuwste versies beschikbaar op de Discord server) is dit mogelijk, en er is ook nog de optie om dit bestand direct naar de aangesloten VR headset te uploaden (developer rechten op de headset zijn hiervoor waarschijnlijk benodigd). Er zijn verschillende instellingen en limieten binnen het benodigde .gltf bestandstype waar rekening mee gehouden moet worden, maar na heel veel trial & error is het uiteindelijk gelukt.

![Screenshot of the environment converter/builder tool](/assets/images/quest-environment-builder-screenshot.jpg)

# Verdere interessante VR artikelen
<div id='featured'></div>

{% include feature_row %}