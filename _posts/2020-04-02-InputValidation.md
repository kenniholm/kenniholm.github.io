---
layout: post
title: Input Validation
---
Så kom tiden til at implementere input validation i min produkt app. Jeg tænkte til at starte med jeg rigtigt gerne kunne tænke mig real
time form validation. Sådan så når brugeren taster en karakter ind vil der ved hjælp af et observer pattern hele tiden holdes øje med
formen og om den opretholder den rigtige format.
<br>
<!--more-->
<br>
Jeg valgte at implementere det via en library fordi der findes så mange smarte. Jeg benyttede mig af noget der hedder vvalidator
som jeg også vil credit længere nede i mit post hvis man har lyst til at tjekke det ud. Selve implementationen gik meget gnidningsfrit,
det er ret simpelt at sætte op. Du implementere en form som tager forskellige input objekter som er dine individuelle input felter.
I disse individuelle inputs kan du så implementere forskellig validation logik.
<br>
<br>
**Her er nogle billeder af hvordan det ser ud for brugeren:**
<br>
![](/images/validationUI.jpg)
<br>
**Her er et billede af hvordan det fungere i koden:**
<br>
![](inputValidator.PNG)
