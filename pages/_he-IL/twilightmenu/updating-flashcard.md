---
lang: he-IL
layout: wiki
section: twilightmenu
category: updating
title: עדכון (פלאשקארט)
long_title: עדכון TWiLight Menu++ (פלאשקארד)
description: איך לעדכן את TWiLight Menu++ על פלאשקארד של Nintendo DS
---

If updating from a version older than v16.4.0, please move your `.sav` files for DS games to a new folder called `saves`, with the `saves` folder being in the same place as the DS ROMs.
{:.alert .alert-info}

If updating from a version older than v21.0.0, please move your `.pub` and/or `.prv` files for DSiWare titles to a new folder called `saves`, with the `saves` folder being in the same place as the DSiWare ROMs.
{:.alert .alert-info}

### עדכון
1. הורידו את הגרסה האחרונה של [`TWiLightMenu-Flashcard.7z`](https://github.com/DS-Homebrew/TWiLightMenu/releases/latest/download/TWiLightMenu-Flashcard.7z)
    - If it does not download, see the [release page](https://github.com/DS-Homebrew/TWiLightMenu/releases/latest)
1. חלצו את `TWiLightMenu-Flashcard.7z`
1. Copy the `_nds` folder to your flashcard's microSD card root, replacing any existing files
    - If using macOS, make sure to **copy** and `Merge`, don't `Replace`
1. Copy the `BOOT.NDS` file to your flashcard's microSD card root, replacing any existing files
1. If TWLMenu++ does not boot after updating, then update the autoboot file(s) as well

### שלבים נוספים עבור הSD של DSi/3DS

אם אתם יכולים להחליף את הקבצים שעל הSD של המכשיר ובין הקבצים על הפלאשקארד באמצעות TWLMenu++, וגם גרסאת TWLMenu++ על הפלאשקארד היא v16.3.0 או גבוהה יותר, עקבו אחרי השלבים האלו.

1. לכו להגדרות של TWLMenu++
1. בחרו ב`Update TWiLight Menu++`
1. בחרו `Slot-1 microSD > Console (micro)SD`
