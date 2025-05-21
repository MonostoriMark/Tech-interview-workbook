# Tesztautomatizálási kérdések

## Tesztelési alapok (ISTQB-hez kapcsolódó)
<img src="https://www.mindsmapped.com/wp-content/uploads/2016/06/ISTQB.jpg" alt="image" width="300" height="220">

#### ✅ Mi a tesztelés célja? Mi nem az?
     A tesztelés célja a hibák és esetleges hiányosságok feltárása, de nem célja a hibamentesség garantálása.




#### ✅ Mik a tesztelési alapelvek?
    Hibák jelenléte bizonyítható, a kimerítő tesztelés lehetetlen, a korai tesztelés költséghatékony, a hibák egyenlőtlenül oszlanak el, a tesztelés kontextusfüggő, az ismétlődés hatékonyságot csökkent, és a teszteket folyamatosan frissíteni kell.




#### ✅ Mi az egységtesztelés (unit testing)? Ki felelős az egységtesztek írásáért?
A tesztelés azt mutatja, hogy vannak hibák.
A kiterjedt tesztelés lehetetlen.
Korai tesztelés, a fejlesztési folyamat korai szakaszában.
Hiba a fürtözésben, keressen érzékeny helyeket.
Paradox peszticid, ne ismételje meg ugyanazt a tesztet.
A tesztelés kontextustól függ.



#### ✅ Mik a tesztszintek, és mi a különbség köztük?
    Egységteszt
    Integrációs teszt
    Rendszerteszt
    Felhasználói vagy elfogadási teszt


#### ✅ Mi a különbség a verifikáció és a validáció között?
    A verifikáció annak ellenőrzése, hogy a szoftver megfelel-e a tervezési és specifikációs követelményeknek, míg a validáció azt vizsgálja, hogy a szoftver megfelel-e a felhasználói igényeknek


#### ✅ Mik a tesztelési típusok, és mi a különbség köztük?
``` Fukcionális tesztelés
    Nem-funkcionális tesztelés
    regressziós tesztelés
    Exploratory tesztelés
    Automatizált tesztelés
    Manuális tesztelés

    A funkcionális tesztelés a szoftver működésére összpontosít, míg a nem-funkcionális tesztelés a működés minőségi jellemzőit vizsgálja; a regresszió a módosítások hatásait ellenőrzi, az exploratory és manuális tesztelés kevésbé strukturált, míg az automatizált szkriptelt és ismételhető.
```

#### ✅ Mi a különbség a fehér doboz, szürke doboz és fekete doboz tesztelés között?
    Fehér doboz tesztelés: A belső kódstruktúra és logika ismeretében történik, és a tesztelő hozzáfér a forráskódhoz.

    Fekete doboz tesztelés: Csak a bemeneti adatokra és a kimenetekre összpontosít, a belső működés ismerete nélkül.

    Szürke doboz tesztelés: Korlátozott ismeretekkel rendelkezik a belső működésről, de főként külső funkciókat vizsgál.


#### ✅ Mi a különbség a felhasználói elfogadási teszt (UAT) és a rendszerteszt között?
    A rendszerteszt a teljes szoftverrendszer tesztelése a specifikációk és műszaki követelmények alapján, technikai szempontból, míg a felhasználói elfogadási teszt azt vizsgálja, hogy a rendszer megfelel-e a végfelhasználók üzleti igényeinek és valódi használati körülmények között is működik-e.



#### ✅ Sorolj fel különbségeket a regressziós tesztelés, a füsttesztelés és az újratesztelés között!
    Fókusz: Regresszió a rendszer egészének stabilitását, füstteszt az alapvető működést, újratesztelés a javított hibák ellenőrzését célozza.

    Tesztesetek száma: Regresszió sok tesztesetet futtat, füst kevés alapvetőt, újratesztelés csak a hibák köré épül.

    Időzítés: Regresszió a módosítások után, füstteszt az új build elején, újratesztelés konkrét hibajavítás után történik.


#### ✅ Mi a különbség a statikus és dinamikus tesztelés között?
    A statikus tesztelés során a szoftver kódját vagy dokumentációját anélkül ellenőrizzük, hogy azt futtatnánk, például kódfelülvizsgálatok, statikus elemző eszközök, vagy dokumentációs ellenőrzés révén. A cél a hibák és problémák feltárása már a kód vagy a rendszerterv írása előtt.

    A dinamikus tesztelés során a szoftver valódi futtatása közben ellenőrizzük annak működését, például tesztesetek végrehajtásával, amely magában foglalhat funkcionális, teljesítmény- vagy integrációs teszteket.


### ✅ Hasonlítsd össze a V-modellt, a vízesés modellt és az Agile megközelítést a tesztelés szempontjából!
    V-modell: A tesztelés a fejlesztés szoros kísérője, lineáris és jól meghatározott fázisokkal.

