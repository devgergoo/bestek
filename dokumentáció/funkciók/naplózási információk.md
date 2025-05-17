# 📘Bot Dokumentáció <br>
Itt olvashatsz a bot dokumentációiról. Azon belül is a log rendszerünkről.<br>
## 🔭Log felépítése<br>
A naplózási rendszerünk jelenleg még kissé alap szinten van. Elég sok dolgot naplóz már, de ezt még mindenképp szeretném bővíteni a jövőben. Ezen kívül úgy müködik mint egy átlagos log rendszer.
Annyi extra dologgal rendelkezik, hogy 24 óránként csinál egy teljes összegző jelentést. Ebben a jelentésben kiírja a 24 óra elmúlt eseményeit.(tagok csatlakozása, törölt üzenetek, csatorna törlések, csatorna létrehozások,
kitiltások, figyelmeztetések, nickváltozások, rangváltozások, üzenet szerkesztések)
![image](https://github.com/user-attachments/assets/59702734-b476-48bd-8ba1-9a62b00ab345) <br>
![image](https://github.com/user-attachments/assets/9627a515-5af7-4996-b5b4-f805f2e1bc53)<br>

## 🛠Log Konfigurálása
1- A log csatornát a `/setlog <csatorna>` paranccsal tudod beállítani.<br>
2- A log csatornát a `/disablelog` paranccsal tudod kikapcsolni

## 🔔Jogosultságok a parancs futtatásához
  - /setlog ~ **Adminisztrátor** jogosultság szükséges
  - /disablelog ~ **Adminisztrátor** jogosultság szükséges

## 🤖Bot számára szükséges jogok a szintrendszer müködéséhez
  - (Ajánlott jogosultság az **adminisztrátor**.)
  - Csatornák megtekintése
  - Üzenetek küldése

## 📁Tárolt adatok
  - Ha nincs beállítva a log rendszer akkor addig semmit nem tárol.
  - Ha bekapcsolod a log rendszert akkor a szerver ID kerül tárolásra.

**Ezek az adatok kérésre bármikor eltávolíthatók.**
Ez ügyben kérlek keress fel engem discordon, vagy pedig hozz létre egy ticketet a support szerveren.
