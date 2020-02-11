---
layout: post
title: Videreudvikling på Testapp
---
Jeg besluttede mig for at lærer at bruge "intents" for at kunne kalde andre activities, samtidig med at kunne sende data<br>
videre fra et view til et andet. I det her tilfælde gjorde jeg det med en string som jeg ville lave et lille pop-up besked med også kaldet en "Toast" i android, bare for at afprøve om jeg kunne få det til at virke.<br>
<!--more-->
Jeg brugte en tutorial fra google som også forklarede en masse best practices omkring blandt andet at bruge "lateinit" til<br>
at finde sine views via ID. Hvis man ikke benyttede sig af det i store applikationer som skulle finde mange views eller tage mange kliks,
kunne den komme til at lagge og blive langsom.<br>
Her er det google kursus jeg tog for at komme godt igang med intents og best practices:<br>
https://classroom.udacity.com/courses/ud9012 <br>
<br>
Billeder af det kode jeg kom frem til for at opnå mit mål: <br>
Activity 1: <br>
![](/images/Mainact.PNG) <br>
Activity 2: <br>
![](/images/Mainactt2.PNG)
