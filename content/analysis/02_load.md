---
Title: Loading
Description: This is our Loading page
Template: analysis
---

Loading
=======================


Urval
-----------------------

Jag kommer jämföra hur tre olika modehus, Dries van noten, Rick Owens och Yohji Yamamoto, presterar när det kommer till laddningstider. Frågan är om dem behöver offra/ändra deras nuvarande visualisering för att förbättra sina laddningstider.

Dries van noten [1], besöktes 2022-12-01
Dries van noten [2], besöktes 2022-12-01
Dries van noten [3], besöktes 2022-12-01
<br>
Yohji Yamamoto, [4] besöktes 2022-12-01
Yohji Yamamoto, [5] besöktes 2022-12-01
Yohji Yamamoto, [6] besöktes 2022-12-01
<br>
Rick Owens, [7] besöktes 2022-12-01
Rick Owens, [8] besöktes 2022-12-01
Rick Owens, [9] besöktes 2022-12-01



Metod
-----------------------
Jag kommer använda mig av devtools och pagespeed för att komma fram till mina resultat.

Resultat
-----------------------
<h1>m = mobil
d = dator</h1>
<br>
Dries Van Noten:<br>
<img src="%base_url%/image/dries.jpg" width="40%" alt="bild"><br>
<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQEYttHubCdR14plYUhpWCKWcgN0eFAUHKHGBjVTt-bOiJdSTMNlDvLVZe8HBY0mY6V47WaTwO0Oxq6/pubhtml?widget=true&amp;headers=false" title="title"></iframe>

https://docs.google.com/spreadsheets/d/e/2PACX-1vQEYttHubCdR14plYUhpWCKWcgN0eFAUHKHGBjVTt-bOiJdSTMNlDvLVZe8HBY0mY6V47WaTwO0Oxq6/pubhtml

Yohji Yamamoto:<br>
<img src="%base_url%/image/yohji.jpg" width="40%" alt="bild"><br>
<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vSoSdZTJEGIW1UZV41_uf0ozNv9yRFW3Ng6M5UMUEm_RgAbTUKcGcfRKszlGqMyergyfrzylUHCHUfp/pubhtml?widget=true&amp;headers=false" title="title"></iframe>

https://docs.google.com/spreadsheets/d/e/2PACX-1vSoSdZTJEGIW1UZV41_uf0ozNv9yRFW3Ng6M5UMUEm_RgAbTUKcGcfRKszlGqMyergyfrzylUHCHUfp/pubhtml

Rick Owens:<br>
<img src="%base_url%/image/rick.jpg" width="40%" alt="bild"><br>
<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vTySSfWngDp3ZWFqxr1bRTy47SyqbXLqE40oAMjaWHr-M8qUXtQxRDNMBe6nbRFYSkNREDSiMdA2ZvH/pubhtml?widget=true&amp;headers=false" title="title"></iframe>
https://docs.google.com/spreadsheets/d/e/2PACX-1vTySSfWngDp3ZWFqxr1bRTy47SyqbXLqE40oAMjaWHr-M8qUXtQxRDNMBe6nbRFYSkNREDSiMdA2ZvH/pubhtml


Analys
-----------------------
Generell analys:
Ett snabbt sett att generellt skynda på laddningstiden är att gzippa alla filer för att mindre data ska överföras. Något som var tydligt i resultaten var den låga prestandan och laddningstiden för mobiltelefoner. Detta var märkbart för varje sida som togs upp i analysen. Om man kollar på resultaten så är det tydligt att Yohji Yamamotos hemsida är en överlägsen förlorare. Dries van notens och Rick owens hemsidor hade ganska jämna resultat. Jag skulle nog säga att Rick owens hemsida är en vinnare prestanda-mässigt. Jag föredrar laddningstider på max 3 sekunder. Annars så känns det väldigt hackigt och segt. Jag tror ändå att man slipper offra visualiseringen av sitt varumärke för att nå bra laddningstider. Vissa bilder och videos kan självklart ta upp mycket plats. Men det går ändå att kombineras med bra laddningstider.
<br>
<br>
Inviduella förbättringar som kan göras:
<br>
<br>
Dries van noten:
När jag kollar på pagespeed[10] så ser jag flera förbättringspotentialer som kan förminska laddningstiden för sidorna som jag gått igenom. Jag ser att man istället kan använda sig av bilder med lämplig storlek istället för att behöva ändra om storleken i koden. Dessutom så ser jag att det finns en del oanvänd Javascript som man kan bli av med för att göra laddningstiden snabbare. För mobilen är det estimerat att det kan göra en skillnad på 4,66 sekunder.
<br>
<br>
Yohji Yamamoto:
På pagespeed[10] så får jag flera förslag på möjligheter som kan göra att laddningstiden minskar. Där finns bland annat en del oanvänd javascript som man kan försöka bli av med. Utöver det så har vi bland annat oanvänd css som man kan bli av med. Dessutom så tipsas det om att ha en kortare responstid för main dokumentet eftersom alla andra serverrequests bli påverkade av den långa responstiden.
<br>
<br>
Rick Owens:
Första möjligheten till förbättring som jag får av pagespeed[10] är att använda sig av next-gen format för bilder. Istället för att använda sig av png och jpg så kan man använda sig av format som WebP och AVIF för att mindre data ska överföras. Likt Dries van noten så finns möjligheten att använda sig av bilder med lämplig storlek så man slipper slösa tid på att koden ska ändra storleken på bilden. Utöver det så finns en del oanvänd javascript för mobila enheter vilket verkar vara vanligt för de hemsidor som jag gått igenom.




Referenser
-----------------------

https://www.driesvannoten.com/[1]
https://www.driesvannoten.com/collections/fragrance[2]
https://www.driesvannoten.com/pages/stories-index[3]

https://theshopyohjiyamamoto.com/[4]
https://theshopyohjiyamamoto.com/shop/pages/recommend.aspx[5]
https://theshopyohjiyamamoto.com/shop/c/c30/[6]

https://www.rickowens.eu/[7]
https://www.rickowens.eu/en/SE/men/section/new-arrivals[8]
https://www.rickowens.eu/en/SE/login[9]
https://pagespeed.web.dev/[10]
Övrigt
-----------------------

Rapporten gjordes av: Olle Frid(studentakronym:olfi22)