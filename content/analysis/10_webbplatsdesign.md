# Webbplatsdesign (KMOM10)
Detta är en rapport för kmom10 krav 5. Analys av aktuell webbplatsdesign.

<br>
<br>

## Urval

I urvalet av hemsidor har jag valt nyhetssidor, särskilt kända sådana. Anledningen är att jag spenderar en del tid varje dag på dessa hemsidor och tycker det hade varit intressant att analysera dessa.
<br>
<br>

## Metod

* För varje hemsida i urvalet
1) Kommentera webbplatsens mål och syfte.
2) Kommentar om webbplats design och designprinciper.
3) Kommentar om responsibilitet och tillgänglighet
4) Kommentar om användarvänlighet.
5) Kommentar om huvuddragen.
6) Särskild kommentar om någon designprincip.

* I analys och slutsats
7) Dra slutsatser om resultatet.
8) Jämför och analysera samtliga inhämtade datapunkter.

*Metoden har jag valt själv efter ett noggrant tänkande kring just frågeställningen i analys rapporten. Jag anser att webbplatssdesign handlar om mer än bara "design" och användarvänlighet (ux) och responsibilitet och tillgänlighet är minst lika viktiga i denna del.

<br>
<br>

## Resultat

### Dagens nyheter

[Länk till hemsida](https://www.dn.se/)

1) Webbplatssens mål och syfte är att främja informationsfriheten och att övervaka maktutövningen i samhället, i vart fall om man frågar redaktionen själva. Därutöver finns såklart ett vinstdrivande syfte, vilket märks på anonserna till höger.

2) Hemsidan har en content del som är centrerad och har en stor padding/margin ut till båda kanterna. Den omfamnas av borders, vilket gör att den frameas på skärmen. På headern dyker tydligt ordet "Dagens nyheter" upp i uppercase och bold typografi. Färgschemat är svart/vitt med en ton av röd (denna ton, som även byts i vissa artiklar (i ekonomi blir den ljusgrön vilket är ganska snyggt faktiskt) syns längst upp med border och under aktiv tab i navigation). En tydlig princip som sajten använder är grid/ layout. Saker och ting är i regel på en layout som gör att skärmen täcks, dock ej texten i själva artiklarna. Även annonserna tas in i layouten i viss mån vilket är intressant. Väl i artiklarna som börjar med en titel, underrubiker, en bild och texten nedanför görs något intressant. Det finns en tydlig balans och hierarki som princip, men bilden tar sig hela vägen ut till kanten (jämfört med allt annat) detta skapar en "randomness" enligt mig som är ganska uppfriskande. Att allting som är i en flexbox som column inte är lika i bredd gör det lite mer levande och inte lika entydigt. Navigationen i headern är i en row och den aktiva tabben visas genom en undre border med accent-färgen. Typografin är en serif.

3) Hemsidan är mycket responsibel, vilket bör förväntas för en sådan stor hemsida. Det utrymmet på sidorna som finns på desktop försvinner när man har en mindre skärm. När man är inne i devtools märks tydligt att hemsidan använder flertalet media queries för mycket, särskilt för storleken på texten. Även layout och grid förändras, och i tillräckligt små enheter så syns inte annonser på höger sidan för att frigöra utrymmet till huvudsyftet med komponenten vilket är att sprida informationen. I tillgänglighet får startsidan 92/100 på lighthouse för desktop och 96/100 för mobil. Ett problem är att vissa delar i navigationen på desktop anses vara för små för att trycka på. Däremot finns inga avgörande problem. Hemsidan fungerar även väl i färgblindehetstesten [länk](https://www.toptal.com/designers/colorfilter/).

4) Användarvänligheten är bra. Huvudelementen är tillräckligt stora att klicka på och artiklarna avskiljs tydligt med linjer och hierarki och särskilt borders. Däremot blir man direkt på startsidan påtryckt med ett stort antal element vilket kan få en att känna sig överväldigad, här görs dock tydliga hierarki val och det viktigaste (enligt dem) kommer först till blicken på grund av denna användning av designprincip. Viktigast är dock repetitionen eftersom användarna egentligen bara har ett mål och det är att se artiklar som dem vill läsa, och att förändra layout dagligen hade inte varit önsvärt mot detta.

5) Huvuddragen är ett tydligt grid layout med tydlig hierarki, större text och bilder för viktigare artiklar. Dem använder mycket scaling därtill för att betona element i hierarkin och även en del färg för att betona vart på hemsidan du är (särskilt grön för ekonomi etc). Därtill återkommer en stor repetition vilket gör det enkelt att använda sidan.

