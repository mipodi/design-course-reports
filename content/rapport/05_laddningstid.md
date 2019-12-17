Laddningstid
=======================

Uppgiften gick ut på välja ut tre webbplatser och testa dem för att titta närmare på laddningstid och möjliga vägar till bättre användbarhet.

Urval
-----------------------

Jag valde samma som under färgrapporten eftersom min första tanke var: undra hur de webbplatserna jag hade förra veckan presterar?!

[Codex Atlanticus](http://www.codex-atlanticus.it/#/)

[A visual introduction to machine learning](http://www.r2d3.us/visual-intro-to-machine-learning-part-2/)

[Market Café Mag](https://www.marketcafemag.com/)


Metod
-----------------------

Jag gjorde analysen med hjälp av inkognito mode i Google Chrome samt stängde av alla adblockers. Med hjälp av dev tools i Chrome gick jag in under network och stängde av cachen. Sedan gjorde jag en hård inläsning och efter det läste jag av informationen och dokumenterade det i ett kalkylark nedan. Google PageSpeed var behjälpligt med ranking (också dokumenterat i kalkylarket) samt stöd för analysen.


Resultat
-----------------------

[Rådatan i ett externt kalkylark](https://docs.google.com/spreadsheets/d/1Q_ggUimFyqLWbGGI2lzOeVK6Pb4QMFpVM8zlcgrWr2g/edit?usp=sharing)

### Codex Atlanticus
[FIGURE src=image/codex-atl-1.png?w=500 alt=""]
[FIGURE src=image/codex-atl-2.png?w=500 alt=""]

[Startsida](http://www.codex-atlanticus.it/#/)

[Översikt](http://www.codex-atlanticus.it/#/Overview)

[Detaljsida](http://www.codex-atlanticus.it/#/Detail?detail=365)

#### Data
Codex Atlanticus fick riktigt kasst resultat på mobilen via Google PageSpeed, under 10 på alla sidorna och den sista gick inte att nå via mobilen (men det verkar bero på att mobilupplevelsen är tänkt att fungera annorlunda). Under network-fliken på devtools så får sidorna mellan 1,8 sek till 5,4 för den sista sidan. Många requests (uppemot 100) och ca 3,5 MB överförs.

#### Kommentar
Webbplatsen skulle kunna läsa in viktiga resurser i förväg, css t.ex. Den skulle kunna spara 10 sek på det under översikten. Den kan även minska antalet element i DOM-trädet, komprimera med ett bibliotek som är specialiserat på det.


### Visual Intro to Machine Learning Part 2
[FIGURE src=image/visual-intro-ml.png?w=500 alt=""]

[Startsida](http://www.r2d3.us/)

[Visualisering maskininlärning](http://www.r2d3.us/visual-intro-to-machine-learning-part-2/)

[Föreläsningssida med slides](http://www.r2d3.us/talks/design-in-a-world-where-machines-are-learning/)

#### Data
Startsidan fick rätt bra resultat, 98 och 99 på mobil respektive desktop i Google PageSpeed score och den tar 0,7 sek att ladda in. Sida två med javascript-baserad visualisering stod ut med 32 och 70 i Google PageSpeed score. Den ligger på 4 sek att ladda in och gör 47 requests. Att jämföra med sista sidan som är väldigt bildtung jämfört med den tidigare, den får bra resultat i på Google PageSpeed, 97 på mobil och 100 på desktop. Däremot tar den 2,24 att ladda in och gör 93 requests samt överför 9,9 MB.

#### Kommentar
Även den här webbplatsen kan läsa in viktiga resurser i förväg, ta bort resurser som blockerar renderingen, exempelvis skjuta upp inläsningen av JS-kod som är mindre viktig. Den kan spara 6 sek på att använda rätt bildstorlek, speciellt på mobilen.

### Market Café Magazine
[FIGURE src=image/market-cafe-1.png?w=500 alt=""]
[FIGURE src=image/market-cafe-2.png?w=500 alt=""]

[Startsida](https://www.marketcafemag.com/)

[Detaljsida](https://www.marketcafemag.com/product/market-cafe-magazine-issue-5)

[Kontaktsida](https://www.marketcafemag.com/contact)

#### Data
Market Café Mag har sitt hyfsat på det torra, ca 87 på mobilen och 100 på desktop från Google PageSpeed. Alla sidor tar mellan 1,7 och 2 sek att läsa in, det överförs en del data (1,20 startsidan, 0,8 för andra och 0,3 för kontaktsidan) och görs som max 32 requests.  

#### Kommentar
Denna webbplats kan använda rätt storlek på bilder för att förbättra sig. Den kan nog ta bort en del resurser som blockerar inläsningen samt minifera koden.



Analys
-----------------------

Det viktigaste verkar vara att använda rätt storlek på bilder och ha koll på sitt DOM-träd så att inte det tar överhanden.

#### Rankning
Jag vänder på steken och lägger rangordningen så här:

Market Café Magazine (vinnare)

R2D3

Codex Atlanticus

Samtidigt så är inte vinnaren full av visualiseringselement, så det är lite svårt att jämföra.

#### Min egna gräns
Jag tror under 1 sek är vad jag uppfattar som en snabb webbplats. När det börjar gå över 2-3 då blir det en långsam sajt. Mitt urval av webbplatser klarar ju inte riktigt det, bara en sida gör det på R2D3:s webbplats. Samtidigt har jag inte tänkt på de andra som långsamma webbplatser tidigare. Möjligen faktiskt samma R2D3 har känts som seg. Codex Atlanticus har nog en del grafiska trix för sig som gör att det uppfattas som en snabbare webbplats än vad det är, men jag har svårt att sätta fingret på vad.


Referenser
-----------------------

[Chrome devtools - network](https://developers.google.com/web/tools/chrome-devtools/network)

[Google PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/)

Övrigt
-----------------------

Rapportförfattare: Julia Johansson.
