# Az alkalmazás letöltése

Az alkalmazás legfrissebb verzióját a [download.anytype.io](https://download.anytype.io) oldalról töltheted le.

{% hint style="info" %}
Az Anytype önálló, asztali és mobil eszközökön működő szoftver. Az alkalmazásnak nincs böngészőben futtatható verziója. A böngészőalkalmazásokban számos sebezhetőségi pont van, amelyek veszélyeztetnék elkötelezettségünket az adatbiztonság és a titkosítás iránt.
{% endhint %}

### Rendszerkövetelmények

Az Electron fejlesztési platform használata miatt asztali környezetben a [Chrome rendszerkövetelményei](https://support.google.com/chrome/a/answer/7100626?hl=en) az irányadók.
* PC: Windows 10 vagy újabb
* Mac: macOS Catalina 10.15 vagy újabb
* Linux: 64-bit Ubuntu 18.04 vagy újabb, Debian 10 vagy újabb, openSUSE 15.5 vagy újabb, Fedora Linux 38 vagy újabb
* Android: 8.0 vagy újabb rendszert futtató, 64-bites, legalább 4 GB RAM-mal rendelkező eszköz (ha az alkalmazás a Google Play-ről lett beszerezve)
* iOS: iOS 16 vagy újabb

### Telepítési hely

Az Anytype telepítési könyvtára az egyes operációs rendszerek esetében az alábbi:

* Windows 10 vagy újabb rendszeren, általában:
  `C:\Felhasználók\<felhasználónév>\Appdata\Local\Programs\anytype2\Anytype.exe`
* MacOS: `HDD > Felhasználók > <felhasználónév> > Library > Application Support > anytype`
* Linux: `~/.config/anytype`
* Android: `_device/data/app\_​`, a gyorsítótár mentési helye: `_device/data/data/io.anytype.app_`\
  A könyvárat biztonságos mappában tároljuk, amely a felhasználó által nem hozzáférhető.
* iOS: az alapértelmezett telepítési helyet a rendszer határozza meg

### Tárolási hely módosítása

A széf létrehozásakor lehetőséged van a tárolási hely kiválasztására a meghajtón. A tárolási helyet abban az esetben is megváltoztathatod, ha már rendelkezel széffel az eszközön. Ehhez jelentkezz ki az alkalmazásból, majd a bejelentkezési képernyő jobb felső sarkában lépj a Beállításokra. A széfbe történő belépést követően az adataidat szinkronizáljuk.

<figure><img src="/.gitbook/assets/Custome Storage Location.gif" alt="" width="563"><figcaption></figcaption></figure>

{% hint style="danger" %}
Ügyelj arra, hogy a **Csak helyi** hálózati beállítás használata esetén az adataidat legfeljebb két eszközön tárolhatod a peer-to-peer (P2P) kapcsolat révén.
{% endhint %}

#### Hordozható meghajtók és felhőtárhelyek&#x20;

A széf tárolási helyeként hordozható meghajtót is beállíthatsz. Ehhez csatlakoztasd a meghajtót az eszközödhöz, majd kövesd a lépéseket a [#Tárolási hely módosítása](get-the-app.md#tarolasi-hely-modositasa "mention") pontban. Ne feledd, hogy adataidat csak akkor fogod tudni elérni, ha a meghajtó csatlakoztatva van.

Felhőtárhelyek használatát (pl. Google Drive, iCloud) tárolási helyként nem javasoljuk, mert az eltérő szinkronizálási technológiák használati problémákat eredményezhetnek.
