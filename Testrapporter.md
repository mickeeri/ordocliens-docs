# Testrapporter
* [Iteration 1](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Testrapporter.md#testrapport-iteration-1-vecka-13)
* [Iteration 2](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Testrapporter.md#testrapport-iteration-2-vecka-14)
* [Iteration 3](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Testrapporter.md#testrapport-iteration-3-vecka-15)
* [Iteration 4](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Testrapporter.md#testrapport-iteration-4-vecka-16)
* [Iteration 5](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Testrapporter.md#testrapport-iteration-5-vecka-17)
* [Iteration 6](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Testrapporter.md#testrapport-iteration-6-vecka-18)
* [Iteration 7](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Testrapporter.md#testrapport-iteration-7-vecka-19)
* [Iteration 8](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Testrapporter.md#testrapport-iteration-8-vecka-20)

## Testrapport Iteration 1, Vecka 13

### Datum
2016-04-03

### Automatiska tester
Se automatiska tester och resultat [här](https://htmlpreview.github.io/?https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/test-reports/rspec-result%202016-04-03.html).

### Analys
Systemet är fortfarande i inledningsfasen, men det verkar efter testningen vara en bra grund att bygga ut projektet på.

***

## Testrapport Iteration 2, Vecka 14

### Datum
2016-04-12

### Automatiska tester
På grund av flera förändingar bland annat införandet av Devise för användarhantering felar nästan alla automatiska tester. Saker och ting fungerar som de ska men tester och fixturer behöver göras om.

## Testrapport Iteration 3, Vecka 15

### Datum 
2016-04-17

### Automatiska tester
Rapport från automatiska tester finns [här](http://htmlpreview.github.io/?https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/test-reports/rspec-result%202016-04-17.html)

### Analys 
Systemet känns fortfarande stabilt. Har försökt men inte lycktas med att göra tester för vyerna eftersom det är React som renderar innehållet. Får försöka nästa vecka eller enbart testa det manuellt. 

## Testrapport Iteration 4, Vecka 16
### Version
[v0.4](https://github.com/me222wm/1dv42e-me222wm/tree/v0.4)

### Datum 
2016-04-22

### Automatiska tester
Lista på automatiska tester och resultat [här](http://htmlpreview.github.io/?https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/test-reports/rspec-result%202016-04-22.html)

### Manuella tester
#### Testmiljö
Publicerad version av [applikationen](http://188.166.165.105/).

Testat i Chrome Version 49.0.2623.112 m (64-bit)

### Resultat

|#    |Testfall                                            |Resultat          |Kommentar|
|-----|----------------------------------------------------|------------------|---------|
|1.1|Logga in med korrekta uppgifter                       |:white_check_mark:||
|2.1|Skapa klient                                          |:white_check_mark:||
|2.1.1|Skapa klient utan att ange nödvändiga fält          |:x:|Visas inte felmeddelanden.|
|2.2|Redigera klient                                       |:white_check_mark:||
|2.2.1|Redigera klient utan att ange nödvändiga fält       |:x:|Inga felmeddelanden.|
|2.2.2|Redigera klient navigering                          |:white_check_mark:||
|2.3|Ta bort klient                                        |:white_check_mark:||
|3.1|Skapa juridiskt ärenden                               |:white_check_mark:||
|3.1.2|Skapa juridiskt ärenden utan att fylla i namn.      |:x:|Inget felmeddelande.|
|3.2|Redigera juridiskt ärende.                            |:white_check_mark:||
|3.2.1|Redigera juridiskt ärende utan att ange nödvändiga fält.|:x:|Inget felmeddelande.|
|3.3|Ta bort juridiskt ärende                              |:white_check_mark:||

### Analys 
Applikationen fungerar överlag bra. Några av de manuella testerna felade eftersom jag inte har implementerat några felmeddelanden på front-end. Förutom det fungerar validering på serversidan som den ska. 

## Testrapport Iteration 5, Vecka 17
### Version
[v0.5](https://github.com/me222wm/1dv42e-me222wm/tree/v0.5)

### Datum 
2016-04-30

### Automatiska tester
Lista på automatiska tester och resultat [här](https://htmlpreview.github.io/?https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/test-reports/rspec-result%202016-04-30.html)

### Manuella tester
#### Testmiljö
Lokal miljö. 

Testat i Chrome Version 49.0.2623.112 m (64-bit)


### Resultat

|#    |Testfall                                            |Resultat          |Kommentar|
|-----|----------------------------------------------------|------------------|---------|
|1.1|Logga in med korrekta uppgifter                       |:white_check_mark:||
|2.1|Skapa klient                                          |:white_check_mark:||
|2.1.1|Skapa klient utan att ange nödvändiga fält          |:white_check_mark:||
|2.2|Redigera klient                                       |:white_check_mark:||
|2.2.1|Redigera klient utan att ange nödvändiga fält       |:white_check_mark:||
|2.2.2|Redigera klient navigering                          |:x:|Funktionalitet under arbete.|
|2.3|Ta bort klient                                        |:white_check_mark:||
|3.1|Skapa juridiskt ärenden                               |:white_check_mark:||
|3.1.2|Skapa juridiskt ärenden utan att fylla i namn.      |:white_check_mark:||
|3.2|Redigera juridiskt ärende.                            |:x:|Ändringar i gränssnittet gör att det inte går att redigera.|
|3.2.1|Redigera juridiskt ärende utan att ange nödvändiga fält.|:x:||
|3.3|Ta bort juridiskt ärende                              |:x:|Tas bort, men sker ingen redirect|

### Analys 
Applikationen fungerar bra på serversidan. Men på grund av stora förändingar i gränssnittet fungerar inte all funktionalitet som den ska. Det behövs bara små ändringar för att få det att fungera igen. 

## Testrapport Iteration 6, Vecka 18
Ingen testning. 

## Testrapport Iteration 7, Vecka 19
### Version
[v0.7](https://github.com/me222wm/1dv42e-me222wm/tree/v0.7)

### Datum 
2016-05-15

### Automatiska tester
Lista på automatiska tester och resultat [här](https://htmlpreview.github.io/?https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/test-reports/rspec-result%202016-05-15.html)

### Manuella tester
#### Testmiljö
Lokal miljö. 

Testat i Chrome Version 49.0.2623.112 m (64-bit)

### Resultat
[Under iteration 7](https://docs.google.com/spreadsheets/d/19ByAyJSDggYLkyr8cpJMBzUUrwEBiPM0XIpPJHqxQiY/edit#gid=1648702780)

### Analys 
Alla testerna fungerar. Sytemet känns stabilt. 

## Testrapport Iteration 8, Vecka 20
### Version
[v0.8](https://github.com/me222wm/1dv42e-me222wm/tree/v0.8)

### Datum 
2016-05-23

### Automatiska tester
Lista på automatiska tester och resultat [här](https://htmlpreview.github.io/?https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/test-reports/rspec-result%202016-05-23.html)

### Manuella tester
#### Testmiljö
Lokal miljö: 
Testat i Chrome Version 50.0.2661.102 (64-bit)
Publicerad applikation: 
Testad i Microsoft Edge 25.19586.0.0

#### Resultat
Resultat från manuella tester presenterar numer [här](https://docs.google.com/spreadsheets/d/1rzFkEfqJGzqhJhAANs7PTpTYKmhoc2VUc4Grx-b3ISc/edit?usp=sharing)

### Analys 
Testerna går igenom. Samtidigt har det skett många förändringar på kort tid, vilket gör att det finns en osäkerhetskänsla. 

