# 📘Bot Dokumentáció <br>
Itt olvashatsz a bot dokumentációiról. Azon belül is a halászatról.<br>
## 🐟Halászat felépítése<br>
A kijelölt csatornában időről időre különféle halak bukkannak fel. Neked csak figyelned kell, és lecsapni rájuk a megfelelő pillanatban. 
Ez egy könnyed, mégis izgalmas kaland, ahol minden fogás számít! A játékban jelenleg 5 ritkasági kategória létezik: Általános, Ritka, Epikus, Legendás, Misztikus. 
Minden ritkaságból különböző haltípusok találhatók, így összesen 13 egyedi hal vár rád a víz alatt. 
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
<img width="900" height="1060" alt="image" src="https://github.com/user-attachments/assets/7c95c0ca-08ee-4271-aea8-428805447145" />


### ❓Hány elfogható hal van?
Jelenleg 13 különböző hal van.
  - 2 Átlagos
      - Ponty
      - Némó
  - 2 Ritka
      - SzemesHal
      - MutánsHal
  - 2 Epikus
      - UwuHal
      - RobotHal
  - 4 Legendás
      - UnikornisHal
      - AlkoholistaHal
      - VámpírHal
      - MacskaHal
  - 3 Misztikus
      - ÖrdögiHal
      - AngyaliHal
      - SzellemHal

### ❓Milyen esélyek vannak a halak megjelenésére? Módosíthatók valahogy?
Az alap esélyek a következőek:
  - Átlagos halak: 50%
  - Ritka halak: 15%
  - Epikus halak: 8%
  - Legendás halak: 2%
  - Misztikus halak: A misztikus halak csak az "Égi" időjárásban jelenhetnek meg, 3% eséllyel.

Ezek az esélyek jelenleg csak az időjárás alatt módosulhatnak:
  - Napos idő --> Semmilyen változás nem történik.
  - Viharos idő --> Az átlagos halak megjelenése 20%-kal csökken, a ritka halaké 20%-kal nő, az epikus halaké 50%-kal nő, a legendás halaké pedig 100%-kal nő.
  - Borult idő --> Az átlagos halak megjelenése nő 10%-kal, a ritka halaké 10%-kal csökken, az epikus halaké 20%-kal csökken, a legendás halaké pedig 30%-kal csökken.
  - Égi idő --> Az összes halak megjelenése csökken 50%-kal, a misztikus halaké pedig 50%-kal nő.

### ❓Lehet cserélni halakat másokkal?
Természetesen! Ezt a /fishtrade paranccsal tudod megtenni. Válaszd ki a felhasználót, és használjátok a feljövő menüt a csere lebonyolítására.

### ❓Milyen lehetőségei vannak a szervernek a halakkal?
Már létrehozhat a szerver vezetősége szerver specifikus boltokat! Itt pl rangokat lehet megadni, és venni őket **BestekCoin**-ból.

BestekCoin: Misztikus/Legendás halak eladásával lehet őket szerezni, valamint a speciális eseményeken. A /fishshop fülön, az eladás menü alatt tudod eladni a halaid. Ha nincs legendás/misztikus ritkaságú halad, akkor se csükkedj! A halaid át tudod alakítani ritkábbá, a fishconvert parancs segítségével.<br>

A profilod a /fishprofile paranccsal tudod megtekinteni, itt kerül megjelenítésre a BestekCoin is. <br>

## 🛠Halászat Konfigurálása
1- A halászatot a `/fishingconfig <csatorna> <intervallum>` parancs segítségével tudod beállítani. Intervallumot percben kell megadni, de elég csak a számot beírni. Ajánlott 2-3 percre állítani a gyors játék érdekében.

## 🔔Jogosultságok a parancs futtatásához
  - /fishingconfig ~ **Adminisztrátor** jogosultság szükséges
  - /fishinginventory ~ nincs szükséges jogosultság
  - /fishingleaderboard ~ nincs szükséges jogosultság
  - /fishtrade ~ nincs szükséges jogosultság


## 🤖Bot számára szükséges jogok a szintrendszer müködéséhez
  - Csatornák megtekintése
  - Üzenetek küldése<br>


## 💎Prémium funkciók
A Bestek bot rendelkezik prémium előfizetéssel. Itt láthatod, hogy erre a funkcióra, milyen extra lehetőségeid vannak, ha előfizetsz.
  - Több BestekCoin és hal speicális eseményeknél - A kereslet nem ismer határokat!
  - /fishpremiumbonus - Extra BestekCoin!
  - A boltban összesen 7 terméket hozhatsz létre - Töltsd fel a szerver boltját!

## 📁Tárolt adatok
  - A szerver ID, a beállított csatorna ID és a megadott intervallum kerül mentésre.
  - Ezenkívül minden hal kifogása mentésre kerül, itt a felhasználó ID és a halak ID-ja kerül mentésre. Ezen kívül még a szintek is mentésre kerülnek.
  - Ha csináltál boltot a szervereden, akkor a szerver ID, és a létrehozott termék kerül mentésre. 


**Ezek az adatok kérésre bármikor eltávolíthatók**
Ez ügyben kérlek keress fel engem discordon, vagy pedig hozz létre egy ticketet a support szerveren.