<img src="https://t4.ftcdn.net/jpg/03/90/15/65/360_F_390156585_8w1lsOyICIAOvDCU8tExXW2QwLCOFwXD.jpg" alt="image" width="550" height="400">

    Vízesés modell: A tesztelés a fejlesztési ciklus végén történik, a változtatások nehezebben implementálhatóak.

<img src="https://i.imgur.com/S38EBJw.png" alt="image" width="550" height="400">   <img src="https://segedletek.level14.hu/assets/img/modszertan-vizeses.svg" alt="image" width="550" height="400">
    
    Agile: A tesztelés folyamatosan, iteratívan történik a fejlesztéssel párhuzamosan, magas rugalmassággal, de gyors ütemű munka esetén a teljes körű tesztelés kihívást jelenthet.

<img src="https://promanconsulting.hu/wp-content/uploads/2022/03/agilis-modszertanok-optimized.jpg" width="550" height="400">











## Reporting, Bugs
<img src="https://moolya.com/blog/wp-content/uploads/2023/05/Bug-Report.png" alt="image" width="300" height="220">

#### ✅ Milyen lépéseket követnél egy hiba megtalálásakor?
    Hiba reprodukálása:
    Ellenőrzöm, hogy a hiba újra előidézhető-e. Ez segít meghatározni, hogy valóban hibáról van szó, és hogy milyen körülmények között fordul elő.

    Dokumentálás:
    Rögzítem a pontos lépéseket, amikkel a hiba előidézhető, a környezetet (böngésző, operációs rendszer, eszköz, verziók), valamint a várt és tényleges viselkedést.

    Logok és konzolüzenetek vizsgálata:
    Megnézem a konzolban, logfájlokban vagy szerveroldali naplókban lévő hibaüzeneteket, amelyek segíthetnek a hiba forrásának beazonosításában.

    Izolálás:
    Helyes működő komponensek kizárása, a hiba okának pontosabb feltárása

    Jelentés készítése:
    Ha nem tudom azonnal megoldani, részletes hibajelentést készítek a fejlesztők vagy az illetékes csapat számára.


#### ✅ Beszélj a gyakori tesztjelentésekről és részleteikről!
    Smoke Test:
    Főbb funkciók működésének gyors ellenőrzése. Ha ez megbukik, nincs értelme tovább tesztelni.

    Regression Test:
    Megmutatja, hogy egy új funkció vagy javítás nem okozott-e visszalépést a már működő funkciókban.

    Functional Test:
    A rendszer funkcionális követelményeinek tesztelése, amely részletezi, hogy az egyes funkciók hogyan viselkednek.

    Exploratory Test:
    Kevésbé strukturált, a tesztelő tapasztalata alapján feltárt hibákat tartalmazza.

    Jelentés részletei:
     - Tesztelés dátuma, környezet
     - Tesztelt funkciók listája
     - Elvárt vs. tényleges eredmények
     - Sikeres/sikertelen tesztek
     - Tesztelő neve, verziószámok

#### ✅ Mit tartalmaz egy hibajelentés?
     - Hiba címe (rövid, lényegretörő leírás)
     - Prioritás / Súlyosság
     - Környezet (böngésző, OS, app verzió, stb.)
     - Reprodukálási lépések
     - Várt eredmény
     - Tényleges eredmény
     - Csatolmányok (screenshot, log, videó)
     - Státusz (új, visszaigazolt, javítás alatt, stb.)
     - Hozzárendelt személy / csapat


#### ✅ Hogyan rangsorolnál egy hibát?
    Súlyosság:
     - Kritikus –> Rendszerösszeomlás, adatvesztés, nem használható funkció
     - Magas –> Fő funkció hibás, workaround nincs
     - Közepes –> Nem alapvető funkció hibás, workaround lehetséges
     - Alacsony –> Esztétikai hiba, helyesírási hiba

    Prioritás:
     - P1 –> Azonnali javítás szükséges
     - P2 –> Magas prioritás, következő sprint-be kerül
     - P3 –> Alacsonyabb prioritás, későbbi javítás
     - P4 –> Nem sürgős, hosszú távú backlog-ba kerülhet



## Test Automation, Selenium
<img src="https://media.licdn.com/dms/image/C4D12AQE3GOyVsZazOw/article-cover_image-shrink_600_2000/0/1583830696602?e=2147483647&v=beta&t=bYHbKyhMoWsMgtEug6eSf3m0db5ZtGEl437TeS1qkfI" alt="image" width="320" height="220">

#### ✅ Melyik teszteseteket érdemes automatizálni és melyiket nem?
    Érdemes:
     - Ismétlődő tesztek: pl. regressziós tesztek, smoke/sanity tesztek.
     - Stabil, jól meghatározott esetek: ahol az elvárt viselkedés világos és nem 
       gyakran változik.
     - Több böngészőn vagy konfiguráción futtatandó tesztek.
     - Adatvezérelt tesztek: pl. űrlapok, ahol sokféle bemenetet kell kipróbálni.
     - Performance tesztek / API tesztek – jól skálázhatók és gyorsan futnak.

    Nem érdemes:
     - Gyakran változó felületű vagy logikájú funkciók.
     - Egyszeri vagy ritkán végzett manuális tesztek.
     - Tiszta UX vagy felhasználói élmény tesztek.


