# 📘Bot Dokumentáció <br>
Itt olvashatsz a bot dokumentációiról. Azon belül is a fehérlistáról(whitelist).<br>
## 📊Fehérlista felépítése<br>
A fehérlista egy olyan funkció amely lezárja a szervered, és senkit nem enged csatlakozni. Ez pl akkor lehet hasznos, ha szerver átalakitáson megy át, stb... 
Természetesen hozzá tudsz adni embereket ehhez a fehérlistáról, így ők képesek lesznek belépni a szerverre, mivel őket nem fogja a bot eltávolítani aszerverről.<br>
![image](https://github.com/user-attachments/assets/988a2330-c585-47c8-b584-75b868a98e00)

## 🛠Fehérlista Konfigurálása
1- A fehérlista konfigurálása elég egyszerű, az első lépéshez be kell írd a `/whitelist be` parancsot. Ezzel bekapcsolod a fehérlistát. Ha pedig kikapcsolni szeretnéd azt a `/whitelist ki` paranccsal tudod megtenni.
2- Ezek után ha valakit hozzá szeretnél adni a fehérlistára, akkor azta `/whitelist add <felhasználó_ID>`* parancs segítségével tudod megtenni. <br>
Ha valakit le szeretnél venni róla, akkor azt pedig a `/whitelist remove <felhasználó_ID>` parancs segítségével tudod<br><br>

## 🔔Jogosultságok a parancs futtatásához
  - /whitelist be ~ **Adminisztrátor** jogosultság szükséges
  - /whitelist ki ~ **Adminisztrátor** jogosultság szükséges
  - /whitelist add ~ **Adminisztrátor** jogosultság szükséges
  - /whitelist remove ~ **Adminisztrátor** jogosultság szükséges

## 🤖Bot számára szükséges jogok a fehérlista müködéséhez
  - (Ajánlott jogosultság az **adminisztrátor**.)
  - Felhasználók kirúgása

## 📁Tárolt adatok
  - Ha nincs beállítva a fehérlista akkor addig semmit nem tárol.
  - Ha konfigurálod a fehérlistát, a szerver ID és a beállított felhasználó ID-ját is elmenti. Ő egyből hozzáadásra kerül a fehérlistához.
  - Ezen kívül minden hozzáadott felhasználó ID mentésre kerül. Ha bárki eltávolításra kerül a fehérlistáról, az az adatbázisból is eltávolístára kerül.
  - Ha a bot eltávolításra kerül a szerverről, de be volt kapcsolva a fehérlista az adatok nem törlődnek.

**Ezek az adatok kérésre bármikor eltávolíthatók.**
Ez ügyben kérlek keress fel engem discordon, vagy pedig hozz létre egy ticketet a support szerveren.
