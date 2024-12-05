# Rapport kmom05 - Prestanda.

Detta är en rapport för kmom05. Uppgiften handlar om prestanda för 3 olika webbplatser. Häri görs mätningar och slutsatser dras från dessa.

<br>
<br>

## Urval

Samma som i analys 1.
<br>
<br>

## Metod

Ta en snapshot (bild) på webbplatsen.
Välj ut tre sidor (bifoga länkarna) som skall mätas med Google Pagespeed. Mät på både Mobile och Desktop. Notera de betyg som ges.
För varje sida, mät med devtools flik networks och notera sidans laddningstid tillsammans med antalet resurser som laddas samt sidans totala storlek. För varje sida gör mätningen tre gånger och ta snittet av mätvärdena.
Diskutera och skriv en mening om hur webbplatsen kan förbättra sig.

(Hämtat från Dbwebb KMOM05)

<br>
<br>

## Resultat

### MSA (Mannheimer Swartling Advokatbyrå)

[Länk till hemsidan](https://www.mannheimerswartling.se/)

[Länk till Snapshot](https://imgur.com/2PS5xbb)
<br>
Resultat
<br>

Prestanda Dator (Mobil) | Tillgäng. Dator (Mobil) | Bästa metoder Dator (Mobil) | SEO Dator (Mobil) | Devtools Load | Devtools Requests | Devtools Size
<br>
91 (60) | 93 (93) | 100 (100) | 92 (92) | 514ms | 22 | 12.9MB
<br>
<br>
MSA har goda resultat i alla delar. Däremot är deras prestanda på mobilenheter låg. Här behövs arbete. Videon i headern laddas inte in snabbt. Detta bör de fixa. De har även oanvänd css etc.

<br>

### Vinge Advokatbyrå

[Länk till hemsidan](https://www.vinge.se/)

[Länk till Snapshot](https://imgur.com/2N5rAdS)
<br>
Resultat
<br>

Prestanda Dator (Mobil) | Tillgäng. Dator (Mobil) | Bästa metoder Dator (Mobil) | SEO Dator (Mobil) | Devtools Load | Devtools Requests | Devtools Size
<br>
67 (62) | 79 (79) | 96 (96) | 85 (85) | 2003ms | 39 | 34.6MB
<br>
<br>
Vinge har de sämsta resultaten. Särskilt i tillgänglighet där de har vissa images som inte har alt-attribut :(). Kontrasterna är inte heller tillräckligt stora enligt pagespeed insights. Både på datorn och mobilen är inladdningen långsam. Deras "huvuddokument" laddas på 2sek, inte bra. Dem har även otroligt stort dom träd med 1223 element...

<br>

### Snellman Advokatbyrå

[Länk till hemsidan](https://snellman.com/)

[Länk till Snapshot](https://imgur.com/qrzrK8q)
<br>
Resultat
<br>

Prestanda Dator (Mobil) | Tillgäng. Dator (Mobil) | Bästa metoder Dator (Mobil) | SEO Dator (Mobil) | Devtools Load | Devtools Requests | Devtools Size
<br>
91 (64) | 92 (92) | 100 (100) | 92 (92) | 609ms | 85 | 11.7MB
<br>
<br>
Snellman har liknande resultat som MSA. Problem med mobila prestandan. Dem har en del javascript som inte körs och bör tas bort exempelvis. Bilden på hemskärmen dyker dock upp direkt jämfört med MSA.

<br>
<br>

## Analys

Sammanfattningsvis har både MSA och Snellman i stort goda resultat. Alla är i "grön området" förutom på prestanda för mobilen. Här ligger det både att en del javascript filer aldrig körs och är onödiga och att vissa element tar lång tid att ladda. Vinge, å andra sidan, har mycket större problem. Här har man glömt att ha alt-attribut i bilder och liknande ganska fundamentala saker. Samtidigt har man ett huvuddokument som tar 2sekunder att ladda in vilket gör att ingenting visas förrens 2 sekunder. 2s response tid på en hemsida är faktiskt långt över vad som får anses vara "okej".

<br>

Mina slutsatser i denna analys är att inladdningstiden är extremt viktigt. Både snellman och MSA laddar fort, alla element laddas inte direkt utan får i möjliga fall skeletons. Men att Vinges hemsida har en fördröjning till att allt är färdig renderat är inte trevligt när man laddar hemsidan. De vanligaste förbättringsåtgärderna är att ta bort onödiga javascript resurser som inte körs på mobila enheter. Vinge har även en del requests som inte lyckas träffa någon endpoint eller få resultat, detta är ganska vanligt, men MSA lyckas utan någon sådan.

<br>

Inladdningstid på under 800ms anser jag vara snabbt. Under 600ms är det riktigt snabbt och över 1000ms är långsamt. 2000ms är extremt långsamt. Vinge är extremt långsam (2000ms), MSA är riktigt snabbt (600ms), Snellman är också riktigt snabb (600ms).

<br>

Vinnare blir Snellman. De har både bäst resultat, men också minst storlek på resurserna och minst inladdningstid. 2a blir MSA och 3a Vinge.

<br>
<br>

## Kalkylark

<p style="min-width: 100%;">
<iframe style="min-width: 100%;" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRCJAjK2myLNC4uBvmiy5GOfG1vu7g6PI6gsq4i7SKa6pPPMxVEH2wWClWZ3e8FtuTzmMbIULy8xmfl/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false"></iframe>
</p>

<br>

[Kalkylark](https://docs.google.com/spreadsheets/d/1Fa9pR06-gssVs0TZkMap0h9UORyqQ21Y-GRVoJ_M-a8/edit?usp=sharing)
<br>
<br>

## Referenser

[Mannheimer Swartling](https://www.mannheimerswartling.se/)
[Vinge](https://www.vinge.se/)
[Snellman](https://snellman.com/)
[Kalkylark](https://docs.google.com/spreadsheets/d/1Fa9pR06-gssVs0TZkMap0h9UORyqQ21Y-GRVoJ_M-a8/edit?usp=sharing)

<br>
<br>

## Övrigt

Elis Sandklo (elsd23).
