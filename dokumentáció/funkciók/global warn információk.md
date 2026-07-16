# 📘Bot Dokumentáció <br>
Itt olvashatsz a bot dokumentációiról. Azon belül is a global warn/ban rendszerünkről..<br>
## ⚠Global Warn / Ban felépítése<br>
Ez a rendszer a szerverek védelmének megerősítését szolgálja.
A listára olyan felhasználók kerülnek fel, akik valamilyen módon már megsértették a Discord szabályait (például gyanús vagy csaló linkeket küldtek), de még nem kerültek kitiltásra.
Amennyiben egy ilyen felhasználó belép a szerveretekre, a bot privát üzenetben értesíti a szerver tulajdonosát, vagy kitiltja a felhasználót. (Attól függ, hogy a warn, vagy a ban van bekapcsolva.)

![image](https://github.com/user-attachments/assets/3a4802c3-1295-4713-b467-d2eca970a3fe)<br>
**Az alábbi kép csak illusztráció egy tesztből kivéve. A képen látható felhasználó NEM szerepel a listán, és hozzájárult hogy példaként kikerüljön.**

### ❓Hogy jelezhetem egy felhasználó feltételét a listára?
A support szerveren ticketben tudjátok ezt jelezni. Lett neki egy külön kategória a ticket rendszerünkben, de akár a segítségkérésben is létrehozhatjátok!<br>
[Support szerver](https://discord.gg/Zjn6vfZUHf)

### ❓Mi kell ahhoz hogy valaki felkerüljön a listára?
Nagyon fontos hogy értékálló bizonyítékkal kell rendelkezzetek arról, hogy az általatok bejelentett felhasználó káros tevékenységeket hajtott végre. 
Ezenkívül szükséges információk: Felhasználói ID-név, szerver(ID-név) /privát üzenet, üzenet ID(egyes esetekben)

### ❓Ha felkerültem a listára, de valami félreértésből adódóan, mi a teendő?
Ez esetben kérlek lépj be a fellebbezési szerverre. Fontos, hogy a csatlakozásnál megfogja kérdezni miért szeretnél belépni, ide normális indokot irjatok. Nem odaillő indokkal való belépést elfogunk utasítani.
A support szerver és a fellebezési szerver nem egyenlő egymással. A szerveren kérlek ticket formájában pontosan fogalmazd meg, mi volt az indok amivel felkerültél, és milyen félreértés történt.
Az olyan indokok hogy "nem gondoltam komolyan", úgy hogy írt egy 10 soros átkozást valakire, azért az nem fog müködni... A fellebbezési szerverre csak olyan felhazsnálk léphetnek be, akik szerepelnek a listán.
Mások csatlakozása egyből elutasításra kerül.<br>
[Fellebbezési szerver](https://discord.gg/BUQv3EvsUN)

### ❓Egyéb kérdés?
[Support szerver](https://discord.gg/Zjn6vfZUHf) / [Fellebbezési szerver](https://discord.gg/BUQv3EvsUN)

## 🛠Global Warn Konfigurálása
1- Ha behívod a botot, a rendszer automatikusan bekapcsolódik. <br>
2- Ezen kívül az állapotát a `/globalsettings` tudod állítani. <br>

## 🔔Jogosultságok a parancs futtatásához
  - /globalsettings ~ **Adminisztrátor** jogosultság szükséges
  - /globalwarncheck ~ nincs szükséges jogosultság

## 🤖Bot számára szükséges jogok a global warn müködéséhez
  - Felhasználók kitiltása.
  - Fontos! A szerver tulaja fogadjon privátba üzeneteket.

## 📁Tárolt adatok
  - A szerver ID kerül csak mentésre.
  - A listán lévő felhasználók számára az alábbi adatok kerülnek mentésre: felhasználó ID, dátum, indok, bizonyítékok.

**Ezek az adatok kérésre bármikor eltávolíthatók.**
Ez ügyben kérlek keress fel engem discordon, vagy pedig hozz létre egy ticketet a support szerveren.
