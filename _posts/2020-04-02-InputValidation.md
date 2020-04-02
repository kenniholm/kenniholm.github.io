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
Jeg valgte at implementere det via et library fordi der findes så mange smarte derude og så kan jeg undgå så meget
boiletplate kode som muligt og stadig opnå det jeg gerne ville. Jeg benyttede mig af noget der hedder vvalidator
som jeg også vil credit længere nede i mit post hvis man har lyst til at tjekke det ud. Selve implementationen gik meget gnidningsfrit,
det er ret simpelt at sætte op. Du implementere en form som tager forskellige input objekter som er dine individuelle input felter.
I disse individuelle inputs kan du så implementere forskellig validation logik. Jeg kunne også implementere mine binding objekter diretke ind i dette library, da input felterne kunne tage et EditText objekt ind i parametrene, hvilket også var super vigtigt
med min applikation. <br>
Jeg sætter disableSubmiet = true for at sørge for min submit knap som jeg definere længere nede ikke kan eksekveres hvis ikke formattet
overholdes.
<br>
<br>
**Link til vvvalidtor:**
<br>
[https://github.com/afollestad/vvalidator](https://github.com/afollestad/vvalidator)
<br>
**Her er nogle billeder af hvordan det ser ud for brugeren:**
<br>
![](/images/validationUI.jpg)
<br>
**Her er et billede af hvordan det fungere i koden:**
<br>
![](/images/inputValidator.PNG)
