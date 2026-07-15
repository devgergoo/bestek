# 📘Bot Dokumentáció <br>
Itt olvashatsz a bot dokumentációiról. Azon belül is az antikáromkodásról.<br>
## ⛔Antikáromkodás felépítése<br>
Az antikáromkodás rendszerünk fejletten védi a szervered. A legtöbb magyar káromkodást, egyből kitörli és figyelmezteti a felhasználót. Lehet a szó akár a mondat elején, közepén, végén a bot érzékeli azt, és egyből törli. A legtöbb átlagosan használt szimbólumokkal helyettesített káromkodást is képes felismerni, és azt sem hagyja ott a szerveren. Az  antikáromkodás az adminisztrátorok üzeneteit nem szűri, tehát rájuk nem vonatkozik ez a szabály. Ezen kívül az adminisztrátorok bármikor hozzáadhatnak felhasználókat, vagy rangokat a kivételek listára. Akik a kivételen vannak, őket nem fogja figyelmeztetni a bot, és az üzeneteiket sem fogja törölni ha káromkodnak. Valamint elérhető prémium funkció is.<br>

![image](https://github.com/user-attachments/assets/00b08442-4892-4ce3-8571-47c27157b2d5)
<br>

## 🛠Antikáromkodás Konfigurálása
1- Az antikáromkodás a szervervédelem egyik funkciója, a **/serverprotection** parancs menün belül az **"Antikáromkodás"** feliratú funkciónál tudod konfigurálni.


## 🔔Jogosultságok a parancs futtatásához
  - /serverprotection ~ **Adminisztrátor** jogosultság szükséges

## 🤖Bot számára szükséges jogok a szintrendszer müködéséhez
  - (Ajánlott jogosultság az **Adminisztrátor**.)
  - Üzenetek kezelése

## 💎Prémium funkciók
A Bestek bot rendelkezik prémium előfizetéssel. Itt láthatod, hogy erre a funkcióra, milyen extra lehetőségeid vannak, ha előfizetsz.
 - **Lehetőség saját szavak létrehozására** - 
*Van ami sértő számodra? Csak add hozzá, és a bot már szűri azt is. Ilyen egyszerű.*


## 📁Tárolt adatok
  - Ha nincs beállítva az antikáromkodás akkor addig semmit nem tárol.
  - Ha bekapcsolod, akkor a szerver ID kerül tárolásra, illetve maga az hogy be van kapcsolva.
  - Ha kivételeteket adsz hozzá akkor a hozzáadott rang, kategória, csatorna vagy felhasználó ID kerül mentésre. (Attól függ mit adsz hozzá)
  - Ha hozzáadsz prémium funkcióként szót, akkor az a szó, és a szerver ID tárolásra kerül.

**Ezek az adatok kérésre bármikor eltávolíthatók.**
Ez ügyben kérlek keress fel engem discordon, vagy pedig hozz létre egy ticketet a support szerveren.
