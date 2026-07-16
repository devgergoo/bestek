# 📘Bot Dokumentáció <br>
Itt olvashatsz a bot dokumentációiról. Azon belül is a nyereményjátékról.<br>
## 🎉Nyereményjáték felépítése<br>
A nyereményjátékok egy igazán jó lehetőség hogy feldobjuk a szerverünket. Épp ezért nem mindegy hogy hogy is néz ki! Próbáltam minél letisztultabb, jól kinéző nyereményjáték rendszert létrehozni, hogy komfortos legyen 
kezelni, és egyben résztvenni is rajta. Ennek köszönhetően saját magadnak tudod megadni a nyereményjáték cimét, és a leirását is, valamint még a nyertesek számát is tudod állítani, mind eztegy felugró menüben!<br>

![image](https://github.com/user-attachments/assets/b1563fb2-4622-4a02-ac8b-71219b4bbb4c)
<br>

## 🛠Nyereményjáték Konfigurálása
1- Elég egyszerű, a csatornába ahova létre akarod hozni a nyereményjátékot, beírod a `/giveaway` parancsot, és a felugró menüt izlés szerint kitöltöd. Ezzel létre is hoztad a nyereményjátékot!<br>
2- Ha korábban le szeretnéd állítani a nyereményjátékot, és szeretnél nyertest, akkor a `/endg <giveaway_id>`* parancs segítségével tudod. Ha teljesen törölni szeretnéd, hogy nyertest se sorsoljon azt a
`/cancelg <giveaway_id>` parancs segítségével tudod.<br>
3- A jelenleg aktív nyereményjátékokat a `/listg` parancs segítségével tudod megnézni, újrasorsolni a már lejárt nyereményjátékokat pedig a `/reroll <giveaweay_id>` paranccsal tudod.<br>
<br>
**giveaway_id = A giveaway id mindig a létrehozott nyereményjáték üzenetének az ID-ja.*

## 🔔Jogosultságok a parancs futtatásához
  - /giveaway ~ **Adminisztrátor** jogosultság szükséges
  - /endg ~ **Adminisztrátor** jogosultság szükséges
  - /cancelg ~ **Adminisztrátor** jogosultság szükséges
  - /listg ~ nincs szükséges jogosultság
  - /reroll ~ **Adminisztrátor** jogosultság szükséges

## 🤖Bot számára szükséges jogok a szintrendszer müködéséhez
  - (Ajánlott jogosultság az **adminisztrátor**.)
  - Üzenetek küldése
  - Csatornák megtekintése

## 📁Tárolt adatok
  - A bot az alábbiakat tárolja el a nyereményjátékokról: Szerver ID, Üzenet(giveaway_id) ID, csatorna ID, nyeremény, jelentkező felhasználók ID-ja, nyereményjáték leírása, nyertesek száma, létrehozás ideje, nyereményjáték végének ideje, nyereményátéknak vége van-e?(rerollhoz.)

**Ezek az adatok kérésre bármikor eltávolíthatók.**
Ez ügyben kérlek keress fel engem discordon, vagy pedig hozz létre egy ticketet a support szerveren.
