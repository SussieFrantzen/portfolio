---
title: Take_a_Chance refelktioner og test
categories: ["project", "ideas"]
tags: ["take a chance", "java"]
date: 2026-10-29
draft: false
weight: 1
series: [Take a chance]
series_order: 8
showauthor: true
authors:
- Sussie Frantzen
---

## Markdown Reflektioner
Da jeg begyndte at sætte min markdown op med skemaet over mine endpoint og deres fejl håndtering fik jeg et andet overblik over fejl håndtering.

Hvis man søger for at lave fejlhåndtering og give klare beskeder kan man lettere forstå systemmmet og eventuelt kommende fejl vil kunne sættes i større perspektiv.

men det gav indsigt også i at der mange steder skal kaldes undervejs og metoder der skal samarbejde.

Jeg tænker der stadig er Endpoints der mangler at blive lavet, når systemmet bliver udviklet mere på.

## Reflektioner:
Jeg er bekendt med jeg ikke har fået den fulde forretningsforståelse ind i min akitektur endnu. Jeg har igennem mit projekt blevet klar over at det simple klasse-diagram jeg startede med var en underdrivelse. 


## Test:
Jeg begyndte at få lavet test klasser til mit projekt. Dette gav mig god mulighed for at teste forbindelse til min database. Men også mere indsigt i min kode og akitektur.


Jeg fandt frem til jeg i nærmeste fremtid skal have lavet lidt om på min opsætning. Jeg havde fået lavet den for fast i struktur, men den skulle være mere flexibel så det var lettere at teste. jeg fik rettet det for min UserDAO og UserService. 

Dette var mit problem: 
>  private final EntityManagerFactory emf =
            HibernateConfig.getEntityManagerFactory(); 

Jeg fandt ud af jeg skulle gøre sådan:

```
 private final EntityManager em;

    public UserDAO(EntityManager em) {
        this.em = em;
    }



 private final EntityManagerFactory emf;

    public UserService(){
        this.emf = HibernateConfig.getEntityManagerFactory();
    }

    public UserService(EntityManagerFactory emf){
        this.emf = emf;
    }
```
På den måde er det ikke bundet til en bestemt database når man skal teste. så kan man bruge en test database.

Jeg fandt ud af man kunne teste via Endpoints via http-client og lave test så man kunne tjekke metoder der ikke var klar ellers det var også rart at vide at når FrontEnd et tidspunkt kommer på virker Endpointsene.