6) En särskild designprincip är typografi. En sak jag märkte först när jag granskade hemsidan är att repliker från DN ledare eller politsiak kommentatorer betonas med en italic font-style vilket gör dem enkla att solla bort, eller solla in i sitt läsflöde. Detta var intressant eftersom det gör dem enkla att både kolla bort från och att fokusera på. En bold text är desto svårare att göra båda med och i detta sammanhang blir det väldigt bra att använda just italic till dessa artiklar då dem inte passar alla i smaken.

<br>

### Aftonbladet

[Länk till hemsida](https://www.aftonbladet.se/)

1) Webbplatssens mål och syfte är att främja informationsfriheten och att övervaka maktutövningen i samhället, i vart fall om man frågar redaktionen själva. Därutöver finns såklart ett vinstdrivande syfte, vilket märks på anonserna till höger. ** Samma som Dagens nyheter ** 

2) Aftonbladet liknar dagens nyheter på ett mycket stort sätt. Webbplattsen börjar med en hero på en annons som man scrollar ner för att komma till själva "hemsidan". Längst ner syns då headern som sedan blir längst upp. Aftonbladet har här även en tydlig text/ logga "Aftonbladet" i vänstra hörnet på headern och en navigation under som är i en row. Här används dock en background opacity för att visa på aktiv tabb, dock ej för start. Själva layouten är i princip exakt samma som dagens nyheter, här arbetar man mer med att varje artikel delas upp i en enskild box med en bakgrund som är vit, denna är dock inte lika tydlig då bakgrunden också är vit. Intressant typografi mässigt är att man arbetar med många olika typsnittsstorlekar. Exempåelvis används 18px, 30px, 31px, 40px, 42px, 46px, 60px i titlarna för artklarna (detta torde vara beroende på nyhetsvärdet). Härtill används färgschemat på ett intressant sätt. Aftonbladet har ju nästan skapat ett varumärke på att sporten är röd/ rosa och varje sportartikel har därför detta som bakgrund istället för vit nyans. Färgschemat är likväl här svart vit + rött och gult. Typografin är en font av sans-serif.

3) Responsibiliteten är även här mycket bra. Däremot tas annonserna bort från sidan först vid en mobilstorlek. Fontstorlekarna ändras i viss mån, samtliga gör dock inte det eftersom det inte behövs alla fall. Tydligt är att man arbetar med media queries för layout och storlek. En intressant grej är att en burger-menu alltid syns, men att nav tabbarna försvinner så fort de överlappar vilket är en intressant lösning i headern. Tillgängligheten är enligt Lighthouse 86/ 100 på dator med problem beträffande att linkar och knappar inte har namn och att bakgrunden i vissa delar inte har tillräcklig kontrast till vissa element. På mobil är det även här 86/100 med samma problem. Problemen är dock inte avgörande och för ögat syns inte problemen. Kontrast felet är alltså inte avgörande exempelvis. Hemsidan fungerar även väl i färblindhetstest [länk](https://www.toptal.com/designers/colorfilter/).

4) I fråga om användarvänlighet må samma kommentarer som ovan på dagens nyheter sägas. Eftersom layouten är likadan. Däremot tycker jag att det på aftonbladets hemsida är mycket svårare att urskilja artiklar när man scrollar. Det som särskiljer är bilderna vilket är tydligt egentligen på båda sidorna. Något om responsibiliteten i detta sammanhang är att annonserna endast försvinner från sidan på en mycken liten storlek vilket blir problematiskt på medelstora små enheter då artiklarna inte syns lika väl. Huvudändamålen fungerar dock bra, startsidan har alla de viktigaste artiklarna listade och i headern är det enkelt att byta till en viss specifik sektion av nyheter. Headern försvinner när man scrollat, men dyker upp direkt när man scrollar uppåt fastän man inte scrollat hela vägen upp vilket gör det enkelt att byta till en annan sektion.

5) Huvuddragen är lika som dagens nyheter. Härtill används däremot fler färger. Man använder inte bara röd och gul vilket är varumärket utan även blå för att få till en extra accent. Denna särskiljer annonseran mycket tydligt vilket är bra ur en ändamålsenlighet också.