#### ✅ Írj le egy jó automatizált tesztet!
    Stabil: Olyan funkciót tesztel, amely ritkán változik, és fontos az alkalmazás működése szempontjából.

    Reprodukálható: Minden alkalommal ugyanúgy lefut, emberi beavatkozás nélkül.

    Gyors és hatékony: Nem tart sokáig, mégis kritikus működést ellenőriz.

    Karbantartható: Könnyen módosítható, ha változik a bejelentkezési oldal vagy a folyamat.

    Világosan dokumentált: Egyértelmű, mit csinál a teszt, és mitől számít sikeresnek.


#### ✅ Mi a Selenium, Selenium IDE és Selenium WebDriver?
    Selenium: Automatizált tesztelési keretrendszer webalkalmazásokhoz, több böngésző támogatásával.

    Selenium IDE: Böngésző bővítmény (pl. Chrome, Firefox), amivel vizuálisan lehet rögzíteni, lejátszani teszteket. Inkább kezdőknek vagy gyors prototípushoz.

    Selenium WebDriver: Programozható API Python, Java stb. nyelveken, amivel alacsony szinten lehet vezérelni a böngészőt.


#### ✅ Hogyan lehet azonosítani a webes elemeket?
    ID: By.ID("loginBtn")

    Name: By.NAME("email")

    Class name: By.CLASS_NAME("input")

    Tag name: By.TAG_NAME("input")

    CSS selector: By.CSS_SELECTOR("#form .input")

    XPath: By.XPATH("//button[text()='Login']")


#### ✅ Hogyan lehet várni az elemekre, és mi lehet a probléma? Gyűjtsd össze a lehetséges hibákat és okokat!
    Implicit wait: Általános késleltetés minden elemkeresésre.

    Explicit wait: Bizonyos feltételre várunk, pl. elem láthatósága.

    Fluent wait: Egyéni polling intervallummal és kivételek kezelésével.

    Gyakori hibák:
     - Elem még nem töltődött be.
     - Ajax kérés még nem futott le.
     - Rossz az XPath vagy ID.
     - Frame-ben vagy modalban van az elem.
     - Oldal újratöltése megszakítja az interakciót.


#### ✅ Hasonlítsd össze a POM és a Keyword Driven Testing megközelítéseket!
| Jellemző                  | POM (Page Object Model)                   | Keyword Driven Testing                    |
| ------------------------- | ----------------------------------------- | ----------------------------------------- |
| **Felépítés**             | Minden oldalhoz külön osztály             | Kulcsszavakhoz logika, adatból vezérelt   |
| **Tesztelők szerepe**     | Főleg fejlesztők írják                    | Nem fejlesztők is írhatnak (pl. Excelből) |
| **Újrafelhasználhatóság** | Nagyon jó (újrafelhasználható objektumok) | Jó, ha a kulcsszavak jól definiáltak      |
| **Tanulási görbe**        | Magasabb                                  | Alacsonyabb (ha eszközzel támogatott)     |
| **Rugalmasság**           | Magas                                     | Korlátozottabb                            |




#### ✅ Mi a különbség a TDD és BDD között?
| Jellemző           | TDD (Test Driven Development)                  | BDD (Behavior Driven Development)                |
| ------------------ | ---------------------------------------------- | ------------------------------------------------ |
| **Fókusz**         | Fejlesztői tesztelés – *"mit csináljon a kód"* | Viselkedés – *"mit csináljon az alkalmazás"*     |
| **Tesztek nyelve** | Kódhoz közeli (pl. JUnit, pytest)              | Természetes nyelv (pl. Gherkin: Given-When-Then) |
| **Szereplők**      | Fejlesztők                                     | Fejlesztők + tesztelők + üzleti szereplők        |
| **Eszközök**       | JUnit, NUnit, pytest                           | Cucumber, Behave, SpecFlow                       |




#### ✅ Mi az API tesztelés és miért hasznos?
    API tesztelés az alkalmazás backend (REST/SOAP) interfészeinek tesztelése, GUI nélkül.

    Miért hasznos?
     - Gyorsabb, mint UI-tesztelés.
     - Stabilabb – kevésbé érzékeny UI-változásokra.
     - Korán tesztelhető (még UI nélkül is).
     - Ellenőrizhető: válaszformátum, státuszkód, adathelyesség.

    Eszközök: Postman, REST Assured, SoapUI, Newman, pytest + requests.



#### ✅ Mi az adatvezérelt tesztelés és miért hasznos?
    Adatvezérelt tesztelés (Data-Driven Testing) során ugyanazt a tesztet többféle bemeneti adattal futtatjuk.

    Miért hasznos?
     - Csökkenti a duplikált tesztek számát.
     - Nagy lefedettség – különböző esetek tesztelése egy teszttel.
     - Könnyen karbantartható: az adatok külön fájlban (CSV, Excel, JSON stb.)