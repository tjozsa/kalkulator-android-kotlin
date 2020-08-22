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

## Challenge
Érdemes megpróbálni felépíteni a layoutot:
* Csak linear layoutot használj
* Ágyazd őket egymásba
* használd az *android:layout_weight* tulajdonságot arra, hogy több oszlopot öleljen fel egy-egy gomb
* használd a *android:layout_weight* tulajdonságot arra is, hogy egyenletesen osszák fel a sorok és az oszlopok a teret.
* maximúm 12 karaktert jelenítsen meg a textview
* a számoknál használd az **android:onClick** xml tulajdonságot és mindegyik számot reprezentáló gomb ugyan azt a methodust hívja.

<img src="images\shot4.png" width="300"/>

```xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout ...>

    <!-- Challenge 1 STAR: build ui for the application -->

    <TextView
        .../>

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:layout_weight="1"
        android:orientation="vertical">
        <!-- row 1 -->
        <LinearLayout ...>
            ...
        </LinearLayout>
        <!-- row 2 -->
        <LinearLayout ...>
            ...
        </LinearLayout>
        <!-- row 3 -->
        <LinearLayout ...>
            ...
        </LinearLayout>
        <!-- row 4 -->
        <LinearLayout ...>
            ...
        </LinearLayout>
        <!-- row 5 -->
        <LinearLayout ...>
            ...
        </LinearLayout>
    </LinearLayout>
</LinearLayout>
```