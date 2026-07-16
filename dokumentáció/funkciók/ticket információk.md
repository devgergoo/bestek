# 📘Bot Dokumentáció <br>
Itt olvashatsz a bot dokumentációiról. Azon belül is a jegyrendszerről.<br>
## 🎫Ticket felépítése<br>
Mint tudjuk a ticket rendszer egy fontos tulajdonság a discord szervereken. Ezért is igyekeztem egy minél jobb, fejlettebb rendszert elhozni. 
A jelenlegi ticket rendszerünk úgy müködik hogy külön kategóriákat állíthatsz be a ticketeknek. Minden ticket kategóriát sajátos módon tudsz konfigurálni: betudod állítani milyen rang férjen hozzá az adott kategóriához,
pingeljen-e valakit(ha igen, milyen rangot). Ez előny lehet sok esetben is, pl partnerkedés kategóriában beállíthatod hogy a partner managerek lássák az abban a kategóriába létrehozott ticketeket, így ők tudják kezelni azt.
A felhasználók szabadon tudnak választani, hogy melyik kategóriában hozzák létre a ticketüket a panelben. Természetesen fontos hogy az adminisztrátorok értesüljenek a ticketekről, és tudják mi folyik bennük. 
Ezért lett kitalálva az archiválás lehetőség is! Szabadon állíthatsz egy olyan csatornát ahova a bot opciónálisan tudja logolni a ticketeket. Ezt egy TXT fájlba fogja megtenni, azonban fontos hogy a ticket bezárása előtt,
meg kell nyomni az Archiválás gombot. Sőt, ha később szeretnél egy ticket kategóriát szerkeszteni azt is simán megtudod csinálni, anélkül hogy törölnöd, majd újra létre kellene hoznod a kategóriát. Ezen kívül 
még azt is be tudod állítani, hogy a bot melyik kategóriába hozza létre a ticket csatornákat.<br><br>
![image](https://github.com/user-attachments/assets/019b0343-b5c6-4ea7-83ba-6c9dde53328e)
<img width="672" height="787" alt="image" src="https://github.com/user-attachments/assets/3f7e9699-0003-47bb-985d-bb89bd0a6e8b" />

<br>

## 🛠Ticket Konfigurálása
1- Elsőnek létre kell hozd a kategóriákat amelyeket szeretnél a ticketben használni, ezt a `/addticketcategory` parancs segítségével tudod megtenni. Itt ki kell töltened a feljövő V2-es menüt.<br>
2- Ha ezzel megvagy, akkor a ticket további beállításait a /ticketconfigpanel parancs segítségével tudod megtekinteni. Itt betudod állítani a következőket: Melyik csatornába küldje a ticket panelt. Melyik discord kategóriába hozza létre a bot a ticketeket. Melyik legyen a ticket log csatorna. Melyik legyen a ticket archive csatorna. Törölje-e automatikusan a ticketeket, ha kilép a felhasználó. Másik szerverről való ticketek átmásolása.
4- A `/listticketcategories` parancs segítségével megnézheted a jelenleg létrehozott ticket kategóriákat, és azoknak a konfigurációját. Itt tudod törölni is őket. Ha valamit szerkesztenél rajta, azt könnyen megteheted a `/editticketcategory` parancs segítségével.<br>

## 🔔Jogosultságok a parancs futtatásához
  - /addticketcategory ~ **Adminisztrátor** jogosultság szükséges
  - /ticketconfigpanel ~ **Adminisztrátor** jogosultság szükséges
  - /listticketcategories ~ **Adminisztrátor** jogosultság szüksége
  - /editticketcategory ~ **Adminisztrátor** jogosultság szükséges

## 🤖Bot számára szükséges jogok a ticket müködéséhez
  - Adminisztrátor!
  - Ha a bot nem kap admin jogot, sajnos nem fogja tudni magát hozzáadni a ticket csatornákhoz, és így nem fog müködni az egész.

## 📁Tárolt adatok
  -  Ha konfigurálod a ticket rendszert, akkor eltárolja a szerver ID-t, a csatorna ID-t ahova a ticket panel kerül kiküldésre, az archive csatorna ahova a bot küldi a ticket fájlokat, és a log csatorna ID.
  -  Ha állítottál kategóriát hogy hova kerüljenek a ticket csatornák, akkor a kategória ID is mentésre kerül.
  -  Ezeken kívül a ticket létrehozásánál amiket beállítottál azok is mentésre kerülnek, hogy a bot visssza tudja hívni.(Ilyen lehet pl: rang ID, kategória neve, emoji)
  -  Minden kategóriához külön ID kerül mentésre, ez azért van hogy utólag tudjátok szerkeszteni, illetve törölni is.
  -  Illetve szintén mentésre kerül egy szám, amely a létrehozott ticketeket követi.

**Ezek az adatok kérésre bármikor eltávolíthatók.**
Ez ügyben kérlek keress fel engem discordon, vagy pedig hozz létre egy ticketet a support szerveren.
