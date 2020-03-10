---
layout: post
title: Første udkast af TrendLog appen
---
Jeg har de seneste par dage arbejdet på at få lavet noget jeg kunne vise til vores PO, i form af den app han godt kunne tænke sig.
Det er en app som skal kunne logges ind på af TrendLogs kunder og vise dem et dashboard som tilhører deres fabrik. På dette dashboard
vil man kunne se nogle grafer og statistikker over produktionsinformation så der fks kan optimeres bedre på et produkt bånd eller noget
i den stil.
<!--more-->
<br>
<br>
Jeg er startet blødt ud med login delen som jeg gerne ville prøve at lave med noget databinding for at lærer hvordan dette fungere i
android. Til at starte med så jeg en masse af googles egen tutorials om hvordan et bud på implementation af dette kunne se ud,
det har været nogle super gode videoer som er virkeligt forklarende. De er gode til at gå i deltaljerne om hvorfor det de gør er smart
og hvad der sker i baggrunden.
<br>
<br>
Jeg kører min TrendLog app med UI designet "Single Activity" som vil sige jeg kun benytter mig af en enkelt activity som hoster et eller
flere fragment views og kan navigere igennem dem via actions dette er også anbefalet af google. Samtidig med dette er min indre
struktur baseret på MVVM. Jeg bruger viewmodels til at sørge for når mit view bliver dræbt ved fks skærm rotation. Så vil alt mit data
stadig være tilgængeligt i min viewmodel til mit UI når det bliver instantieret igen. Jeg vedhæfter nogle billeder nedenunder til
illustration af det jeg har fortalt om og samtidig nogle links til de guides jeg har benyttet.
<br>
<br>
**GUIDES:** <br>
Herunder benyttede jeg mig af disse sektioner: App Navigation, App Architechture <br>
[https://classroom.udacity.com/courses/ud9012](https://classroom.udacity.com/courses/ud9012) <br>
Første version af mit login UI: <br>
![](/images/trendlogAppV1.jpg) <br>
Her er en illustration af min MVVM struktur: <br>
![](/images/architechtureMVVM.PNG)
