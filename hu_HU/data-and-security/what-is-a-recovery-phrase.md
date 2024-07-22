---
description: Az Anytype-ban nincs szükség jelszavakra - kizárólag a kulcsodra
---

# Kulcs

<figure><img src="/.gitbook/assets/Screenshot 2023-08-17 at 18.31.38.png" alt=""><figcaption><p>A kulcsot bármikor elérheted a Beállítások > Széf > Kulcs pontban</p></figcaption></figure>

A széfed létrehozásával egyidőben létrejön a széfhez tartozó, az eszközödön helyben generált, tizenkét véletlenszerű szóból álló kulcs. A kulcs a széfben tárolt, titkosított adatok elérésének egyedüli módja.

A kulcsod egymagában szolgál a felhasználóneved és jelszavad helyettesítésére, mintegy emlékezést segítő módszerként, mesterjelszóval azonosít, hasonlóan a Bitcoin pénztárcákhoz.

A széfedhez rendelt kulcsot nem lehet megváltoztatni, biztonságban tartása pedig kiemelten fontos. A kulcsot bármikor elérheted a 'Beállítások > Széf > Kulcs' pontban.

### Ne felejtsd el elmenteni!

A kulcsod rajtad kívül senki nem ismeri. Biztonsági másolat sem készül róla, így ha elfelejted, az Anytype sem tudja helyreállítani a széfed tartalmát. Éppen ezért kifezetten javasoljuk, hogy hozz létre egy kézzel készült másolatot, vagy jegyezd fel és tárold biztonságos helyen.

A kulcsra minden alkalommal szükséged lesz, amikor a széfedbe új eszközről szeretnél belépni.

### Mi az a kulcs?

A kulcsod egy _seed_phrase_, amely kriptográfiai kulcsként azonosít az Anytype-ban. Egy átlagos kulcs egy előre definiált listán található tizenkét, tizennyolc vagy huszonnégy véletlenszerűen kiválasztott szó egyedi kombinációjából áll.

A hozzád tartozó kulcs a felhasználói fiókod [**egyéni azonosítóját**](https://en.wikipedia.org/wiki/Public-key\_cryptography) származtatja a [**BIP39 algoritmus**](https://medium.com/coinmonks/mnemonic-generation-bip39-simply-explained-e9ac18db9477) segítségével.

### Miért seed phrase-t használunk kulcsként?

A _seed_phrase_ használatának elsődleges célja egy biztonságos és kényelmes módszer biztosítása a széfedben tárolt titkosított információk mentésére és helyreállítására. A _seed_phrase_ használatával a biztonsági kulcsokat abban az esetben is vissza lehet állítani, ha az azonosításra használt eszköz elveszett, ellopják, vagy használhatatlanná válik. A _seed_phrase_ egyfajta főkulcsként működik, amely kinyitja az adatokhoz vezető kaput, így hosszú távú adattárolási és biztonsági megoldásként tekinthetünk rá.

A _seed_phrase_ felépítése szabványosított protokollt követ, amit BIP-39-nek (Bitcoin Improvement Proposal 39-nek) nevezünk. Ez nemcsak átjárhatóságot biztosít a különböző kripto-tárcák és az alkalmazások között, de bevezeti a hibafeltáró ellenőrzőösszeget is, amely segít felismerni a leírási hibákból eredő veszteségeket, minimalizálva ezzel az ember okozta hibák miatti adatvesztési kockázatot.

### Megszerezhetik a kulcsom?

A kulcsod ereje abban rejlik, hogy képes megvédeni digitális tartalmaidat. Ha a kulcs generálása megfelelően megtörtént és felelős kezelése, tárolása biztosított, ahhoz szinte lehetetlen hozzáférni a beleegyezésed vagy a tudtod nélkül. A kulcsokat bonyolult matematikai algoritmusok segítségével hozzuk létre, a lehetséges kombinációk száma emiatt rendkívül nagy, így a támadók számára hatalmas kihívást jelentene nemcsak brute-force módszerekkel megfejteni, de egyáltalán megtalálni azt.

Fontos azonban megérteni, hogy a kulcsod védelmének biztosítása leginkább rajtad áll. Bár használatuk az elmúlt időben egyre inkább természetessé váltak, a digitális tárolási módok sebezhetőséget is hordoznak magukban. Ehelyett javasolt a kulcsot fizikai adathordozón (pl. papíron), írásban rögzíteni és egy csak általad ismert, biztonságos helyen tárolni. Kerüld el a kulcs tárolását internetkapcsolattal rendelkező eszközökön vagy felhőtárhelyeken, mert az hackerek vagy jogosulatlan hozzáféréssel rendelkező személyek áldozatává válhat.

### Kulcs tárolása

Az alábbi megoldásokat a potenciális adatvesztés és a kulcsok elfelejtésének elkerülése érdekében állítottuk fel. Bár a jövőre nézve egyéb lehetőségeket is vizsgálunk, jelenleg az alábbi módokon van lehetőség a kulcsok tárolására és megtekintésére:

#### macOS

Az Anytype a kulcsokat macOS-en alapértelmezetten a Kulcskarika-elérésben tárolja. A kulcsok ezen kívül sehol máshol nem lelhetők fel, még akkor sem, ha a jelszavak iCloud-ra történő automatikus mentése engedélyezve van. Az automatikus biztonsági mentésekről bővebben az [Apple támogatási weboldalán](https://support.apple.com/en-us/HT204085) találsz bővebb információt.

Amennyiben már beléptél a széfbe, a kulcsot az alábbi helyen érheted el:

1. Nyisd meg a Kulcskarika-elérés alkalmazást ('Finder > Alkalmazások > Segédprogramok').
2. A bal oldali oldalsávon válaszd a "bejelentkezési" pontot az "Alapértelmezett kulcskarikák" listában.
3. Válaszd ki az "Anytype" bejegyzést.
4. Kattints a "Jelszó megjelenítése" gombra a kulcsod megtekintéséhez.

#### Windows és Linux

A kulcsodat Windows rendszeren a [Hitelesítőadat-kezelőben](https://support.microsoft.com/en-us/windows/accessing-credential-manager-1b5c916a-6a16-889f-8581-fc16e8165ac0) tároljuk.

Linux-alapú operációs rendszeren a kulcsodat a [seahorse](https://wiki.gnome.org/Apps/Seahorse/) alkalmazással érheted el a [GNOME Keyring](https://wiki.gnome.org/action/show/Projects/GnomeKeyring?action=show\&redirect=GnomeKeyring) használata esetén.
