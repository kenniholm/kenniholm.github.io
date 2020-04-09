---
layout: post
title: Dashboard/Options menu og logout.
---
Idag og igår har jeg blandt andet arbejdet med at få lavet logout til min applikation, sådan så når man klikkede på androids egen tilbage 
knap så ville den spørge brugeren om man vil logge ud og så skal brugeren confirm for at bekræfte det ikke var et fejl klik. Dette
i sig selv var meget enkelt, jeg skulle bare tilføje en callback metode og så tager android sig af resten, det vil der være et billede af
i bunden.
<br>
<!--more-->
<br>
Derefter besluttede jeg mig for jeg også ville have en toolbar til at have forskellige elementer til mit dashboard som brugeren kan vælge
imellem. Jeg startede med at implementere en options menu i XML og derefter prøve at få mit dashboard til at vise en toolbar. Da jeg kører
med "No toolbar" tema i min app er det skjult pr default. Det tog mig lidt tid at få den til at vise den toolbar fordi den metode jeg
skulle bruge var kun til rådighed i en activity. Jeg fandt så ud af efter en del google søgninger at man kunne smart caste sin activity i
sin fragment og igennem sin host activity få lov at sætte en toolbar i min dashboard fragment, dette har jeg også billede af i bunden.
<br>
<br>
Dernæst tilføjede jeg mit første item til min lille optionsmenu jeg har lavet i XML, og få det vist på skærmen med funktionalitet når
du klikker på "Logout." Når dette gøres prompter den dig ligesom på tilbage knappen, om du er sikker på dit valg af logout, hvor der igen
kan svares "Yes" eller "No."
<br>
<br>
Udover den nye funktionalitet, ville jeg også gerne tilføje lidt extra input validation i form af forskellige tegn som kan benyttes
til sql injection og andre ondsindet angreb. Derfor skulle jeg lærer at bruge vvalidator's custom assertion metode som tog lidt tid
at forstå hvordan det virkede. Men det virker rigtigt fint nok og brugeren bliver prompted realtime hvis de benytter nogle af disse tegn
i deres display navn. Dette er der også billede af i bunden.
<br>
<br>
**Callback metode til androids tilbageknap:** <br>
![](/images/logout2.PNG)
<br>
<br>
**Logout logik:** <br>
![](/images/logout1.PNG)
<br>
<br>
**Sætter min toolbar fra mit view's xml fil med smart cast:** <br>
![](/images/toolbar1.PNG)
<br>
<br>
**Inflater min menu jeg har lavet i XML, det gør jeg ved at override den eksisterende.** <br>
**Plus jeg sætter logikken for hvad der sker ved klik af logout i menuen:** <br>
![](/images/toolbar2.PNG)
<br>
<br>
**Billede af mit Dashboard so far, med toolbar og åben menu i toppen:** <br>
![](/images/menuScreen.PNG)
<br>
<br>
**Her ses den ekstra input validation logik jeg tilføjede med costum assert fra vvalidator:**
![](/images/customAssert.PNG)
