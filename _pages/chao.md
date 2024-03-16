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
---
# Een virtuele omgeving in VR

Ik heb tijdens de honours cursus het meeste met VR (Virtual Reality) gedaan, daar was ik altijd wel geintereseerd in maar ik had verder geen contact gehad met de apparatuur. Tijdens de thema avond kregen we een introductie met VR technologie door een meeting te houden met binnen Metaverse, en daarna hebben we nog verschillende informatie gekregen en applicaties uitgeprobeerd. Na de introductie besloot ik om verder te gaan met VR technologie, waarbij ik een korte Unity demo werkend heb gekregen op het apparaat, maar vooral veel heb gewerkt aan deze "environment" applicatie.

{% include video id="3sOHRzDN4SI" provider="youtube" %}

# Wat is dit?
Dit is in essentie één grote 3D object met ingebakken textures (plaatjes) en animaties dat uitgevoerd wordt op het VR apparaat (in dit geval de Meta Quest-2). Het leuke aan dit eind resultaat is dat de wereld niet een spel applicatie is, nee het is een environment apk dat herkend wordt door de OS die op de headset draait. Hierdoor zit je niet "vast" in een spel, maar wordt je omgeving in het hoofd menu aangepast. Waardoor je in deze wereld nog steeds toegang hebt tot alle menu opties zoals: je account, instellingen of een andere app.

{% include video id="OunEt3b-hCM" provider="youtube" %}

# Kan ik deze wereld uit proberen?
Dat kan zeker, ik heb [de apk bestanden op mijn Github account gedeeld](https://github.com/Mark-Shun/VR-Egg-Carrier-Chao-Garden-Home-Environment), dus die zouden gedownload en dan handmatig op een Quest-2 headset geupload kunnen worden.
Daarnaast op het moment van schrijven heb ik een aanvraag voor deze environment op SideQuest (applicatie voor "sideloading" op de Meta headsets) nog open staan.

# Hoe is deze VR wereld gemaakt?
## 3D wereld
De 3D wereld is bijna volledig met de gratis software Blender gemaakt. Het 3D model van het eiland is uit een bestaand spel gehaald, waarbij het materiaal op de polygons en geometrie opnieuw gemaakt/toegevoegd moest worden. De animaties van de chao's (kleine blauwe poppetjes) heb ik in Blender gemaakt. Verder was het animeren van het water knap lastig, waarbij ik uiteindelijk ervoor gekozen heb om een doorzichtige plaatje om de 2 frames van positie te verwisselen. Een aardig grote hack (veel standaard methoden werken niet in de benodigde geexporteerde bestandstype) wat aardig werkt.

![Screenshot of Blender project file](/assets/images/blender-chao-garden-screenshot.jpg)

## APK voor de VR headset
Maar met een 3D wereld in Blender zijn we er nog niet. Ik heb een gespecialiseerde tool gebruikt om het 3D bestand (.gltf is benodigd) om te zetten naar een bruikbaar bestand voor de headset. Via de ["Quest Home Environments Converter/Builder" tool](https://github.com/VinceCrusty/Quest-Homes-Environment-Converter/releases) (nieuwste versies beschikbaar op de Discord server) is dit mogelijk, en het is ook nog eens mogelijk om dit bestand direct naar de aangesloten VR headset te uploaden (developer rechten zijn hiervoor waarschijnlijk benodigd). Er zijn verschillende opties en limieten binnen het benodigde .gltf bestandstype waar rekening mee gehouden moet worden, maar na heel veel trial & error is het uiteindelijk gelukt.

![Screenshot of the environment converter/builder tool](/assets/images/quest-environment-builder-screenshot.jpg)