6) Något särskilt om en särskild designprincip är aftonbladets användande av grid, särskilt på sidan när man väl läser en artikel. I alla fall blir inte höger kolumnen av gridet använt av annonser och då känns layouten väldigt ensidig åt vänster. Ögat behöver då endast gå rakt upp och ned. När man scrollat till nästa artikel fortsätter detta. Det blir ensidigt i viss mån och tomt i mycket [Länk till screenshot](https://imgur.com/a/Hrhh7hw). Här borde man kanske överväga att försöka dela upp saker och ting mera som en riktig tidning, jag tror man hade känat designmässigtp på det.
<br>

### Dagens juridik

[Länk till hemsida](https://www.dagensjuridik.se/)

1) Huvudändamålet med hemsidan är sprida information nyheter i det juridiska affärslivet, därtill är den till för ett vinstdrivande syfte. Hemsidan vill framhäva en profesionell ton och är även tydligt riktiade mot verksamma jurister och advokater.

2) Färgschemat är tydligt svart, vitt och härtill även rött. Urvalet är litet om man inte ser till att tre olika grader av röd finns. Annars används bara svart, vit och röd, förutom footern och en knapp som är mörkblå. Typografin är en serif font, men man använder även sans-serikf i footern och har även flertalet olika fonter (två i footern och en i artikel headers). Härtill har man två olika font-families som titel och underubrik på varje artikel. DJ använder ett grid med tre kolumner. Varav den längst till höger är till för annonser som huvudändamål. (Kolumnerna ändras dock för responsibilitet) Mitten kolumnen är lite allt i ett, både sidebars (typ top 5 artiklar) och annan närliggande information (såsom lediga jobb etc) samt vissa annonser och senaste nytt. Huvuddragen är likväl precis som alla andra hemsidor. Man har en centrerad kontet box som blir framerad av allt. Utrymmet på sidorna försvinner dock direkt med mindre enheter. Headern använder däremot design elementen med depth med en border och box-shadow (dev-tools inspect) som gör att den ser lite flytande ut. Den finns också kvar på toppen hela tiden, men all onödig information förutom logga, navigation och vissa knappar döljs. Härtill kan nämnas att texten endast är i två olika storlekar, jämfört med de andra sidorna som har mycket fler urval på font-sizes. 

3) Responsibiliteten för dagens jurdik är god. I typografin och särskilt storleken på texten används rem och vw i en clamp. Det är intressant och fungerar lika bra. Element förminskas och grid layout förändras vid rescaling. Anonsdelen (den längst till höger) förvsinner på medelstora enheter. På mobiler blir det endast en kolumn. I footern förändras även i vilken row allting hamnar när hemsidan förändras i storlek (ikonerna för sociala medier hamnar längre upp). Annonserna blir också betydligt färre och hamnar inte emellan artiklarna. I Lighhouse får hemsidan 80/100 på dator och 85/100 på mobil. Problemen här är att vissa bilder inte har alt-attribut. Att vissa element har dålig kontrast mot bakgrunden, att heading element inte används i rätt ordning och något till. Problemen är däremot inte möjligt att se med ögat. 

4) En tydlig sak som dagens juridik gör med användarvänlighet är att använda olika nyanser av röd som färg för olika typer av prenumerationer. Detta gör sedan att det redan är enkelt på första sidan att veta om man har tillgång till artikeln eller ej. Desto mörkare, desto dyrare vilket också fungerar väl. Därtill har man olika ikoner också, men dessa är så pass små att de är svåra att urskilja. Härtill kommer, som alla andra, att viktiga artiklar har större bilder och är enklare att urskilja ur ett scroll.

5) Huvudragen för webbplattsen är i princip samma som de andra. Jag får dock känslan av att man tagit tillvara på en mer high-end känsla i och med valet av de mest användna principerna. Man använder en tydlig box-shadow på många element vilket gör att de står ut. Därtill används få färger och jag får även känslan av att man har valt bilderna till artiklarna med en synpunkt i att inte alltför starka färger ska ingå (detta kan dock ha och göra med just dagens urval av nyheter), men i princip alla bilder är av mjuk ton och inte hård. Jag tycker huvudraget är typografin. Man har arbetat mycket med hierarkin i olika text-element och det blir ur en användarvinkel enkelt att få hjärnan att följa "rätt" (det tänkta) schemat för att läsa och urskilja artiklar. Tydligt blir det i kolumn 2 på desktop där senaste nytt är i små font-size men inte för liten. Den är minimalistisk men tydlig och enkel att läsa.



<br>

## Analys
Jag har i analysen valt att dela upp slutsatserna under underrubriker för att få till en sammansatt analys och redogörelse.

### Grid och layout
En tydlig trend är att samtliga och även andra som inte kom med i urvalet använder en tydlig grid layout som gör att de enkelt kan hantera både text och annonser effektivt. Detta verkar även vara de bakomliggande syftena med samtliga hemsidor inom branschen, både informationsspridning och vinstsyften ligger alltså bakom layouten. Angående vilket av dessa som prioriteras se avsnitt nedan om responsibilitet.

### Responsibilitet
En slutsats som enkelt framgår av datan som sammlats in är att 

<br>
<br>



## Referenser

[Dagens nyheter](https://www.dn.se/)
[Aftonbladet](https://www.aftonbladet.se/)
[Dagens juridik](https://www.dagensjuridik.se/)
[Färgblindhetstestet](https://www.toptal.com/designers/colorfilter/)
<br>
<br>

## Övrigt

Elis Sandklo (elsd23).
