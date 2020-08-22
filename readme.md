## Alkalmazas feladata
Egyszerű kalkulátor. Csak annyira kell, hogy működjön, amennyit a használt adattípusok engedni fognak. Ha nagyon hosszú számot kell kijelezni akkor nem várjuk el, hogy a kalkulátor tökéletesen tudjon tovább működni.
Ezekben a helyzetekben a CLR (clear) gomb nyújthat megoldást, mely arra szolgál, hogy alap helyzetbe hozzuk a kalkulátort.

## Felhasználói felület
A teljes felület egy db LinearLayoutban van megvalósítva, persze ezen belül több beágyazott LiearLayout is lehet.

A gombsor előtt egy TextView van ami elég tetemes helyet foglal.

Minden sor gomb 1 db LinearLayout ami horizontális.
Az összes gombsor 1 db LinearLyaoutban van ami vertikális.


<img src="images\shot1.png" width="200"/>
<img src="images\shot2.png" width="200"/>
<img src="images\shot3.png" width="200"/>

## Használandó technológiák
* bonyolultabb felhasználói felület építése XML segítségével
    * Button
    * TextView
    * Linear Laybout
* listener