---
lang: it-IT
layout: wiki
section: twilightmenu
category: other
title: Giocare in Widescreen
description: Come usare TWiLight Menu++ in widescreen su Nintendo 3DS
---

Questa sezione richiede una console della famiglia 3DS con un moderno CFW installato da [3ds.hacks.guide](https://3ds.hacks.guide).
{:.alert .alert-info}

If you're currently using Luma v13, please update to v13.0.1, before following this guide.
{:.alert .alert-info}

### Installazione
1. Apri FBI e seleziona `Remote Install`, poi `Scan QR Code`
1. Scannerizza questo QR code per installare l'ultima versione di [Universal-Updater](https://github.com/Universal-Team/Universal-Updater)<br> ![QR code Universal-Updater](https://db.universal-team.net/assets/images/qr/universal-updater-cia.png)
1. Apri Universal Updater dal tuo menu HOME
1. Installa il pacchetto TWPatch
    - Se la tua console non può collegarsi ad internet, puoi scaricare [TWPatch.cia](https://gbatemp.net/download/twpatch.37400/version/38832/download?file=302085) direttamente, e poi installarlo con FBI
1. Return to the HOME menu and launch TWPatch
    - If you get a message which says `Can't open /luma/exeTWL.bin`, then use [TWLFix-CFW](https://github.com/MechanicalDragon0687/TWLFix-CFW/releases/) to fix broken TWL mode
1. Tieni premuto <kbd class="face">Y</kbd> + <kbd class="face">B</kbd> per aprire il patch menu e abilita `Widescreen patch (384x240 16:10)`
1. (Opzionale!) Per un widescreen meno pixellato, abilita anche `GPU scaling (blurry, no filters)`
1. Premi <kbd class="face">B</kbd> per uscire dal patch menu
1. Premi <kbd>START</kbd> per generare un `TwlBg.cxi`file con widescreen
    - Se lo schermo superiore non indica che la wide patch è abilitata, riprova il passaggio 3
1. Muovi `TwlBg.cxi` da `sd:/luma/sysmodules/` a `sd:/_nds/TWiLightMenu/TwlBg/` (se non è gia presente, crea la cartella `TwlBg`), e rinomina il file in `Widescreen.cxi`
1. Riavvia il tuo 3ds tenendo premuto <kbd>SELECT</kbd> per aprire il menu di Luma3DS's
1. Abilita `external FIRMs and modules`, e premi <kbd>START</kbd> per salvare e uscire
1. Apri TWiLight Menu++, premi <kbd class="face">Y</kbd> su un gioco a tua scelta per aprire le impostazioni del gioco selezionato, e imposta `Proporzioni schermo` a `16:10`

Hai finito! Goditi i tuoi giochi del DS in widescreen!

**NOTE:**
1. Non tenere premuto <kbd>START</kbd> o <kbd>SELECT</kbd> quando avvii TWLMenu++, se non vuoi avvere problemi con il widescreen
1. Non tutti i giochi sono compatibili con il 16:10. [Questa è una lista con tutti i giochi supportati](https://github.com/DS-Homebrew/TWiLightMenu/blob/master/7zfile/3DS%20-%20CFW%20users/Games%20supported%20with%20widescreen.txt)
1. If you're stuck in widescreen mode in all of TWL_FIRM (including the TWLMenu++ GUI) after following this guide and launching a widescreen-compatible game, delete `TwlBg.cxi` at `sd:/luma/sysmodules/`.
    - If the problem persists, [uninstall](https://wiki.ds-homebrew.com/twilightmenu/uninstalling-3ds) and [re-install](https://wiki.ds-homebrew.com/twilightmenu/installing-3ds) TWiLight Menu++, and re-follow the above guide, as well as using the original build of Luma
1. La maggior parte delle patches regoleranno solamente gli elementi 3D, gli elementi 2D (come i menu) saranno solo allungati
1. Luma3DS **deve** essere caricato dalla scheda SD, se il widescreen non funziona assicurati di avere il file  `boot.firm` nella root della tua scheda SD
