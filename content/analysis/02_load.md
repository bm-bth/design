---
Title: Laddningstider
Description: Colors
Template: analysis
Sidebar: true
hidden: false
---

##Webbplatsers laddningstid

Denna rapport går ut på att välja ett antal olika webbplatser och testa dem för att mäta deras laddningstider och se om det finns några saker som kan förbättras och på så sätt optimera laddningstiden och användbarheten för webbplatserna.

##Urval

Webbplatserna som har valts ut för mätningen är: <br>
<div class="link-div">
    <ul class="li-list">
        <li><a href="https://www.fastighetsbyran.com/sv/sverige" class="links-analys">1. Fastighetsbyrån</a></li>
        <li><a href="https://www.svenskfast.se/" class="links-analys">2. Svensk Fastighetsförmedling</a></li>
        <li><a href="https://www.lansfast.se/" class="links-analys">3. Länsförsäkringar fastighetsförmedling</a></li>
    </ul>
</div>
<br>
Anledningen till att jag valde dessa webbplatser är att jag ville se om de största och mest etablerade mäklarbyråerna gav någon vikt och uppmärksamhet åt deras webbplatsers laddningstider och optimering. Speciellt med anledning till att fastighetswebbplatserna och mäklarbyråerna använder många bilder i olika storlek och format som kan påverka användbarheten och känslan när besökare surfar in på deras webbplatser.

##Metod
Verktygen för att testa webbplatsernas hastighet och prestanda var Google Chrome devtools och Googles Page insights<sup>1</sup>. Mätningarna togs på webbplatsernas startsida, mäklarsida och till-salu sida. Varje mätning gjordes tre gånger på respektive sida för att ett genomsnittligt värde skulle beräknas. Vidare stängdes Ad-blockern för webbläsaren och alla cachade bilder, filer, cookies och annan webbplatsdata rensades innan mätningen. <br><br>

##Resultat<br><br>
<picture>
    <source media="(min-width: 767px)" srcset="%base_url%/image/fast-start.webp?w=900&">
<img class="loadImg" src="%base_url%/image/fast-start.webp?w=400&q=100" alt="start page fastighetsbyrån">
</picture>
<br>
<div class="embed-container2">
<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRSA6nZAZcenukdhxTkMSk5j812gLCxNWwRlyGrKMSz2b8hpseslvkfK8GmKtDFgB5jy9Skgq43UoD9/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false" title="google sheet fastighetsbyrån"></iframe>
</div>
Fastighetsbyråns webbsidor fick allmänt väldigt dåliga prestanda betyg. För mobiler låg prestanda poängen på mellan 16-20 poäng, och för datorer 52-57 poäng. Webbsidorna tog i genomsnitt mellan 1.7 och 10.86 sekunder på sig att läsas in helt. Detta visas i "load"-kolumnen som visar tiden det tar för alla resurser som skripts, bilder, stylesheets och iframes att läsas in. En av anledningarna till varför Fastighetsbyrån fick så dåliga "load"-tider är pga en bild på Vadstena som finns på mäklar-sidan som är 21.5 MB stor och som tar upp mer än hälften av alla resurser som läses in på sidan. För att förbättra prestandabetygen och laddningstiden kan Javascript och CSS som inte används tas bort. Vidare kan resurser som blockerar renderingen tas bort och bildformaten WebP och AVIF som ger en bättre komprimering användas istället för PNG och JPG-formaten som används för tillfället.<br><br><br>

<picture>
    <source media="(min-width: 767px)" srcset="%base_url%/image/svensk-start.webp?w=900">

<img class="loadImg" src="%base_url%/image/svensk-start.webp?w=400&q=100" alt="start page svensk fastighetsbyrå">
</picture>
<br>

<div class="embed-container2">
<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRGethpzudlHQ9oX6rGdc15dQU_KTO93j8rPgRqTQs_J8nEWfhQcYNjszW73iYBqShCF319S8BuSExQ/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false" title="google sheet svensk fastighetsförmedling"></iframe>
</div>


Webbplatsen för Svensk Fastighetsförmedling hade "load"-tider på mellan 2 och 5.95 sekunder. Prestanda poängen för mobiler var mellan 58-76 poäng och 97-98 poäng för datorer. Till skillnad från Fastighetsbyrån och Länsförsäkringar fastighetsförmedling, använder sig Svensk Fastighetsförmedling av en interaktiv karta på sin mäklar-sida istället för bilder på städer där deras mäklarbyråer befinner sig. Svensk Fastighetsförmedling kan optimera prestandan för sin webbplats ännu mer genom att oanvänd CSS och Javascript reduceras och resurser som blockerar renderingen tas bort. Detta kan förbättra "load"-tiderna ännu mer och öka tidsbesparingarna för laddningstiderna. <br><br><br>

<picture>
    <source media="(min-width: 767px)" srcset="%base_url%/image/lans-start.webp?w=900&">
