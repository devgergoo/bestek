# 📘Bot Dokumentáció <br>
Itt olvashatsz a bot dokumentációiról. Azon belül is az üdvőzlő-távozó rendszerünkről.<br>
## 👋Üdvözlés-Távozás felépítése<br>
A müködése elég egyszerű, ha belép valaki a szerverbe akkor egy megadott csatornába üdvözli az új felhasználót. Ha pedig kilépne valaki, akkor egy megadott csatornába búcsúzik tőle a bot.
Az üdvözlő és távozó rendszerünk jelenleg egy kezdő állapotában van csak. A jelenlegi álláspont szerint csak a csatornákat tudod saját magad konfigurálni, az üzenetet és a képet amit a bot küld, azt még nem.

![image](https://github.com/user-attachments/assets/40fdf542-7bee-4698-b2c1-9b198765e4dc) <br>
![image](https://github.com/user-attachments/assets/7bccd174-1e69-4461-b476-f05e2daf0082) <br>



## 🛠Üdvözló-Távozó Konfigurálása
1- Elsőként a `/welcome <státusz> <csatorna>` illetve a `/bye <státusz> <csatorna>` parancsokat kell kiadnod, ezzel kapcsolod be a rendszert. <br>
2- Ha ez megvan, megy is minden. Kikapcsoláshoz pedig szintén ezeket a parancsokat kell használd, csaka státuszba mást kell írnod.

## 🔔Jogosultságok a parancs futtatásához
  - /welcome ~ **Adminisztrátor** jogosultság szükséges
  - /bye ~ **Adminisztrátor** jogosultság szükséges

## 🤖Bot számára szükséges jogok a szintrendszer müködéséhez
  - (Ajánlott jogosultság az **adminisztrátor**.)
  - Üzenetek küldése a beállított csatornákon

## 📁Tárolt adatok
  - Ha nincs beállítva az üdvözlő-távozó rendszer akkor addig semmit nem tárol.
  - Ha beállítod akkor a szerver ID, az üdvözlő csatorna ID, a távozó csatorna ID tárolásra kerül.
  - **SEMMILYEN** csatlakozó, távozó felhasználói adat nem kerül tárolásra.
