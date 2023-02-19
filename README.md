########################################################################################################
#   MAGYAR LEÍRÁS LENTEBB VAN, AZ ANGOL VERZIÓ ALATT  #   
########################################################################################################
#   HUNGARIAN VERSION IS BELOW THE ENGLISH ONE  #

This is the public version of my thesis project. If you want to know more about this project, or if you want to discuss the code, please contact me.
I made the code private, because I have tons of work put in it, and I (and my university teachers as well) see the potential in it that I could make it something bigger. 

In this file, only the summary of my thesis work is included, but in the future I will put a video, and an url of the working site, to this repository.

"I have achieved all the goals of my thesis project. The building of the graph of Budapest
was separated from the software’s other parts, because it took over 35 hours to build
since I wanted to assure the two-way properties of each path, because the software is
designated to people who want to walk or run. Loading the already built graph is much
faster, it takes only 6 seconds.
I implemented both A* and Dijkstra algorithms, furthermore I also implemented an
alternative version for both algorithms, that prioritizes footways over paths that are
sidewalks. These algorithms can be used to generate routes between two points on the
map, but for the randomly generated route another implementation was needed. The
random route generation is generating a route that has the same starting point as it’s
ending point. I modified the alternative A* algorithm to implement this random
generation. This random generation might be slower, the longer the route’s required
length is, but it is more precise in staying close to the required length. The evaluation
and comparison of these algorithms had been done between them, and between other
applications as well. It can be seen from these comparisons that the A* algorithm is
much faster than the Dijkstra algorithm. The Haversine formula could be used for both
the exact distance calculation, and the estimated distance calculation, that could be used
for an optimal heuristic.
To display the generated routes, and to be able to initiate these generations, I used an
incteractive map provided by Mapbox, at the Frontend part of the application. The
communication between the Frontend and the Backend is done via REST API calls.
The user can select which route generating algorithm they want to use, or if they want
to do a random generation, then to determine what the length of that generation should
be. The shape of these random generations is close to a round route.
The determination of which point in the graph is the closest to the placed point on the
map can was done, and after that, using the angles of vector I could decide on which
segment the said point lies on, but this is not perfect. I also modified the geocoordinates
at the two ends of the generated route, so the software would really generate a route
between the placed two points. I also determined where the user would have to turn at
certain points of the generated route, and the total length of the route was also
determined, by including the modifications at the two ends of the route."

-----------------------------------------------------------------------------------------------------------------
HUNGARIAN - MAGYAR

Ez a szakdolgozatom publikus verziója. Kérlek amennyiben többet szeretnél tudni a projektről, vagy amennyiben meg szeretnéd tekinteni a kódot,
vedd fel velem a kapcsolatot.
Azért nem publikus a kód, mert rengeted munkám van benne, és az egyetemi Tanáraim, illetve én is látom benne a potenciált hogy egy nagyobb projektté váljon.

Egyelőre csak a szakdolgozatom végén lévő összefoglalást szúrnám be ide, de a későbbiekben bővíteni fogom egy videóval, illetve a használható oldalhoz vezető linkkel
is ezt a repositoryt.

"A szakdolgozatomhoz kitűzött célok mindegyikét sikerült megvalósítanom. Budapest
térképének felépítését elkülönítettem a szoftver többi részétől, mivel egy ekkora méretű
gráfnál ügyelnem kellett a kétirányúság biztosítására is, több mint 35 óráig tartott
Budapest szűrt térképének a felépítése. A gráf felépítése után generált fájljaim
betöltésével sokkal gyorsabban, csupán 6 másodperc alatt be tudtam tölteni Budapest
teljes, megfelelően szűrt és felépített térképét a memóriába.
Az útvonal generáló algoritmusok közül mind az A*, és a Dijkstra algoritmust is
megvalósítottam, illetve ezeknek egy átalakított, nem járdákat előnyben részesítő
verzióit is sikerült megcsinálnom. Ezek két pont közötti útvonal generálásához
megfelelően működnek, ráadásul a tesztelés, illetve a kiértékelés során bemutatott
esetekben, bizonyos szemszögekből még más alkalmazásokkal szemben is jobban
teljesít. A véletlenszerű generáláshoz is sikerült elkészítenem egy külön algoritmust,
amihez az A* algoritmus már átalakított alternatív verzióját módosítottam tovább. A
véletlenszerű generálás, habár nagy távolságoknál lassú, nagyon pontos. A generáló
algoritmusok kiértékelését elvégeztem, amiből gyakorlatban is látható, hogy az A*
algoritmus mennyivel jobban teljesít a Dijkstra algoritmusnál. Az útvonaltervezéshez
használt súlyszámításokhoz a Haversine formula pontos súlyok megadására is
használható volt, viszont optimális heurisztikaként is alkalmazni tudtam.
A generált útvonalak megjelenítéséhez, illetve a generálás kezdeményezéséhez egy
Frontend részt is megvalósítottam. Ez REST API kérések segítségével kommunikál a
program Backend részével, ahonnan json formában kapja a megfelelően generált
adatokat. A Frontend oldalon a felhasználó kiválaszthatja, hogy milyen
útvonaltervezési algoritmus szerint szeretne utakat generálni két pont között, a pontokat
pedig egy interaktív térkép segítségével tudja meghatározni, amihez a Mapbox által
szolgáltatott térképet használtam. Ezen kívül pedig lehetősége van egy távolság
megadásával egyetlen pontból útvonalat generálni, ami oda fog visszaérkezni, ahonnan
indult, alakja pedig egy körútra fog hasonlítani.
Az útvonal generálása során meg tudom határozni, hogy a térkép melyik pontja fekszik
legközelebb a felhasználó által lerakott ponthoz, majd a két pont közötti vektor
irányszöge által azt is el tudom dönteni, melyik Segment elemen fekszik a felhasználó
által lerakott pont. Ez nem az optimális működése a programnak, de a 11. fejezetben
kifejtettem miért nem működik optimálisan máshogy a kezdő és célpont kiválasztása.
Ezen kívül az útvonaltervezés által generált út széleinek rendbe rakása is működik a
felhasználó által lerakott pontok szerint, hogy ténylegesen a lerakott két pontja között
jelenjen meg az útvonal a térképen, illetve az utat felépítő útszakaszok, vagyis Segment
elemek között is meg tudtam határozni, mikor merre kell fordulnia a felhasználónak. A
tervezett útvonal hosszának számításakor mindig a már módosított útvonalat adom
vissza, ezért ez is a megfelelő értéket adja vissza."
