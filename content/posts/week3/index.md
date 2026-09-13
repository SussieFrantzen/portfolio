---
title: Take_a_Chance uge 3
categories: ["project", "ideas"]
tags: ["take a chance", "java"]
date: 2026-09-06
draft: false
weight: 1
series: [Take a chance]
series_order: 3
showauthor: true
authors:
- Sussie Frantzen
---

## Uge 3:

I denne uge redigerede jeg ydeligere på mit klasse diagram.
og begyndte at få lavet nogle flere af java klasserne med lombok og jpa.

Da US ikke har været helt klar har jeg ikke fået lavet meget kode endnu. Men har lavet en metode til terningen da den var basic.
samt er coin også lavet med en enkelt metode.


![klassediagram_2](klassediagram_2.png)


## US story i den rækkefølge de vil blive håndteret efter:

### US1 – Vælg antal spillere
Som game-master vil jeg kunne vælge antallet af spillere, så jeg kan oprette spillet med det ønskede antal deltagere.

#### Acceptkriterier:
•	På startskærmen kan game-master åbne spillerindstillinger.
<br>
•	Game-master kan angive antallet af spillere.
<br>
•	Systemet validerer, at antallet af spillere er inden for det tilladte antal.
<br>
•	Spillet kan først startes, når et gyldigt antal spillere er valgt.

### US9 – Angiv spillerens niveau/alder
Som game-master vil jeg kunne angive hver spillers alder eller faglige niveau, så spillet kan tilpasses den enkelte spiller.

#### Acceptkriterier:
•	Game-master kan angive alder eller niveau for hver spiller.
<br>
•	Oplysningerne gemmes sammen med spilleren.
<br>
•	Niveauet bruges til at tilpasse relevante spørgsmål/kort.

### US2 – Vælg emne/bane
Som game-master vil jeg kunne vælge et emne eller en bane, så spillet kan tilpasses det ønskede faglige område.

#### Acceptkriterier:
•	Game-master kan vælge "Vælg bane/emne" fra startmenuen.
<br>
•	Systemet viser de tilgængelige emner/baner.
<br>
•	Game-master kan vælge ét emne/bane.
<br>
•	Det valgte emne anvendes i det efterfølgende spil.

### US7 – Se spillebrikker
Som spiller vil jeg kunne se min egen og de andre spilleres placeringer på spillepladen, så jeg kan følge spillets udvikling.

#### Acceptkriterier:
•	Hele den relevante spilleplade vises.
<br>
•	Alle aktive spilleres brikker vises.
<br>
•	Det er muligt at identificere, hvilken brik der tilhører hvilken spiller.
<br>
•	Brikkernes placering opdateres efter en spillers tur.


### US4 – Udfør sin tur
Som spiller vil jeg kunne se, når det er min tur, og hvilke handlinger jeg kan foretage, så jeg ved, hvad jeg skal gøre.

#### Acceptkriterier:
•	Den aktive spiller fremhæves tydeligt.
<br>
•	Spilleren kan se sine tilgængelige handlinger.
<br>
•	Terning/spinner eller andre relevante spilleelementer kan aktiveres, når det er spillerens tur.
<br>
•	Andre spillere kan se, hvem der har tur.

###  US12 – Kast terning
Som spiller vil jeg kunne aktivere en terning, så systemet kan generere et tilfældigt antal øjne.

#### Acceptkriterier:
•	Spilleren kan aktivere terningen, når den er relevant.
<br>
•	Terningen viser en animation.
<br>
•	Systemet genererer et tilfældigt resultat.
<br>
•	Resultatet vises tydeligt.

### US14 – Flyt spillerbrik
Som spiller vil jeg kunne se min brik flytte sig efter mit terning-/spinnerresultat, så jeg tydeligt kan se resultatet af min tur.

#### Acceptkriterier:
•	Spillerens resultat bestemmer, om og hvor langt brikken flyttes.
<br>
•	Brikken animeres eller flyttes synligt på spillepladen.
<br>
•	Spillerens point/status opdateres efter bevægelsen.
<br>
•	Hvis spilleren mister sin tur, bliver brikken stående.
<br>
•	Systemet viser tydeligt, hvis spilleren mister sin tur.

### US15 – Vælg retning
Som spiller vil jeg kunne vælge retning, når spillepladen deler sig i flere mulige veje, så jeg selv kan bestemme, hvilken vej min brik skal bevæge sig.

#### Acceptkriterier:
•	Systemet viser de mulige retninger.
<br>
•	Spilleren kan vælge mellem de tilgængelige retninger.
<br>
•	Den valgte retning fremhæves.
<br>
•	Spilleren kan bekræfte sit valg.
<br>
•	Brikken fortsætter derefter i den valgte retning.


