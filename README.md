# Projekt
* Csapat név: Ellenállók

* Csapattagok: Egyedi Gergő, Timár Klaudiusz

* Lottó program (adatbázis, regisztráció, bejelentkezés, modellezés)

* Követelmény

1. Teljes értékű JavaFX alkalmazás: A hangsúly a funkcionalitáson van, a design másodla-
gos! Félkész funkciók ne legyenek az alkalmazásban! Ha megakadtok egy funkció fej-
lesztése közben, az órákon megbeszéljük. A projektben az MVC struktúrát kell alkal-
mazni (tehát külön-külön fájlokban és osztályokban legyen a nézet, a modell és a kont-
roller). Az alkalmazásban a nagyon eltérő funkciókat külön-külön Pane-en kell megje-
leníteni. Ezeken kívül JDK17-et és Maven csomagolót kell használni!
2. Kivétel- és hibakezelés: Az alkalmazásban minden előforduló kivételt és hibát le kell
kezelni, ennek előfordulásakor adj vissza hibaüzenetet piros betűszínnel egy Label-be!
Ha nem történt hiba és sikeresen lefutott egy funkció, adj vissza fekete / zöld betű-
színnel egy tájékoztató üzenetet ugyanabban a Label-ben!
3. Adatbázis használata JDBC-vel: Az adatbázis funkciókat külön, erre a célra kialakított
osztályban kell implementálni. Adatbázishoz való csatlakozás után érdemes rávizs-
gálni, hogy létezik-e a kívánt adatbázis és táblák. Így ha nem létezik, akkor az alkalma-
zásból létre is tudjuk hozni őket. Célszerű Derby-t használni, viszont egyéb MySQL
megvalósítás is elfogadott.
4. Clean code alapelvek használata: A kód legyen letisztult, a különböző részek megfele-
lően tagolva, indentálva! Figyelni kell, hogy a különböző funkciók külön-külön metó-
dusokba / függvényekbe legyenek tagolva, ne egybe ömlesztve (+ újra felhasználható-
ság)! Értelmes változó neveket kell használni, legyenek beszédesek, hogy kitalálható
legyen, mire is jók. Célszerű kommentelni is, melyik részegység mire való.
5. Szoftver ergonómia: A feliratok jól láthatóak legyenek, a gombok megfelelően kattint-
hatóak legyenek (ne túl kicsi, ne túl nagy)!


1. Készítsd el a projekted dokumentációjához az osztály diagramot! A diagram tartal-
mazza a megoldás összes osztályát, az osztályok adattagjait és metódusait továbbá a
(ha van) jelöld nyilakkal az öröklődéseket
2. A program gyenge pontjain (ahol felhasználótól kérünk adatot), kezelje megfelelően
egy tanult módzserrel úgy, hogy ne okozhasson hibát a felhasználó!
3. A programban valahol használjon legalább egy saját készítésű kivételt!
4. Készítsen tesztelési útmutatót a projektjéhez! Ez egy reademe.md (segédlet) fájl le-
gyen, amiben lépésről lépésre bemutatja az alkalmazás felhasználását. Figyeljen arra, hogy a program minden funkcióját bemutassa vele! Például:
        1. Indítsuk el az alkalmazást a yxz.java futtatásával.
        2. Kattintsunk a “hozzáadás” gombra egy új elem hozzáadásához.
            1. 2/a. Adjunk meg egy nevet a ... mezőbe, ez lesz a ... neve
            2. 2/b Adjunk meg egy évszámot a ... mezőbe, ami a ... lesz
5. Készítsen Unit teszteket a programhoz! Válasszon ki legalább 2 függvényt, amelyhez
elkészíti a Unit teszteteket. Minden függvényhez készítsen egy egyenlőség vizsgálatot
legalább 3 opcióval
6. Szám esetén:
    1. “Nem egyenlő” vizsgálat: túl kicsi opció
    2. “Egyenlő” vizsgálat: megfelelő opció
    3. “Nem szám” vizsgálat: rossz bemenet
7. Szöveg esetén:
    1. “Üres” vizsgálat: üres bemeneti mező
    2. “Megfelelő” vizsgálat: jó bemenő adat
    3. “Hibás” vizsgálat: nem megfelelő adat
1. Bemutató készítése az elkészített szoftverhez.
2. A bemutatónak legalább 15 diát kell tartalmaznia, mely az alábbi felépítést tartal-mazza:
    1. A szoftver céljának rövid bemutatása
    2. A szoftver felépítése (menürendszer, képernyőképek, stb.)
    3. A szoftver használatának bemutatása
    4. Az elkészített szoftver továbbfejlesztési lehetőségei
3. A diákon maximum 28-as betűméret alkalmazható
4. Figyelni kell a helyesírásra, nyelvhelyességre (zavaró elírások, helyesírási hibák, stb.
PONTLEVONÁST fog jelenteni)
5. Az elkészített bemutató előadása


* Munkamegosztás

1. Gergő 
    1. Modellezés, adatbázis, dokumentáció, osztályok,  
2. Klaudia
    1. Bejelentkezés, Regisztráció, Readme, ppt, dokumentáció 

* Megvalósitás

1. Bejelentkezés vagy Regisztráció Lesz 3 stage, gombok segitségével tudsz váltogatni
2. Bejelentkezés: A bejelentkezés gombra katintva megjelenik a bejelentkezés ablak ahol meg kell adni a felhasználónevet és jelszót, az adatbázisban a program mehvizsgálja hogy létezik-e.
3. Regisztráció: A program vár egy jelszót, email cimet, felhasználonevet amit majd át add az adatbázisnak
4. Modellezés: A felhasználó válaszait összehasonlitja a generált válaszait és levonja a megadatott összegből a sorsolás árát
5. adatbázis: Eltárolja a felhasználó nevét, email cimét, jelszavát, tippjeit, nyereségeit és veszteségeit
* Adatok tárolása
1. Adatbázis
