---
section: Materialtyper
title: Bidrag
order:
date: 2020-03-
tags:
- under arbete
- Bidrag
- Artikel
--- 

# Bidrag
Denna hjälptext ger kortfattade instruktioner för de vanligaste egenskaperna vid beskrivning av bidrag, t.ex. artiklar i tidskrifter eller kapitel i en monografi. För mer utförliga instruktioner, se de generella hjälptexterna för Adminmetadata, Instans och Verk, se innehållsförteckningen nedan. Det finns två mallar för bidrag, en för bidrag i tryckta publikationer och en för bidrag i elektroniska publikaioner. Hjälptexten ger instruktioner för båda typerna.

## Innehåll   

[Inledning](#inledning)

| [Adminmetadata](#adminmetadata) | [Instans](#instans) | [Verk](#verk) | 
| ----------- | ----------- |  ----------- |
| [Generell hjälptext för Adminmetadata](https://libris.kb.se/katalogisering/help/workflow-adminmetadata) | [Generell hjälptext för Instans](https://libris.kb.se/katalogisering/help/workflow-instance) | [Generell hjälptext för Verk](https://libris.kb.se/katalogisering/help/workflow-work) |
| | [Utgivningssätt](#utgivningssatt) | [Verkets titel](#verkets-titel) |
| | [Medietyp](#medietyp) | [Medverkan och funktion](#medverkan-och-funktion) |
| | [Bärartyp](#barartyp) | [Språk](#sprak) |
| | [Titel](#titel) |[Genre/form](#genre-form)|
| | [Upphovsuppgift](#upphovsuppgift) | [Klassifikation](#klassifikation)  |
| | [Utgivning](#utgivning)| [Ämne](#amne)|
| | [Anmärkning](#anmarkning) | [Innehållstyp](#innehallstyp) |
| | | [Sammanfattning av innehåll](#sammanfattning-av-innehall) |


## Inledning
Beskrivningen av ett bidrag innehåller följande tre delar:  
* [Adminmetadata](https://libris.kb.se/katalogisering/help/workflow-adminmetadata) - administrativa data om instansbeskrivningen, såsom kontrollnummer och beskrivningsnivå
* [Instans](https://libris.kb.se/katalogisering/help/workflow-instance) - instans kan också kallas utgåva eller manifestation. Exempel på egenskaper under Instans för ett bidrag är titel, upphov och utgivning.
* [Verk](https://libris.kb.se/katalogisering/help/workflow-work) – återger egenskaper för det abstrakta verket såsom medverkan och funktion, ämne, klassifikation, språk och innehållstyp. Verksbeskrivningen ligger under rubriken Instans av verk.

Om bidraget är publicerat i flera olika publikationer och man vill beskriva det bör man skapa en beskrivning för varje publicering.

Många av egenskaperna finns redan i mallarna för  Bidrag, andra kan behöva läggas till. För instruktioner om att lägga till eller ta bort egenskaper, länka till entitet, skapa lokal entitet och om hur formuläret fungerar i övrigt, se Redigering i vänstermenyn. 

För information om katalogiseringsregler och Librispraxis, [se Anvisningar för katalogisering - RDA](http://www.kb.se/rdakatalogisering/ "Anvisningar för katalogisering - RDA") samt [se RDA Toolkit](https://access.rdatoolkit.org/). 

[Se även instruktionsfilmer på KB:s Youtubekanal](https://www.youtube.com/playlist?list=PLZVkEICvA5-GRT2oJQmLgq_2Pksx6zYPy).

## Adminmetadata
[Använd generell hjälptext för Adminmetadata](https://libris.kb.se/katalogisering/help/workflow-adminmetadata).
* Kontrollera beskrivningsnivån. I mallen är standardvärdet Biblioteksnivå (normalvärde för Librisbiblioteken). 

## Instans
För att lägga till egenskaper under Instans, klicka på plustecknet i redigeringsvyn (den stora runda plusikonen under Verktygsikonen) - Lägg till egenskaper under: Tryck (för bidrag i tryckt publikation) eller Elektronisk (för bidrag i elektronisk publikation). Sök fram egenskapen och välj den genom att klicka på plustecknet vid egenskapens namn. 

### Utgivningssatt
* Utgivningssätt (issuanceType)  
  Välj från lista:  
  ```Del av sammansatt resurs```

### Medietyp
* Medietyp (mediaType/Mediatype = 337 #b)  
  Länka till entitet.
  </br>```Exempel:```
  * ```omedierad, n``` (bidrag i tryckt publikation)
  * ```dator, c ``` (bidrag i elektronisk publikation)
  
### Barartyp
* Bärartyp (carrierType/CarrierType = 338 #b)  
  Länka till entitet:
  </br>```Exempel:```
  * ```volym, nc``` (bidrag i tryckt publikation)
  * ```onlineresurs, cr``` (bidrag i elektronisk publikation) 
  
  För bidrag i elektronisk publikation:
  
    Om koden "r" (= fjärranslutning) behövs i 007/01 (= särskild bärarbeteckning) för bibliotekets lokala system, länka till entiteten:</BR>
  ```Onlineresurs, r```</BR>
  
  Om koden "o" (= onlineutgåva) behövs i 008/23 (= form för manifestationen) för bibliotekets lokala system, länka till entiteten:</br>
  ```Onlineutgåva, o```</BR>
  
### Titel 
#### Huvudtitel    
* Har titel/Titel/Huvudtitel (hasTitle/Title/mainTitle = 245 #a)</br>
  ```Exempel: Herrgårdsbyggnader i Mälardalen under 1700- och 1800-talet```
* Har titel/Titel/Övrig titelinformation (= Undertitel) (hasTitle/Title/subtitle = 245 #b)  
   ```Exempel: när, var och av vem?```

För att ange föredragen titel, t.ex. om bidraget är översatt, se [Verkets titel](#verkets-titel).  

#### Varianttitel
* Har titel/Varianttitel/Huvudtitel (hasTitle/VariantTitle/mainTitle = 246 #a)

#### Delbeteckning och deltitel
* Har titel/Titel/Har del/Titeldel/Delbeteckning (hasTitle/Title/hasPart/TitlePart/partNumber = 245 #n)
* Har titel/Titel/Har del/Titeldel/Deltitel (hasTitle/Title/hasPart/TitlePart/partName = 245 #p)
  
#### Parallelltitel  
* Har titel/Parallelltitel/Huvudtitel (hasTitle/ParallelTitle/mainTitle = 246 1/1 #a)
* Har titel/Parallelltitel/Övrig titelinformation (hasTitle/ParallelTitle/subTitle = 246 1/1 #b)
     
### Upphovsuppgift
* Upphovsuppgift (responsibilityStatement = 245 #c)<br/>
  ```Exempel: Johan Ahlner, Karin Kjellgren```
  
### Utgivning  
* Utgivning (publication)  
  Välj typ från lista. För bidrag, använd Primär utgivning. 
 
#### Utgivningsland  
* Land (country = 008/15-17)  
  Länka till entitet.  
  ```Exempel: Sverige (sw)``` 
    
#### År
  * Primär utgivning/Utgivning/År (date = 008/07-10, 264 -/1 #c)<br/>
År får endast innehålla siffror (0-9) och bokstaven u.

### Anmarkning
* Anmärkning/Anmärkning/Benämning (hasNote/Note/label = 500 #a)<br/>

### Är del av
Här anges värdpublikationen, d.v.s. den publikation som bidraget ingår i. I första hand länkar man till värdpublikationen men om den inte har någon beskrivning i Libris kan den beskrivas som lokal entitet.<br/> 

I Libris rekommenderas att man för bidrag alltid länkar till eller beskriver årsbokens/tidskriftens huvudpost, även när en årsboksårgång eller ett tidskriftshäfte har en monografisk/tematisk karaktär (med egen, distinkt titel, fullständig titelsida och så vidare eller med en tematitel). Om så önskas kan tematiteln eller motsvarande anges som serieuppgift i bidragsposten.<br/>
* Seriemedlemskap/Seriemedlemskap/Serieuppgift</br>
```Exempel: Trädgårdar och parker : historia, dagsläge``` 

I monografiposten som beskriver årsboksårgången eller tidskriftshäftet kan en förklarande fras anges i en anmärkning. Det gör det lättare för användarna att hitta artiklar.<br/>
* Anmärkning/Anmärkning/Benämning (hasNote/Note/label = 500 #a)<br/>
```Exempel: Artiklar ur detta häfte söks i LIBRIS via Bebyggelsehistorisk tidskrift``` 

#### Länka till värdpublikationen
* Är del av (isPartOf = 773)<br/>
Sök fram beskrivningen av värdpublikationen i Lägg till entitet.<br/>
Länka till värdpublikationen.

#### Beskriva värdpublikationen som lokal entitet
I Är del av, lägg till Instans som lokal entitet. Lägg till egenskaper för värdpublikationen under Instans. 

###### Värdpublikation med primär medverkan
* Instans av Verk/Verk/Medverkan och funktion/Primär medverkan/Agent/Agent<br/>
Lägg till egenskapen Instans av verk och skapa Verk som lokal entitet. Under Verk, lägg till egenskapen Medverkan och funktion och välj typ Primär medverkan. Under Agent, lägg till Agent som lokal entitet.<br/> 
Skriv in uppgiften under Benämning.<br/>
  ```Exempel:```
  * ```Carlsson, Magnus```
  * ```Sverige. Socialtjänskommittén```
  * ```International Congress on Military History (26 : Stockholm : 2000)```
* Instans av Verk/Verk/Medverkan och funktion/Primär medverkan/Funktion<br/>
Länka till entiteten:<br/>
```Författare, aut```

##### Övriga egenskaper för värdpublikationen
* Identifikator (identifiedBy = 773 #z ISBN, 773 #x ISSN)<br/>
Lägg till egenskapen Identifikator. Välj typ och ange värdpublikationens identifikator (om sådan finns) i Värde.<br/>
* Har titel/Titel/Huvudtitel (hasTitle/Title/mainTitle = 773 #t)<br/>
Lägg till egenskapen Har titel. Välj typ Titel. 
Om värdpublikationen är en monografi, ange huvudtitel och eventuellt övrig titelinformation åtskild med interpunktion i Huvudtitel. Om Övrig titelinformation ska anges eller inte är en bedömningsfråga. Huvudtiteln kan i vissa fall vara ganska intetsägande medan övrig titelinformation ger tydligare information om innehållet.</br>
```Exempel: Historia - ekonomi - forskning : fem rapporter om idrott : rapporter till Idrottsutredningen```<br/>
Om värdpublikationen är en årsbok eller tidskrift, ange nyckeltiteln (om värdpublikationen har ISSN), annars huvudtiteln<br/>
```Exempel: Karolinska förbundets årsbok```
* Uppgift om produktion, utgivning, distribution och eller tillverkning (provisionActivityStatement = 773 #d)<br/>
Lägg till egenskapen ppgift om produktion, utgivning, distribution och eller tillverkning.<br/>
Om värdpublikationen är en monografi, ange utgivningstiden för monografin.<br/>
```Exempel: 2002```
* Serieuppgift (seriesStatement = 773 #k)
Om värdpublikationen är en monografi som ingår i en serie, lägg till serieuppgift om så önskas.<br/> 
```Exempel: Statens offentliga utredningar, 0375-250X ; 1998:33```

#### Placering i värdpublikationen
* Del (part = 773 #g)<br/>
Här anges i vilken årgång och/eller nummer av värdpublikationen bidraget är publicerat och/eller paginering.

###### Bidrag i årsbok eller tidskrift
Ange årgång och/eller nummer samt paginering.<br/>
  ```Exempel:```
  * ```2000, sidorna 215-217```
  * ```2002(87):2, sidorna 145-172```
  
När en årgång består av flera nummer anger vi också numret enligt exemplet: "2002(87):2" (följer den standard som beskrivs i Sten Hedbergs Bibliografiska referenser), även om årgången har genomgående paginering.

###### Bidrag i monografi
Ange paginering.<br/>
```Exempel: Sidorna 379-390```

## Verk 
För att lägga till egenskaper under Instans av Verk, klicka på plustecknet till höger om Instans av Verk och verkstypen. Sök fram egenskapen och välj den genom att klicka på plustecknet vid egenskapens namn.

[Läs mer om egenskaperna under den generella beskrivningen av Verk](https://libris.kb.se/katalogisering/help/workflow-work)

### Instans av verk 
* Instans av verk/Text (instanceOf/Work/Text) 

### Verkets titel 
Ange vid behov den föredragna titeln för verket här. [Följ anvisningarna under Konstruera sökingångar för verk och uttryck i Anvisningar för katalogisering - RDA.](http://www.kb.se/rdakatalogisering/Anvisningar/Allmanna-anvisningar/Sokingangar-for-verk-och-uttryck/) 
Ange föredragen titel för översättningar, för verk som har givits ut under olika titlar på samma språk eller när samma titel har använts för olika verk.

#### Verkets titel - verk med primär medverkan
* Har titel/Titel/Huvudtitel (hasTitle/Title/mainTitle = 240 1/0 #a)</BR> 
"Originaltitel" för ett verk med Medverkan och funktion/Primär medverkan anges här.

#### Verkets titel - verk utan primär medverkan
*	Uttryck av/Verk/Har titel/Titel/Huvudtitel (expressionOf/Work/hasTitle/Title/mainTitle (= 130 #a)  

### Medverkan och funktion
[Följ instruktioner i hjälptexten Relationer till Agent](https://libris.kb.se/katalogisering/help/workflow-agent-org-instance) 

* Medverkan och funktion/Primär medverkan/Agent/Person</br>
(contribution/PrimaryContribution/agent/Person = 100 1/- #a)

* Medverkan och funktion/Primär medverkan/Funktion</br>
(contribution/PrimaryContribution/role = 100 #4)

* Medverkan och funktion/Medverkan/Agent/Person</br>
(contribution/agent/Person = 700 1/- #a)

* Medverkan och funktion/Medverkan/Agent/Organisation (710 2/-)</br>

* Medverkan och funktion/Medverkan/Agent/Jurisdiktion (710 1/-)</br>
 
#### Sprak 
* Språk (language = 008/35-37)</BR>
  Länka till entitet.  
  ```Exempel: svenska (swe)``` 
  För att ange originalspråk för ett översatt verk, se Originalversion/Verk/Språk under [Översättning](#oversattning).
  
#### Översättning  
För en artikel som är/innehåller en översättning, lägg till:  
* Anmärkning: Språk (marc:LanguageNote = 041 i1: 1)  
  Ange om resursen är/innehåller en översättning.  
  
* Originalversion/Verk/Språk (originalversion/Work/language = 041 #h)  
  Ange originalspråk här. Klicka på plustecknet vid Instans av Verk, välj Originalversion, klicka på plustecknet vid Originalversion, välj Skapa lokal entitet. Skriv Verk i rutan för Skapa lokal entitet och välj * Verk. Lägg till Språk under verk. Sök fram språkentiteten och länka.  
  ```Exempel: engelska (eng)```  

### Genre form 
För utförliga anvisningar om hur man anger genre/form, [se hjälptexten Verk](https://libris.kb.se/katalogisering/help/workflow-work#genre): Genre form.
    
### Klassifikation  
För anvisningar om hur man anger klassifikation, [se hjälptexten Verk](https://libris.kb.se/katalogisering/help/workflow-work#klassifikation): Klassifikation.
 
### Amne  
* Ämne  
  Länka  i första hand till entiteter för ämnesord. [Följ instruktionerna under Ämnesord i Libris](https://libris.kb.se/katalogisering/help/workflow-general-sh).   
 
### Innehallstyp
 * Innehållstyp/Innehållstyp (contentType/ContentType = 336 #b)   
  Länka till entiteten:</BR>
  ```Computer program, cop (= datorprogram)```
  
### Sammanfattning av innehall
 * Sammanfattning av innehåll/Sammanfattning/Benämning (summary/Summary/label = 520 #a)</BR>
Lägg till Sammanfattning av innehåll. Välj Sammanfattning av innehåll. Lägg till Sammanfattning. 
</BR>Skriv in uppgiften under Benämning.
 <br/>```Exempel: Om en planerad fredskonferens som aldrig kom till stånd```<br/> 
 * Typ av sammanfattning/typ av innehållsbeskrivning (marc:summaryType = 520 ind1)  
 Sök fram och lägg till Typ av sammanfattning. Välj typ från lista.  
 ```Exempel: Ej preciserad```
