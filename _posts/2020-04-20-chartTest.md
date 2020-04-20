---
layout: post
title: MPAndroidChart med kaggle data
---
Jeg har de seneste par dage arbejdet på min datavisualisering i form af at afprøve et nyt library ved navn "MPAndroidChart." Dette
gjorde jeg for at få et sammenlignings grundlag til det andet visualiserings library jeg brugte "AndroidPlot." Jeg synes at de fungere meget
på samme vis, dog er der små forskelle som fks MP's måde at wrappe entry objekter på som jeg synes giver en smule ekstra arbejde men samtidig
giver dig et godt overblik over hvad for nogle entries du har og giver dig stylings muligheder på de enkelte samlinger af entries. Det
kan du også i AndroidPlot men du har ikke samme overblik over dine entries som du har i MPAndroidChart synes jeg.
<!--more-->
<br>
<br>
Jeg løb ikke ind i de store problemer med at få det til at fungere, udover at jeg selfølgelig lige skulle sætte mig ind i dokumentationen
og finde ud af hvordan jeg ville sortere mit data i forhold til at få det til at give mening på den chart jeg valgte. Samtidig skulle jeg også
finde en måde at få dataen hevet ud fra en CSV fil som også var et af mine andre læringsmål. Dette gjorde jeg ved hjælp af OpenCSV, som er
et andet library til android til at udtrække data fra CSV, link og implementation vil være længere nede i billede format.
<br>
<br>
Jeg valgte at hive denne data ind omkring elevers ydeevne til eksamen og hvordan andre parametre spiller ind, sådan som forældres uddannelse
og andre faktore. Jeg valgte så at sortere ud fra elevernes forældres uddannelse og så elevens præstation til eksamen. For at se om
forældrene havde nogen indflydelse i form af social arv. Så jeg tog gennemsnittet af elevernes score og delte dem op i 2 grupper. Elever
hvor forældrene har en bachelor, op i mod elever hvor forældrene har et lavere uddannelses niveau.
<br>
<br>

**Link til MPAndroidChart:** <br>
[https://github.com/PhilJay/MPAndroidChart](https://github.com/PhilJay/MPAndroidChart) <br>
**Link til OpenCSV:** <br>
[http://opencsv.sourceforge.net/](http://opencsv.sourceforge.net/)
<br>
<br>
**Mit view med min chart:** <br>
![](/images/chartTestView.PNG)
<br>
<br>
**Her er min onCreate metode som eksekvere mine metoder og sætter min chart ved instantiering:** <br>
![](/images/chartTestOnCreate.PNG)
<br>
<br>
**Min første metode som henter dataen ind fra CSV filen og kalder sortToEntry():** <br>
![](/images/chartTestGetData.PNG)
<br>
<br>
**Min sort metode som wrapper mine data class objekter til entry objekter:** <br>
![](/images/chartTestSort.PNG) <br>
**Min data class hvor jeg gemmer alt min data i:** <br>
![](/images/chartTestDataClass.PNG)
