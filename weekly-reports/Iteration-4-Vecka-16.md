# Veckorapporter
***

* [Iteration 0](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/weekly-reports/Iteration-4-Vecka-16.md#iteration-0-vecka-12)
* [Iteration 1](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/weekly-reports/Iteration-4-Vecka-16.md#iteration-1-vecka-13)
* [Iteration 2](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/weekly-reports/Iteration-4-Vecka-16.md#iteration-2-vecka-14)
* [Iteration 3](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/weekly-reports/Iteration-4-Vecka-16.md#iteration-3-vecka-15)
* [Iteration 4](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/weekly-reports/Iteration-4-Vecka-16.md#iteration-4-vecka-16)
* [Iteration 5](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/weekly-reports/Iteration-4-Vecka-16.md#iteration-5-vecka-17)
* [Iteration 6](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/weekly-reports/Iteration-4-Vecka-16.md#iteration-6-vecka-18)
* [Iteration 7](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/weekly-reports/Iteration-4-Vecka-16.md#iteration-7-vecka-19)
* [Iteration 8](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/weekly-reports/Iteration-4-Vecka-16.md#iteration-8-vecka-20)
* [Iteration 9](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/weekly-reports/Iteration-4-Vecka-16.md#uppgifter-iteration-9)
* [Iteration 10](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/weekly-reports/Iteration-4-Vecka-16.md#iteration-10-vecka-22)

***

### Iteration 0 (Vecka 12)

### Analys av föregående iteration
Ingen föregående iteration.

### Planering för iteration 1
Det viktigaste uppgiften för nästa iterationen är att undersöka och bestämma vilka tekniker som ska användas. 

### Uppgifter
[Sprint backlog](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Sprint%20backlogs.md#iteration-1-vecka-13).


***

### Iteration 1 (Vecka 13)

### Analys av föregående iteration
Efter att ha undersökt flera tekniker som skulle kunna vara lämpliga har det skett en förändring i mitt val av teknik för back-end. Jag kommer att utveckla applikationen med Ruby on Rails istället för tidigare Electron. Detta minskar risken eftersom jag tidigare arbetat med just Ruby on Rails. 

### Planering för Iteration 3
Nästa steg blir fortsatt arbete med dokumentation, särskilt projektplan och kravspecifkation. Min plan är även att implementera högriskdelar och få en körbar publik version av applikationen som jag förhoppningsvis kan visa för kunden.

### Uppgifter
[Sprint backlog](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Sprint%20backlogs.md#iteration-2-vecka-14)

***

### Iteration 2 (Vecka 14)

### Analys av föregående iteration
Hade som mål att börja med front-edn delen och skapa en körbar version. Tanken var att använda Angular, men beslutet har istället fallit på React eftersom det verkar vara bättre integrerat med Rails. Det var dock inte helt enkelt att få det att fungera. Det visade sig att en liten miss från min sida ställde till det. 

Jag har nu också publicerat en version av applikationen på en droplet hos Digital Ocean. Det tog en hel dag. Jag ville inte använda en färdig lösning som Heroku eftersom jag efter kundens önskemål kan behöva lägga upp applikationen på en server i Sverige.

För övrigt har jag också bytt till att använda en postgreSQL-databas. Detta för att kunna använda dess sökfunktioner med pg_search.

Det har strulat mycket under den här iterationen, men det positiva är att jag har behandlat flera stora risker och fastslagit vilka tekniker som ska användas. Förhoppningsvis har jag en enklare bana framöver.

### Planering för nästa iteration
Under iteration 4 planerar jag att skapa de modellklasser som är kvar, samt börja med crud-funktionalitet för klienter och juridiska ärenden.

Testningen behöver också sättas igång, vilket den kommer att göra nästa vecka. 

### Uppgifter iteration 3
[Sprint backlog](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Sprint%20backlogs.md#iteration-3-vecka-15)


***

### Iteration 3 (Vecka 15)

## Analys av veckans arbete
Har arbetat mycket med att lära mig React. Har fått till en sida där en enskild klient visas. Det går också att redigera och ta bort klienten. Har problem med utformingen av databasen. 

Har däremot hunnit med att skriva fler tester och lära mig rspec tillsammans med shoulda-matchers för att skriva bra och kompakta tester. Tyvärr fungerar det inte så bra att testa själva vyverna eftersom mycket innehåll renderas med React vilket inte vill gå ihop med testramverken. 

I övrigt har jag skapat modellklasser och seedat de tabeller som är kvar, vilket betyder att de stora delarna är på plats. 

## Planering för nästa iteration
Under nästa iteration planerar jag att implementarea funktionalitet för att lägga till klienter och kontaktuppgifter, samt börja med crud-funktionalitet för ärenden. Jag vill även försöka få till möjligheten att testa de komponenter som renderas med React. 

### Uppgifter iteration 4
[Sprint backlog](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Sprint%20backlogs.md#iteration-4-vecka-16).

***

### Iteration 4 (Vecka 16)

### Analys av iteration
Har hunnit med att göra det jag företog mig under iterationen. Hade dock problem med automatiska tester för vyerna, vilket gjort att jag beslutat mig för att bara ha manuella tester för de vyer som renderas med React. 

I övrigt har det gått väldigt bra. Jag börjar bekanta mig mer med React och börjar kunna återanvända kod vilket gjort att det gått mycket snabbare än förväntat att skapa crud-funktionalitet för övriga modellklasser.

### Avklarade uppgifter
[Sprint backlog](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Sprint%20backlogs.md#iteration-4-vecka-16)

### Planering för nästa iteration
För Iteration 5 är målet att skapa crud-funktionalitet för tidrapporering, dvs de uppgifter som tillhör ett ärende. Med det börjar de stora bitarna bli färdiga vilket gör att jag kan börja fokusera på de icke-funktionella kraven.

### Uppgifter iteration 5
[Sprint backlog](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Sprint%20backlogs.md#iteration-5-vecka-17).

***

### Iteration 5 (Vecka 17)

### Analys av iteration
Ligger bra till enligt planeringen. Har dock fastnat lite för mycket i gränssnittet istället för att få de stora bitarna på plats. Måste göra mockups för att fundera över hur sidorna ska se ut innan jag arbetar för mycket med dem. Blir lätt att man fastnar med detaljer i css:en, vilket är för tidigt att göra i det här skedet. 

### Avklarade uppgifter
[Sprint backlog](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Sprint%20backlogs.md#iteration-5-vecka-17)

### Planering för nästa iteration
Backend-delen bör bli färdig nu. Men ska lägga till några kolumner i databasen efter kundens önskemål. Ska även utforska möjligheten att skapa en rapport i word-format, något som är ett önskemål från kunden. 

### Uppgifter iteration 6
[Sprint backlog](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Sprint%20backlogs.md#iteration-6-vecka-18).

***

### Iteration 6 (Vecka 18)
### Analys av iteration
Fick svårt att hinna med de uppgifter jag tagit mig an under iterationen. Detta berodde på att kunden önskade några ändringar som gjorde att jag behövde göra om databasrelationerna. Har haft problem med att publicera applikationen och har inte hunnit med testning. Däremot har jag förbättrat debuggingen för React-komponenterna vilket kommer att snabba på framtida utveckling.

### Avklarade uppgifter
[Sprint backlog](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Sprint%20backlogs.md#iteration-6-vecka-18)

### Planering för nästa iteration
Prioritet under iterationen är att få färdigt de stora byggstenarna. Det finns fortfarande några problem som måste lösas. Exempelvis att kunden vill att ett juridiskt ärende ska ha flera klienter och flera motparter och att det ska gå att lista och söka efter alla motparter som är inblandade i en klients ärenden.

Sedan behöver jag också få ordning på testerna och publicera en version så snart som möjligt.

### Uppgifter iteration 7
[Sprint backlog](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Sprint%20backlogs.md#iteration-7-vecka-19)

***

### Iteration 7 (Vecka 19)
### Analys av iteration
En fullständig applikation börjar nu växa fram. Har visat för kunden som är nöjd och visar stort intresse för applikationen. Det ökade intresset leder dock till en del önskemål om ändringar som gör att saker och ting tar längre tid.

### Avklarade uppgifter
[Sprint backlog](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Sprint%20backlogs.md#iteration-7-vecka-19)

### Planering för nästa iteration
Planen är få klart applikationen så att jag kan lägga resterande tid på att göra förbättringar, fixa buggar och jobba med ändringar i gränssnittet.

### Uppgifter iteration 8
[Sprint backlog](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Sprint%20backlogs.md#iteration-8-vecka-20)

***

### Iteration 8 (Vecka 20)
### Analys av iteration
Applikationen börjar bli klar. Men det finns många småsaker som skulle behöva fixas. Har skrivit upp dem i en [product backlog](https://docs.google.com/spreadsheets/d/19ByAyJSDggYLkyr8cpJMBzUUrwEBiPM0XIpPJHqxQiY/edit?usp=sharing) där de checkas av i prioritetsordning.

### Avklarade uppgifter
[Sprint backlog](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Sprint%20backlogs.md#iteration-8-vecka-20)

### Planering för nästa iteration
Applikationen är tillräckligt klar för att snart börja användas. Därför kommer den här iterationen ägnas åt att de få de sista betydande bitarna på plats.

### Uppgifter iteration 9
[Sprint backlog](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Sprint%20backlogs.md#iteration-9-vecka-21)

***

### Iteration 9 (Vecka 21)
### Analys av iteration
Vi har nu ett fullt fungerande system och om de skulle vilja skulle kunden kunna lägga in sina klienter idag. Har dock en ganska lång lista på saker som kan förbättras och läggas till. Vissa planerar jag att göra nästa iteration. Andra får hamna på listan över framtida funktionalitet. Kunden har testat och är mycket nöjd med applikationen. Flera andra jurister som känner min kund har även visat intresse. 

### Avklarade uppgifter
[Sprint backlog](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Sprint%20backlogs.md#iteration-8-vecka-20)

[Product backlog](https://docs.google.com/spreadsheets/d/19ByAyJSDggYLkyr8cpJMBzUUrwEBiPM0XIpPJHqxQiY/edit?usp=sharing)

### Planering för nästa iteration
Planen är att fixa det mest viktiga som är kvar. Städa upp koden, testa hur applikationen ser ut på olika skärmstorlekar och testa ännu mera.

### Uppgifter iteration 10
[Sprint backlog](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Sprint%20backlogs.md#iteration-10-vecka-22)

***

### Iteration 10 (Vecka 22)
### Analys av iteration
Kunden har börjat använda applikationen och tycker att det är en bra produkt. Utvecklingen har i det stora hela gått enligt planeringen. Har fokuserat mest på testning under iterationen. 

### Avklarade uppgifter
[Sprint backlog](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Sprint%20backlogs.md#iteration-9-vecka-21)

### Planering för framtiden
Applikationen är redo för användning, men det är inte färdigt för mig utan blir ett projekt som jag kommer att bygga förbättra kontinuerligt. 

Min  [lista](https://docs.google.com/spreadsheets/d/19ByAyJSDggYLkyr8cpJMBzUUrwEBiPM0XIpPJHqxQiY/edit?usp=sharing) saker att göra och sådant som kan förbättras kommer att fortsätta att bockas av. 