<img class="loadImg" src="%base_url%/image/lans-start.webp?w=400&q=100" alt="start page länsförsäkringar">
</picture>
<br>

<div class="embed-container2">
<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRGethpzudlHQ9oX6rGdc15dQU_KTO93j8rPgRqTQs_J8nEWfhQcYNjszW73iYBqShCF319S8BuSExQ/pubhtml?gid=586639532&amp;single=true&amp;widget=true&amp;headers=false" title="google sheet länsförsäkringar"></iframe>
</div>

"Load"-tiden för Länsförsäkringar fastighetsförmedling varierade mellan 2.35-4.06 sekunder. Utav de tre sidor som testades på webbplatsen var "till salu"-sidan den sida med flest resurser och sidan som var långsammast att laddas. Sidan använder både WEBP och JPEG-formaten. Prestanda poängen för mobiler var 41-52 poäng och 75-97 poäng för datorer. Precis som föregående webbplatser kan Länsförsäkringar fastighetsförmedling
reducera Javascript som inte används. För mobiler kan en tidsbesparing mellan 2.1 och 2-25 sekunder göras om oanvänd Javascript reduceras enligt Page Insight. Precis som ovanstående webbplatser kan sidan optimeras om bild-formaten ändras och om oanvänd CSS tas bort.<br><br>

##Sammanfattning

Det finns flera påverkande faktorer som saktar ner webbplatsernas laddningstider, och bilderna är en av de största bidragande faktorerna. Stora, högupplösta bilder, som bilden på Vadstena på Fastighetsbyråns webbplats påverkar laddningstiden och prestandan av webbplatsen avsevärt. För att förbättra laddningstiderna kan för stora bilder optimeras genom att formatet på de byts eller genom att verktyg används som komprimerar bilderna utan att kvaliten minskar. När filstorleken på bilderna minskas bidrar det till att de laddas snabbare när webbplatsen besöks av användare. Reduceringen av all oanvänd kod och minifieringen av CSS, JavaScript och HTML filer kan också hjälpa att förbättra laddningstiderna.<br><br>


Allt under två sekunder betraktas vanligtvis som en snabb laddningstid för en webbplats<sup>2, </sup><sup>3</sup>. Webbplatsens typ och komplexitet, mängden resurser som laddas och hastigheten på användarens internetanslutning är några av de faktorer som påverkar laddningstiden för webbplatser.<sup>4</sup> För de valda webbplatserna i denna rapport varierar laddningstiderna och baserat på dessa tider och antalet prestanda poäng från Googles Page Insights har jag rangordnat de enligt följande:<br><br>

1.Fastighetsbyrån - snabbast "load"-tid för start- och till salu-sida.<br>
2.Svensk Fastighetsförmedling - bäst prestanda poäng i överlag och speed index för mobiler.<br>
3.Länsförsäkringar fastighetsförmedling - snabbast "load"-tid för mäklar-sida och speed index för dator.<br>
<br>
Min gräns för absolut laddningstid satte jag på 2.9 sekunder efter ha läst "What Is a Good Page Load Time for SEO?"<sup>5</sup> och "Website Load Time in 2021: How Fast Is Fast Enough?"<sup>6</sup>. Med en absolut laddningstid på 2.9 sekunder skulle webbplatserna bli cirka 50% snabbare än alla andra webbplatser på internet<sup>5</sup>, och det var en gräns jag tyckte tre av Sveriges största mäklarbyråer kunde uppnå. Även om ingen av webbplatserna i denna rapport klarade av den utsatta laddningstiden för alla tre utvalda sidor, kändes ingen av webbplatserna långsamma eller "laggiga". Närmast att uppnå den utsatte laddningstiden var Fastighetsbyrån, med 2 av 3 sidor. Hade antalet resurser på Fastighetsbyråns mäklar-sida optimerats och bilden på Vadstena komprimeras så kanske även den sidan hade kunnat nå målet.   <br><br><br>

Rapport skriven av: Botan Mahmood

##Referenser

<sup>1</sup> https://pagespeed.web.dev/<br>
<sup>2</sup> https://www.portent.com/blog/analytics/research-site-speed-hurting-everyones-revenue.htm#:~:text=The%20first%205%20seconds%20of,(between%20seconds%200%2D5)<br>
<sup>3</sup> https://www.pingdom.com/blog/website-load-time-in-2020/<br>
<sup>4</sup> https://www.cloudflare.com/learning/performance/why-site-speed-matters/#:~:text=The%20amount%20of%20resources%20a,load%20time%2C%20to%20a%20webpage.<br>
<sup>5</sup> https://www.semrush.com/blog/how-fast-is-fast-enough-page-load-time-and-your-bottom-line/<br>
<sup>6</sup> https://www.pingdom.com/blog/website-load-time-in-2020/<br><br><br>


