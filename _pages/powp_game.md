---
layout: single
read_time: false
comments: false
share: false
author_profile: false
title: <br><br><br><br><br>Interactieve Kunst Powerpoint Quiz
permalink: /kunst-powerpoint-quiz/
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/rococo-stroming.jpg
feature_row:
  - image_path: /assets/images/outside/gamification-class.jpg
    alt: "The Gamification of Learning"
    title: "The Gamification of Learning"
    url: "https://link.springer.com/content/pdf/10.1007/s10648-019-09498-w.pdf"
    btn_label: "Paper"
    btn_class: "btn--inverse"
  - image_path: /assets/images/outside/game-gamification.jpg
    alt: "Gamification revolutionizing learning to code"
    title: "Gamification revolutionizing learning to code"
    url: "https://medium.com/@victor5.vm58/breaking-the-code-how-gamification-is-revolutionizing-learning-in-programming-0268671f5221"
    btn_label: "Artikel"
    btn_class: "btn--inverse"
---

# Spelend leren
TIjdens de thema avond over gamification werden we geintroduceerd over verschillende producten en projecten dat binnen het onderwerp Gamification vallen. Gamification wordt benut om de aandacht en motivatie van de deelnemers of gebruikers te verbeteren (bijvoorbeeld door de introductie van: dynamische- en spel elementen). Één van de voorbeelden die getoond werd door de gast spreker was een spel verwerkt in Powerpoint om de geschiedenis van China te leren, waarbij je als adviseur van de keizer keuzes maakt die gevolgen hebben op het land en de relatie tussen jou en de keizer. Dit vond ik een zeer leuke implementatie binnen powerpoint, dus na een korte introductie tijdens de avond had ik besloten om zelf thuis ook een interactieve powerpoint te maken. Omdat ik naar mijn idee een visueel persoon ben, leek het me leuk om kunstgeschiedenis in de powerpoint te verwerken en hiervan een quiz te maken.

![Quiz vraag over een schilderij stroming](/assets/images/schilderij-stroming.jpg)

# Kan ik mijn kunst kennis beproeven?
Dat kan, zo ver ik weet is het niet mogelijk om een powerpoint met macro's online te laten draaien. En dus is het nodig om de powerpoint lokaal te downloaden, te openen, en macro's er binnen toe te staan (waarschijnlijk verschijnt er een pop up). Indien de wens ervoor is, is het volgens mij mogelijk om de macro code te inspecteren voordat je het draait, om te controleren of er niks geks in staat.
[Download het Powerpoint bestand](/assets/powerpoint/Kunst%20Quiz%20-%20Een%20Interactive%20Powerpoint.pptm)

# Hoe is het gemaakt
Dit is dus gemaakt in Microsoft Powerpoint, zoals mij al verteld was is er een mogelijkheid om "acties" toe te voegen aan knoppen/figuren, waarbij je bij het drukken op de knop wordt doorgeleidt naar een specifieke dia. Er was echter één probleem: ik wou ook een score bijhouden (een zeer belangrijk game element) en aan de hand van de eind score de gebruiker een specifieke eind scherm laten zien. Hiervoor moest ik iets verder kijken.

## Gebruik van macro's
Om tot mijn doel te komen heb ik uiteindelijk gebruik gemaakt van macro's binnen het powerpoint project.
Ik wist dat macro's bestonden maar niet precies hoe ze werken. Want door mogelijke veiligheids waarschuwingen wordt in het algemeen geadviseerd om macro's uit te schakelen (macro's kunnen namelijk gebruikt worden door kwaadaardige coders om malware of een trojan te introduceren). Om deze reden worden macro's standaard geblokkeerd als het bestand van het internet komt. Hierdoor zie ik macro's eigenlijk weinig in gebruik.

Des al te min wou ik leren om macro's te gebruiken voor mijn doeleinden: het maken van een interactieve powerpoint quiz presentatie dat een score bijhoudt.
Hiervoor heb ik de programeertaal VBA gebruikt om functies te schrijven en deze te koppelen aan elementen in de presentatie. Door het drukken op knoppen wordt de code uitgevoerd dat bijvoorbeeld de gebruiker veplaatst naar een andere dia, een antwoord controleerd, en de score updatet.

![Afbeelding van macro code](/assets/images/functie-code.jpg)

## Gebruik van activeX
Een andere functionaliteit die ik nodig had voor het maken van dit project zijn activeX elementen. Met het gebruik van activeX elementen was het mogelijk om invoer balkjes toe te voegen in de powerpoint waarmee met VBA de inhoud gecontroleerd kon worden, aan de hand van het antwoord kunnen dan punten wel of niet gegeven worden.

![ActiveX element](/assets/images/activex.jpg)

# Verdere interessante artikelen over gamification
<div id='featured'></div>

{% include feature_row %}