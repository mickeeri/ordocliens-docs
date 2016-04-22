# Testrapporter
* [Iteration 1](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Testrapporter.md#testrapport-iteration-1-vecka-13)
* [Iteration 2](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Testrapporter.md#testrapport-iteration-2-vecka-14)
* [Iteration 4](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Testrapporter.md#testrapport-iteration-3-vecka-15)
* [Iteration 5](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Testrapporter.md#testrapport-iteration-4-vecka-16)
* [Iteration 6](https://github.com/me222wm/1dv42e-me222wm-docs/blob/master/Testrapporter.md#testrapport-iteration-5-vecka-17)

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


