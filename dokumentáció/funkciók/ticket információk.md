# 📘Bot Dokumentáció <br>
Itt olvashatsz a bot dokumentációiról. Azon belül is a jegyrendszerről.<br>
## 📊Ticket felépítése<br>
Mint tudjuk a ticket rendszer egy fontos tulajdonság a discord szervereken. Ezért is igyekeztem egy minél jobb, fejlettebb rendszert elhozni. 
A jelenlegi ticket rendszerünk úgy müködik hogy külön kategóriákat állíthatsz be a ticketeknek. Minden ticket kategóriát sajátos módon tudsz konfigurálni: betudod állítani milyen rang férjen hozzá az adott kategóriához,
pingeljen-e valakit(ha igen, milyen rangot). Ez előny lehet sok esetben is, pl partnerkedés kategóriában beállíthatod hogy a partner managerek lássák az abban a kategóriába létrehozott ticketeket, így ők tudják kezelni azt.
A felhasználók szabadon tudnak választani, hogy melyik kategóriában hozzák létre a ticketüket a panelben. Természetesen fontos hogy az adminisztrátorok értesüljenek a ticketekről, és tudják mi folyik bennük. 
Ezért lett kitalálva az archiválás lehetőség is! Szabadon állíthatsz egy olyan csatornát ahova a bot opciónálisan tudja logolni a ticketeket. Ezt egy TXT fájlba fogja megtenni, azonban fontos hogy a ticket bezárása előtt,
meg kell nyomni az Archiválás gombot. Sőt, ha később szeretnél egy ticket kategóriát szerkeszteni azt is simán megtudod csinálni, anélkül hogy törölnöd, majd újra létre kellene hoznod a kategóriát. Ezen kívül 
még azt is be tudod állítani, hogy a bot melyik kategóriába hozza létre a ticket csatornákat.<br><br>

## 🛠Ticket Konfigurálása
1- Elsőnek létre kell hozd a kategóriákat amelyeket szeretnél a ticketben használni, és létre kell hozd a `/addticketcategory <név> <ping> <pingelt_rang> <hozzáférhető_randok> <emoji>` parancs segítségével.<br>
2- Ha ezzel megvagy, létre kell hoznod melyik csatornába szeretnéd elküldeni a ticket panelt, ahol a ticket kategóriákból lehet választani. Ezt a `/setticketmessage <csatorna>` paranccsal tudod megcsinálni. 
Ne aggódj, ha később még adnál hozzá kategóriát, akkor nem kell újra beírd ezt a parancsot, mert a panel frissíti magát egyből.<br>
3- Állítsd be egy log csatornát, amelyet csak a vezetőség lát. Ide fogja majd a bot küldeni az archivált ticket fájlokat. Ezt a `/setticketarchive <csatorna>` paranccsal tudod megcsinálni.<br>
4- A `/listticketcategories` parancs segítségével megnézheted a jelenleg létrehozott ticket kategóriákat, és azoknak a konfigurációját. Ha valamit szerkesztenél rajta, azt könnyen megteheted a `/editticketcategory` parancs segítségével.<br>

## 🔔Jogosultságok a parancs futtatásához
  - /addticketcategory ~ **Adminisztrátor** jogosultság szükséges
  - /setticketmessage ~ **Adminisztrátor** jogosultság szükséges
  - /setticketarchive ~ **Adminisztrátor** jogosultság szükséges
  - /listticketcategories ~ nincs szükséges jogosultság
  - /editticketcategory ~ **Adminisztrátor** jogosultság szükséges

## 🤖Bot számára szükséges jogok a ticket müködéséhez
  - Adminisztrátor
  - Ha a bot nem kap admin jogot, sajnos nem fogja tudni magát hozzáadni a ticket csatornákhoz, és így nem fog müködni az egész.

## 📁Tárolt adatok
  -  Ha nincs beállítva a ticket rendszer akkor addig semmit nem tárol.
  -  Ha konfigurálod a ticket rendszert, akkor eltárolja a szerver ID-t, a csatorna ID-t ahova a ticket panel kerül kiküldésre, az archive csatorna ahova a bot küldi a ticket fájlokat,
  -  **HA** állítottál kategóriát hogy hova kerüljenek a ticket csatornák, akkor a kategória ID is mentésre kerül
  -  Ezeken kívül a ticket létrehozásánál amiket beállítottál azok is mentésre kerülnek, hogy a bot visssza tudja hívni.(Ilyen lehet pl: rang ID, kategória neve, emoji)
  -  Minden kategóriához külön ID kerül mentésre, ez azért van hogy utólag tudjátok szerkeszteni, illetve törölni is.
  -  Illetve szintén mentésre kerül egy szám, amely a létrehozott ticketeket követi.

**Ezek az adatok kérésre bármikor eltávolíthatók.**
Ez ügyben kérlek keress fel engem discordon, vagy pedig hozz létre egy ticketet a support szerveren.
