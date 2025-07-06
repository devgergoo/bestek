# 📘Bot Dokumentáció <br>
Itt olvashatsz a bot dokumentációiról. Azon belül is a halászatról.<br>
## 🐟Halászat felépítése<br>
A kijelölt csatornában időről időre különféle halak bukkannak fel. Neked csak figyelned kell, és lecsapni rájuk a megfelelő pillanatban. 
Ez egy könnyed, mégis izgalmas kaland, ahol minden fogás számít! A játékban jelenleg 4 ritkasági kategória létezik: Általános, Ritka, Epikus, Legendás. 
Minden ritkaságból 2 különböző haltípus található, így összesen 8 egyedi hal vár rád a víz alatt. 
A játék része egy szintrendszer is: összesen 10 szintet járhatsz be, mindegyikhez különböző feltételek tartoznak. 
Leszel elég kitartó elérni a nehezebb szintekre? Teszteld le magad! Ez nem csak horgászat, ez egy felfedezéssel teli utazás, ahol minden szinttel egyre tapasztaltabb horgásszá válsz! <br><br>
Figyelj a játékban előforduló időjárásokra is... minden időjárás másféle boosterrel lep meg. 🤫 Légy te a legjobb halász, nem csak a szervereden, de egész globálisan!



Szint elérésekhez tartozó kritériumok: 
| Szint | Szükséges halak | Szükséges epikus halak | Szükséges legendás halak |
|:-------:|:--------------:|:-------------:| :-------------: |
|1 - Újonc Halász|10|1| - |
|2 - Újonc Halász II.|40|10| - |
|3 - Újonc Halász III.|100|20| - |
|4 - Haladó halász|200|-| 5 |
|5 - Haladó halász II.|500|-| 10 |
|6 - Haladó halász III.|1000|-|-|
|7 - Profi Halász|1500|-|-|
|8 - Profi Halász II.|2000|-|-|
|9 - Profi Halász III.|5000|-|-|
|10 - Mester Halász|5001|-|-|

<br><br>
Halászathoz tartozó bemutató képek: <br>
![image](https://github.com/user-attachments/assets/67bd78ae-1b15-424c-b5cc-d5634d6624f8)<br>
![image](https://github.com/user-attachments/assets/48ccafab-5a95-4f77-a19f-8d707c7d2850)<br>

### ❓Hány elfogható hal van?
Jelenleg 8 különböző hal van.
  - 2 Átlagos
      - Ponty
      - Némó
  - 2 Ritka
      - SzemesHal
      - MutánsHal
  - 2 Epikus
      - UwuHal
      - RobotHal
  - 2 Epikus
      - UnikornisHal
      - AlkoholistaHal

### ❓Milyen esélyek vannak a halak megjelenésére? Módosíthatók valahogy?
Az alap esélyek a következőek:
  - Átlagos halak: 50%
  - Ritka halak: 15%
  - Epikus halak: 8%
  - Legendás halak: 2%

Ezek az esélyek jelenleg csak az időjárás alatt módosulhatnak:
  - Napos idő --> Semmilyen változás nem történik.
  - Viharos idő --> Az átlagos halak megjelenése 20%-kal csökken, a ritka halaké 20%-kal nő, az epikus halaké 50%-kal nő, a legendás halaké pedig 100%-kal nő.
  - Borult idő --> Az átlagos halak megjelenése nő 10%-kal, a ritka halaké 10%-kal csökken, az epikus halaké 20%-kal csökken, a legendás halaké pedig 30%-kal csökken.



## 🛠Halászat Konfigurálása
1- A halászatot a `/fishingconfig <csatorna> <intervallum>` parancs segítségével tudod beállítani. Intervallumot percben kell megadni, de elég csak a számot beírni. Ajánlott 1 percre állítani a gyors játék érdekében.

## 🔔Jogosultságok a parancs futtatásához
  - /fishingconfig ~ **Adminisztrátor** jogosultság szükséges
  - /fishinginventory ~ nincs szükséges jogosultság
  - /fishingleaderboard ~ nincs szükséges jogosultság
  - /trade ~ nincs szükséges jogosultság


## 🤖Bot számára szükséges jogok a szintrendszer müködéséhez
  - Csatornák megtekintése
  - Üzenetek küldése<br>

## 📁Tárolt adatok
  - A szerver ID, a beállított csatorna ID és a megadott intervallum kerül mentésre.
  - Ezenkívül minden hal kifogása mentésre kerül, itt a felhasználó ID és a halak ID-ja kerül mentésre(illetve nyilván a mennyiségek)


**Ezek az adatok kérésre bármikor eltávolíthatók**
Ez ügyben kérlek keress fel engem discordon, vagy pedig hozz létre egy ticketet a support szerveren.


