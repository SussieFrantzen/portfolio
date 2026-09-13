---
title: Take_a_Chance uge 4
categories: ["project", "ideas"]
tags: ["take a chance", "java"]
date: 2026-09-13
draft: false
weight: 1
series: [Take a chance]
series_order: 4
showauthor: true
authors:
- Sussie Frantzen
---

## Uge 4:
I denne uge har jeg fået lavet et par få DAO metoder til User. således at der kan ske nogle kald til databasen.
<br>
Jeg har også forsøgt at finde api'er, lettere sagt end gjort.
<br>
Jeg fandt ud af at den form for api jeg gerne ville have haft til mit system krævede, en længere procudere at få adgang til har jeg valgt at fjerne us 2.

#### US2 – Vælg emne/bane
Som game-master vil jeg kunne vælge et emne eller en bane, så spillet kan tilpasses det ønskede faglige område.


Det lykkedes mig at få oprettet forbindelse efter flere forsøg til Gemini api.
som giver mig adgang til en LLM.
<br>
Jeg kom i tanke om en ret væsentlig US jeg havde glemt, den kom til at ligge øverst i priotet.

### US 19 - Opret profil
Som Bruger vil jeg kunne logge ind på en profil, så jeg kan vende tilbage til spil jeg har startet.
#### Acceptkriterier
•	Brugeren skal kunne oprette en profil med brugernavn og adgangskode.
<br>
•	Brugeren skal kunne logge ind med sine loginoplysninger.
<br>
•	Systemet skal give en fejlbesked, hvis brugeren indtaster forkerte loginoplysninger.
<br>
•	Brugernavnet skal være unikt, så to brugere ikke kan oprette en profil med samme brugernavn.
<br>
•	Adgangskoden skal gemmes sikkert og ikke som almindelig tekst i databasen.
<br>
•	Når brugeren er logget ind, skal systemet kunne genkende brugeren.
<br>
•	Brugeren skal kunne se og fortsætte spil, som brugeren tidligere har startet.
<br>
•	Hvis brugeren logger ud og senere logger ind igen, skal de tidligere gemte spil stadig være tilgængelige.
<br>
•	Brugeren skal kunne logge ud af sin profil.
