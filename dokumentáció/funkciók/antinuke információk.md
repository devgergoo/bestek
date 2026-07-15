# 📘Bot Dokumentáció <br>
Itt olvashatsz a bot dokumentációiról. Azon belül is az antinuke rendszerről.<br>
## ⛔Antinuke felépítése<br>
Az antinuke rendszerünk úgy müködik, hogy ha 2 perc alatt 10 új tag csatlakozik a szerveredhez, akkor a szerver egy lezárás alá kerül. Ezt a lezárást manuálisan sehogy sem tudod feloldani. Meg kel lvárd amíg lejár 
a 10 perc és csak az után tudnak csatlakozni a felhasználók. Ez azért jó hogyha esetleges raid lenne a szervered ellen és ez be van kapcsolva, akkor egyszerűen megtudod akadályozni. Ha az antinuke rendszerünk lezárja
a szervert, akkor egyből értesítést is küld privát üzenetben a szerver tulajdonosának.<br>

![image](https://github.com/user-attachments/assets/84b19234-a15b-42d9-8ea4-3ba64daf1116)
![image](https://github.com/user-attachments/assets/3ffe04d5-c7c1-4ea4-b30a-91606d3885f1) <br>
(Mivel még nem történt a sima bottal nuke riasztás, ezért csak a teszt bottal tudok képet csatolni. Ettől függetlenül úgyan így müködik.)

## 🛠Antinuke Konfigurálása
1- Az antnuke a szervervédelem egyik funkciója, a **/serverprotection** parancs menün belül az **"Antinuke"** feliratú funkciónál tudod konfigurálni.

## 🔔Jogosultságok a parancs futtatásához
  - /serverprotection ~ **Adminisztrátor** jogosultság szükséges

## 🤖Bot számára szükséges jogok a szintrendszer müködéséhez
  - (Ajánlott jogosultság az **adminisztrátor**.)
  - Felhasználók kirúgása
  - Az viszont fontos, hogy legyenek engedélyezve a szerver tulajának a privát üzenetek fogadása, hiszen ott fog majd a bot írni.

## 📁Tárolt adatok
  - Ha beállítod, akkor a szerver ID kerül tárolásra.
  - Ezen kívül a csatlakozások száma fog mentésre kerülni, hogy a bot számon tudja követni őket. Minden 2 percenként ezt az adatot törli.

**Ezek az adatok kérésre bármikor eltávolíthatók.**
Ez ügyben kérlek keress fel engem discordon, vagy pedig hozz létre egy ticketet a support szerveren.
