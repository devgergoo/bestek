# 📘Bot Dokumentáció <br>
Itt olvashatsz a bot dokumentációiról. Azon belül is az antikáromkodásról.<br>
## ⛔Antikáromkodás felépítése<br>
Az antikáromkodás rendszerünk fejletten védi a szervered. A legtöbb magyar káromkodást, egyből kitörli és figyelmezteti a felhasználót. Lehet a szó akár a mondat elején, közepén, végén a bot érzékeli azt, és egyből törli. A legtöbb átlagosan használt szimbólumokkal helyettesített káromkodást is képes felismerni, és azt sem hagyja ott a szerveren. Az  antikáromkodás az adminisztrátorok üzeneteit nem szűri, tehát rájuk nem vonatkozik ez a szabály. Ezen kívül az adminisztrátorok bármikor hozzáadhatnak felhasználókat, vagy rangokat a kivételek listára. Akik a kivételen vannak, őket nem fogja figyelmeztetni a bot, és az üzeneteiket sem fogja törölni ha káromkodnak.<br>

![image](https://github.com/user-attachments/assets/00b08442-4892-4ce3-8571-47c27157b2d5)
<br>

## 🛠Antikáromkodás Konfigurálása
1- Elsőnek is a `/antikáromkodás <Bekapcsol/Letilt>` parancs segítségével tudod kezelni hogy ki/be legyen kapcsolva a rendszer.
2- Ezek után ha szeretnél kivételt hozzáadni, azt a /antikáromkodáskivétel `<Hozzáadás/Eltávolítás>` parancs segítségével tudod. Itt ki kell válaszd, hogy embert vagy rangot szeretnél hozzáadni.
3- Megnézni a kivételek listáját pedig a `/antikáromkodáskivételek` paranccsal tudod.

## 🔔Jogosultságok a parancs futtatásához
  - /antikáromkodás ~ **Adminisztrátor** jogosultság szükséges
  - /antikáromkodáskivétel ~ **Adminisztrátor** jogosultság szükséges
  - /antikáromkodáskivételek ~ **Adminisztrátor** jogosultság szükséges

## 🤖Bot számára szükséges jogok a szintrendszer müködéséhez
  - (Ajánlott jogosultság az **adminisztrátor**.)
  - Üzenetek kezelése

## 📁Tárolt adatok
  - Ha nincs beállítva az antikáromkodás akkor addig semmit nem tárol.
  - Ha bekapcsolod, akkor a szerver ID kerül tárolásra, illetve maga az hogy be van kapcsolva.
  - Ha kivételeteket adsz hozzá akkor a hozzáadott rang ID kerül eltárolásra, vagy a hozzáadott felhasználó ID (Attól függ mit adsz hozzá)

**Ezek az adatok kérésre bármikor eltávolíthatók.**
Ez ügyben kérlek keress fel engem discordon, vagy pedig hozz létre egy ticketet a support szerveren.