### US8 – Træk tilfældigt kort
Som spiller vil jeg automatisk få tildelt et tilfældigt kort, når jeg lander på et felt, der udløser et kort, så spillet kan fortsætte med en tilfældig udfordring eller handling.

#### Acceptkriterier:
•	Systemet registrerer, når en spiller lander på et kortfelt.
<br>
•	Systemet vælger et tilfældigt kort fra den relevante kortbunke.
<br>
•	Det valgte kort vises for spilleren.
<br>
•	Korttypen afhænger af feltet og spillets indstillinger.


### US5 – Se spørgsmål-/chancekort
Som spiller vil jeg kunne se det kort, jeg har trukket, så jeg kan læse og forstå spørgsmålet eller handlingen.

#### Acceptkriterier:
•	Når spilleren lander på et relevant felt, vises kortet.
<br>
•	Kortet vises tydeligt på skærmen.
<br>
•	Kortet indeholder det relevante spørgsmål eller den relevante handling.


### US6 – Besvare kort
Som spiller vil jeg kunne besvare et spørgsmålskort, så mit svar kan registreres i spillet.

#### Acceptkriterier:
•	Spilleren kan vælge eller indtaste et svar.
<br>
•	Spilleren kan trykke på en "Besvar"-knap.
<br>
•	Systemet registrerer spillerens svar.
<br>
•	Systemet kan afgøre, om svaret er korrekt, hvis spillet kræver det.


### US18 – Tilpas kort efter niveau
Som spiller vil jeg få spørgsmålskort, der passer til mit valgte niveau eller min alder, så spillets faglige udfordringer passer til mig.

#### Acceptkriterier:
•	Spillerens alder/niveau er registreret.
<br>
•	Når spilleren lander på et kortfelt, identificerer systemet spillerens niveau.
<br>
•	Systemet vælger kun relevante kort eller tilpasser sværhedsgraden.
<br>
•	Det valgte kort vises derefter for spilleren.


### US11 – Kast mønt
Som spiller vil jeg kunne aktivere en mønt, så systemet tilfældigt kan vælge mellem møntens to udfald.

#### Acceptkriterier:
•	Spilleren kan aktivere mønten.
<br>
•	Mønten animeres som om den bliver kastet.
<br>
•	Systemet genererer tilfældigt et udfald.
<br>
•	Udfaldet vises tydeligt for spilleren.

### US13 – Stem på startspiller
Som spiller vil jeg kunne stemme på, hvilken spiller jeg tror starter spillet, så jeg kan deltage i spillets startmekanisme.

#### Acceptkriterier:
•	Funktionen er tilgængelig i "Take a Chance".
<br>
•	Alle spillere kan afgive én stemme.
<br>
•	Spillerne slår med terningen for at afgøre, hvem der faktisk starter.
<br>
•	Ved samme antal øjne starter den yngste spiller.
<br>
•	Spillere, der har gættet korrekt, får den beskrevne fordel ved start.

### US16 – Se skæbneskjold
Som spiller vil jeg kunne se, når jeg har et skæbneskjold, så jeg ved, at jeg har en beskyttelse til rådighed.

#### Acceptkriterier:
•	Når spilleren modtager et skæbneskjold, vises et ikon.
<br>
•	Ikonet vises ved spillerens navn.
<br>
•	Ikonet forbliver synligt, indtil skjoldet bliver brugt.

### US17 – Anvend skæbneskjold
Som spiller vil jeg automatisk være beskyttet af mit skæbneskjold, når jeg udsættes for en negativ hændelse, så jeg ikke mister de point eller effekter, som hændelsen ellers ville påvirke.

#### Acceptkriterier:
•	Systemet registrerer, om spilleren har et aktivt skæbneskjold.
<br>
•	Skjoldet aktiveres automatisk ved en relevant negativ hændelse.
<br>
•	Spilleren påvirkes ikke af hændelsen.
<br>
•	Skæbneskjoldet fjernes efter brug.
<br>
•	De øvrige spillere påvirkes efter spillets regler.

### US10 – Se faglig feedback
Som spiller vil jeg efter spillets afslutning kunne se feedback på min faglige præstation, så jeg kan se, hvilke emner jeg har styr på, og hvilke jeg bør træne mere.

#### Acceptkriterier:
•	Der vises en resultatside, når spillet afsluttes.
<br>
•	Spilleren kan se sin samlede præstation.
<br>
•	Resultatet viser relevante faglige områder.
<br>
•	Systemet angiver eventuelt områder, hvor spilleren bør træne mere.


### US3 – Gem spil
Som game-master vil jeg kunne gemme et aktivt spil, så spillet kan fortsættes på et senere tidspunkt.

#### Acceptkriterier:
•	Game-master kan logge ind under et aktivt spil.
<br>
•	Spillets aktuelle status gemmes.
<br>
•	Spillernes placeringer, point og relevante spilstatusser gemmes.
<br>
•	Et gemt spil kan indlæses igen.


