# 📘Bot Dokumentáció <br>
Itt olvashatsz a bot dokumentációiról. Azon belül is a log rendszerünkről.<br>
## 🔭Log felépítése<br>
A naplózási rendszerünk fejlett dizájnnal, és sokoldalú üzenetekkel dobja fel a szervered. A log rendszer webhook alapú. Valamint még kis extra dologgal rendelkezik, hogy 24 óránként csinál egy teljes összegző jelentést. Ebben a jelentésben kiírja a 24 óra elmúlt eseményeit.(tagok csatlakozása, törölt üzenetek, csatorna törlések, csatorna létrehozások,kitiltások, figyelmeztetések, nickváltozások, rangváltozások, üzenet szerkesztések) <br>
<img width="360" height="539" alt="image" src="https://github.com/user-attachments/assets/e82a0189-f690-4045-9bd1-3f3f412d34f4" />
<br>
<img width="472" height="262" alt="image" src="https://github.com/user-attachments/assets/9f4f57f4-e725-4242-9345-e2797c7fd451" />
<br>

## 🛠Log Konfigurálása
1- A log csatornát, a /log parancs segítségével tudod kezelni. Itt tudod beállítani, és kikapcsolni is.

## 🔔Jogosultságok a parancs futtatásához
  - /log ~ **Adminisztrátor** jogosultság szükséges

## 🤖Bot számára szükséges jogok a szintrendszer müködéséhez
  - (Ajánlott jogosultság az **adminisztrátor**.)
  - Vizsgálati napló megtekintése

## 📁Tárolt adatok
  - Ha bekapcsolod a log rendszert akkor a szerver ID, valamint a választott csatorna ID kerül tárolásra.

**Ezek az adatok kérésre bármikor eltávolíthatók.**
Ez ügyben kérlek keress fel engem discordon, vagy pedig hozz létre egy ticketet a support szerveren.
