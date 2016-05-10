---
layout: book
title: Continous Delivery på 5 minuter
published: 2016-05-03
coverimage: img/cover-continous-delivery.png
featured: true 
preface: |
    Continuous Delivery – för dig närmare kunden 
    Continuous Delivery, CD, är en metodik som bygger på:
    individuellt ansvar för kvalitet,
    automatisk testning samt
    korta cykler med snabb och kontinuerlig återkoppling.
---------------------------------------------------------

# EN VANLIG DAG PÅ JOBBET ...

![](../img/en-dag-pa-jobbet.png)

**Behöver din organisation strama upp kvaliteten och leveranssäkerheten – och få nöjdare kunder på köpet?**

Då rekommenderar vi en närmare titt på Continuous Delivery – metodiken där
- stressnivån sjunker och utrymmet för kreativitet ökar
- det går snabbt att anpassa sig till ändrade förutsättningar och kund-
  önskemål
- dina utvecklare slipper gräva fram gamla problem som borde varit lösta
  för länge sen
- din organisation kan ge leveranslöften som kunden kan lita på • du tidigt kan ge kunden något att prova och ge 
  återkoppling på
- du alltid vet vad koden har för status: klar för leverans!
- teamet får snabbt bekräftat efter varje ändring av koden att allting fungerar
- du tidigt kan ge kunden något att prova och ge återkoppling på

Inte minst är Continuous Delivery en metodik som låter utvecklarna fokusera på att skriva bra kod; 
de vet ju att det som de levererar faktiskt fungerar tillsammans med andra delar av mjukvaran.

----------

# VAD INNEBÄR CONTINUOUS DELIVERY?

**Continuous Delivery, CD, är en metod som gör att mjukvaruorganisationer kan leverera 
nya versioner eller uppdateringar snabbt och löpande utan att drabbas av interna förseningar 
eller kvalitetsproblem.**

Metoden är till för team som samarbetar kring en gemensam mjukvaru- produkt eller -tjänst. 
Den bygger på ett arbets öde där varje utvecklare tar stort individuellt ansvar för kvaliteten på koden. 
Automatiska tester utförs omedelbart efter varje ändring eller komplettering av koden. Arbetet präglas 
av korta cykler och snabb återkoppling. Det gör att mjukvaran ständigt är testad och klar för skeppning. 
Därför behöver inte ny funktionalitet, förbättringar och bugg xar paketeras i stora uppdateringar utan 
kan levereras så fort de är klara.
Mottagaren eller kunden kan vara ett team inom samma organisation eller en affärspartner 
(som inte är slutanvändare av mjukvaran).

## Ständigt levererbar mjukvara

![](../img/cd-puzzle.png)

 > Notera att den slutliga produktionssättningen inte ingår i begreppet CD. När vi gör paketerad och 
   levererad mjukvara  kontinuerligt tillgänglig för slutanvändaren kallas det Continous Deployment 
   

# PRINCIPERNA FÖR CONTINUOUS DELIVERY

**Continuous Delivery innebär att den kod som produceras hela tiden och på alla nivåer befnner sig under 
kvalitetskontroll, främst genom automatisk testning. Koden ska så fort som möjligt testas i sin kontext 
och paketeras för att bli redo för leverans.**

### Individuellt ansvar för kvalitet

Huvudloopen i CD är den individuella utvecklarens arbete med kodändringar som byggs och testas innan 
de integreras med teamets övriga kodändringar. Arbetet bygger på tillit och laganda: varje utvecklare 
måste utföra sin del av arbetet på ett förutsägbart och noggrant sätt, utan att ta genvägar eller göra 
”fulhack” (läs gärna Clean Code på fem minuter).

### Automatisk kvalitetssäkring

För att kvalitetssäkringen ska  yta måste den automatiseras så mycket det går även om kodgranskning 
fortfarande har sin plats. Det för också det goda med sig att utvecklarna tillbringar minimalt med 
tid på kvalitets- kontrollen av varje leverans. En ytterligare fördel är att automatiseringen minskar 
risken för fel. När man tillämpar CD ska det alltid gå undan; till exempel bör testningen av nya 
kodändringar vara klara inom en timme.

### Korta cykler med snabb och kontinuerlig feedback

Här följer CD de sedvanliga principerna för Agile. CD handlar om att få ett komplext samarbete 
att  yta utan väntetider eller fel – som kugghjulen i ett väloljat maskineri.

Genom att kontinuerligt lägga till små ändringar som testas får teamen god insikt om hur långt 
de har kommit och tar därigenom en liten risk vid varje tillägg. Produkten kommer med stor 
sannolikhet att kunna sättas i produktion strax efter det att de senaste tilläggen gjorts i koden.

------

# CONTINOUS DELIVERY I PRAKTIKEN

**Continuous Delivery handlar om att bli duktig på att hantera kod, byggen, test och 
leveranser effektivt. Resultatet blir ett välsmort maskineri där man utvecklar produkten
inkrementellt med tillägg och rättningar i små steg. Produkten är hela tiden redo att levereras.**

![](../img/cd-in-practice.png)

> I en väl fungerande CD-organisation snurrar leveranshjulet (= den gråa cirkeln) hela tiden i hög hastighet.
  Notera hur de fyra disciplinerna – kod, byggen, test och leveranser – går igen på varje nivå. Man skulle 
  nästan kunna säga att CD har en fraktal struktur!
>  
> Den kod som har integrerats och hur testerna har utfallit visualiseras tydligt. Alla kan enkelt se vilka 
  tillägg som gjorts från backloggarna varje dag och hur testresultatet ser ut – dels för de nya funktionerna, 
  dels för de sedan tidigare existerande funktionerna.
>
> Minst en gång om da- gen är organisationen redo att skeppa en
  ny produktversion till kunden.  

En fungerande CD-organisation bygger på att
både individer och team behärskar fyra så kallade discipliner:

**kod** - (code) verktyg och processer för att lägga till ny kod samt hantera versioner.   
**byggen** – (build) verktyg och processer för att bygga koden i en produkt.  
**test** – (test) verktyg och processer för att hantera testkod tillsammans med 
kod för produkten samt automatisk test av produkten.  
**leveranser** - (delivery) förmågan att paketera mjukvaran och göra den tillgänglig för kunden.  
När organisationen har uppnått hög mognad inom disciplinerna uppkommer det sällan några negativa 
överraskningar vid integration och leverans.

-----

# UTVECKLAREN STÅR I CENTRUM I CONTINUOUS DELIVERY

![](../img/cd-developer.png)

> CD-konceptets minsta beståndsdel är den enskilde utvecklaren som behärskar de fyra disciplinerna.

**I Continuous Delivery eftersträvar man att utvecklaren har så effektiva verktyg och processer 
som möjligt för hantering av de tre disciplinerna kod, bygge och test. Möjligheten att få värdefull 
återkoppling gör att ut- vecklaren sporras till att jobba i snabba cykler och därigenom tillämpa 
den fjärde disciplinen: att leverera kodändringar så fort de är klara.**

Genom att alla jobbar på samma sätt  nns de senaste kodversionerna från övriga utvecklare tillgängliga 
hela tiden – testade och klara. Väntetiderna mellan olika delar av organisationen blir därigenom så 
korta som de någonsin kan bli. Via tydlig visualisering förstår alla i organisationen vad som är färdigt 
och hur bra de olika delarna av koden fungerar – enskilt och integrerat.

En tumregel för CD säger att en enskild leverans av kod inte ska behöva ta mer än en timme. 
Bygge och automatiska tester kommer snabbt att ge återkoppling om leveransen inte fungerar som det är tänkt.

