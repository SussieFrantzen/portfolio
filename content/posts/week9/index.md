---
title: Take_a_Chance uge 9
categories: ["project", "ideas"]
tags: ["take a chance", "java"]
date: 2026-10-25
draft: false
weight: 1
series: [Take a chance]
series_order: 6
showauthor: true
authors:
- Sussie Frantzen
---

## Uge 9:

Nu kunne jeg begynde at kode så småt igen.
Men jeg fandt ud af min akitektur ikke var korrekt og jeg manglede en masse elementer til at få det hele til at spille sammen.
Jeg manglede service klasser, flere DAO, DTO'er, og havde ikke lavet Controllers og routes.
<br>
Selvfølgelig viste jeg der var ting der skulle kunne kalde metoderne og kommunikere op når det engang er til en frontEnd.
Men det der var specielt og gjorde den store ændring var hele mit spils logik.
<br>
>Ja min user story fortæller hvad jeg ønsker, men ikke hvor meget logik der ligger bag. 

<br>
Jeg fandt ud af jeg skulle have metoder der håndterede for hvems tur det er og hvad der skal afgøre, hvornår en tur er færdig.
<br>
 Hvad der sker, når der er trukket et kort med en bestemt type. Det blev hurtigt mere avanceret. 
<br>
Jeg havde også fået adgang til en ny API som kunne generere spørgsmålskort.


 Det betød at jeg skulle lave en måde, hvor den ikke gav dubletter ned i databasen. Jeg lavede nogle kriterier da det kunne blive voldsomme mængder fyldplads i database, hvis der ikke kom nogle kræv opsætninger.

### Jeg tog følgende beslutning:

•	Lav kun nye spørgsmål hvis masterbunken indeholder mindre end 20 kort inden for aldersgruppen.


•	Lav 10 nye spørgsmål hvis den samme User har spillet spillet før. Kortene kommer ind på den fælles masterbunke.


•	Masterbunken er fælles og user kan ikke tilføje spørgsmål til bunken. Det er spillet ved opstart der tjekker om det skal kalde metoden.


•	Der laves ikke flere spørgsmålskort hvis der er +200 kort inden for en aldersgruppe indenfor det given emne som masterbunken holder på.


•	Der dannes kun 10 kort max selvom der 2 spiller i samme alder. Men der kan godt dannes 10 kort mere i en anden aldersgruppe. (så spillet danner op mod 20 kort).


 Dette betød at jeg skulle lave en smule om i min entities. Da jeg skulle have en boolean ind der kunne skifte fra false til true, når en User spillede for første gang et spil. Tilføjelsen 



