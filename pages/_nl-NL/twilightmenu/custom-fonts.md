---
lang: nl-NL
layout: wiki
section: twilightmenu
category: customization
title: Aangepaste Lettertypen
description: Hoe gebruik je aangepaste lettertypen met TWiLight Menu++
---

TWiLight Menu++ kan aangepaste lettertypes in NFTR-formaat (Nitro FonT Resource) gebruiken. Ze zullen worden gebruikt in Instellingen, de titels van de Handleiding, en in de Nintendo DSi, Nintendo 3DS, SEGA Saturn, en Homebrew Launcher thema's.

### Mapstructuur
Aangepaste lettertypen worden geladen van `sd:/_nds/TWiLightMenu/extras/fonts/[lettertypenaam]/[lettertypebestand].nftr` waar `[lettertypenaam]` de gewenste naam is en `[lettertypebestand].nftr` een van de volgende is:
- `large.nftr`: The larger font used for titles
- `small.nftr`: The smaller font used for most other text

### Skin-lettertypen
Je kunt lettertypen toevoegen aan [aangepaste DSi-/3DS-themaskins](custom-dsi-3ds-skins), die zullen overschrijven wat is ingesteld in TWiLight Menu++-instellingen. Deze lettertypen gaan in de map `font`, in de hoofdmap van de skin.

Aangepaste skins kunnen bovendien overschrijflettertypen gebruiken voor de datum en tijd met `date_time.nftr`, en de console gebruikersnaam met `username.nftr`.

### Aangepaste lettertypes genereren
Je kunt je eigen lettertypen maken met behulp van een hulpbron zoals [nftr-editor](https://pk11.us/nftr-editor/) van Pk11. Om één van de bestaande lettertypen van TWiLight Menu++ te regenereren:
1. Laad een NFTR-bestand in nftr-editor
1. Typ de namen van de lettertypen die je wilt gebruiken van de hoogste naar de laagste prioriteit in het tekstvak `Input font`, komma gescheiden
    - Je kunt een voorbeeld zien van de invoerlettertypen in het bovenste vak links en de huidige NFTR in het onderste vak
1. Klik op `Generate from font`, en `OK` om bestaande tekens te regenereren en `Cancel` om de speciale knoptekens te regenereren (bijv. &#xE000;)
1. Klik op `Save`, en herhaal dit voor de andere maten
