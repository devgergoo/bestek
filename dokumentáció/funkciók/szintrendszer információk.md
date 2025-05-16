# 📘Bot Dokumentáció <br>
Itt olvashatsz a bot dokumentációiról. Azon belül is a szintrendszerről.<br>
## 📊Szintrendszer felépítése<br>
A szintrendszer úgy möködik hogy minden 30 másodpercenként elköldött üzenet után random 5 és 11 közötti xp jár. Minden szinthez 100-al több xp kell. Tehát az első szinthez 100 xp, a második szinthez 200 xp, stb szükséges.
Minden szintlépésnél elveszted az addig gyüjtött xp-t. Tehát ha szintet lépsz, és pl 2. szintű leszel, akkor ismételten 0 xp-ről indulsz.<br><br>
Szintek társuló xp szükségletek<br>
| Szint | Szükséges XP | Kiinduló XP |
|:-------:|:--------------:|:-------------:|
| 1     | 100          | 0           |
| 2     | 200          | 0           |
| 3     | 300          | 0           |
| 4     | 400          | 0           |
| 5     | 500          | 0           |
| 6     | 600          | 0           |
| 7     | 700          | 0           |
| 8     | 800          | 0           |
| 9     | 900          | 0           |
| 10    | 1000         | 0           |
| 11    | 1100         | 0           |
| 12    | 1200         | 0           |
| 13    | 1300         | 0           |
| 14    | 1400         | 0           |
| 15    | 1500         | 0           |
| 16    | 1600         | 0           |
| 17    | 1700         | 0           |
| 18    | 1800         | 0           |
| 19    | 1900         | 0           |
| 20    | 2000         | 0           |
| 21    | 2100         | 0           |
| 22    | 2200         | 0           |
| 23    | 2300         | 0           |
| 24    | 2400         | 0           |
| 25    | 2500         | 0           |
| 26    | 2600         | 0           |
| 27    | 2700         | 0           |
| 28    | 2800         | 0           |
| 29    | 2900         | 0           |
| 30    | 3000         | 0           |
| 100    | 10000         | 0           |
| 1000    | 100000         | 0           |

A szinteknél nincs maximum szint megadva, és ezt a rendet követi az összes szint.<br><br>
## 🛠Szintrendszer Konfigurálása
1- A szintrendszer alapértelmezetten ki van kapcsolva, ezért manuálisan be kell kapcsold a `/toggleleveling` parancs segítségével!<br>
2- Ezek után fontos, hogy állítsd egy csatornát, ahová a bot kiírhatja a szintlépéseket. Ezt a `/setlevelingchannel <csatorna>` parancs segítségével tudod megtenni. Ha szeretnél opcióonálisan állíthatsz saját szintlépő üzenetet, a `/setlevelingmessage <üzenet>` parancs segítségével. Az alapértelmezett szintlépő szöveg: `🎉 <@felhasználó> elérte a <szint>. szintet!`.<br>
3- Ha szeretnél opciónálisan állíthatsz szintekhez tartozó rangokat is. Ha egy felhasználó elér egy szintet, és be van állítva, akkor egyből egy ranggal jutalmazza. Ezt a `/setlevelrole <szint> <rang>` paranccsal állíthatod be. Ha meg szeretnéd nézni hogy milyen szintekhez milyen rangot adtál, egyszerűen megtudod a `/checklevelroles` parancs segítségével. Ezek után, ha megállapítottad hogy törölni szeretnél egy szinthez tartozó rangot, csak be kell írnod a `/removelevelrole <szint>` parancsot. Ez kitörli az adott szinthez tartozó rangot, és több felhasználó már nem kapja meg. Magát a rangot persze nem törli a szerverről. Ha valaki elér egy szintet amelyhez rang van állítva akkor a bot privát üzenetben is értesíti a felhasználót, hogy biztosan megkapta a rangot. Ez így néz ki: `Gratulálunk, elérted a <szint>. szintet és megkaptad a <rang> rangot!`. Jelenleg ez az üzenet nem konfigurálható.<br>
4- Ha szeretnél opciónálisan állíthatsz olyan rangokat amelyek bónusz xp-t kapnak. Ehhez egy szorzót kell beállítanod. Alapból mindenki 1x szorzón kapja az xp-t. Használd a `/setboostrole >rang> <szorzó>` parancsot. A szorzóhoz elég csak a számot írnod. Pl: 2, vagy 3, vagy akár 2.5. Logikusan ez úgy működik, hogy a kapott xp, az beszorzódik az állított szorzóval, így azt az értéket kapják meg a ranggal rendelkező felhasználók.Pl: ha kapsz 6xp-t de 2-es szorzó van, akkor 12xp-t fogsz kapni.Ezeket a rangokat a `/listboostroles` parancs segítségével tekintheted meg. Ha pedig el szeretnéd távolítani a ranghoz tartozó bónusz szorzót azt a `/removeboostrole <rang>` paranccsal tudod.<br><br>
## 🔔Jogosultságok a parancs futtatásához
  - /toggleleveling ~ **Adminisztrátor** jogosultság szükséges
  - /setlevelingchannel ~ **Adminisztrátor** jogosultság szükséges
  - /setlevelingmessage ~ **Adminisztrátor** jogosultság szükséges
  - /setlevelrole ~ **Adminisztrátor** jogosultság szükséges
  - /checklevelroles ~ nincs szükséges jogosultság
  - /removelevelrole ~ **Adminisztrátor** jogosultság szükséges
  - /setboostrole ~ **Adminisztrátor** jogosultság szükséges
  - /listboostroles ~ nincs szükséges jogosultság
  - /removeboostrole ~ **Adminisztrátor** jogosultság szükséges
  - /rank ~ nincs szükséges jogosultság
  - /levelleaderboard ~ nincs szükséges jogosultság<br>

## 🤖Bot számára szükséges jogok a szintrendszer müködéséhez
  - (Ajánlott jogosultság az **adminisztrátor**.)
  - Csatornák megtekintése
  - Üzenetek küldése<br>
(Ettől független a privát csatornákhoz külön-külön hozzá kell add a botot ha nem kap adminisztrátor jogot.)<br><br>

## 📁Tárolt adatok
  - Ha nincs beállítva a szint rendszer akkor addig semmit nem tárol.
  - Ha konfigurálod a szintrendszert, akkor mentésre kerülnek az alábbi adatok: szerver ID, a csatorna ID amelyekre a bot kiírja a szintlépési üzeneteket, **HA** állítottál be saját üzenetet akkor az üzenet szövege, **HA** állítottál be a szintekhez rangot akkor a rang ID és a szint mentésre kerül, **HA** állítottál be  bónusz xp-t kapó rangot, akkor a rang ID és a mennyiség mentésre kerül.
  - Ezeken kívül pedig még mentésre kerül minden a szerveren üzenetet hagyó felhasználó ID-ja azután hogy be lett kapcsolva a szintrendszer. Ez nyilván azért van, hogy felhasználónként nyomon tudja követni a hozzájuk rendelt xp-t és a szintet a bot.
  - A bot **SEMMILYEN** üzenetet nem ment, csak az érte járó xp-t írja jóvá a felhasználónak.<br>
  - Ha a bot eltávolításra kerül a szerverről, de be volt kapcsolva a szintrendszer az adatok nem törlődnek.

**Ezek az adatok kérésre bármikor eltávolíthatók**
Ez ügyben kérlek keress fel engem discordon, vagy pedig hozz létre egy ticketet a support szerveren.


