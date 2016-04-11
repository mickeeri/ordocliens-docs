# Kravspecifikation

## 1. Ej funktionella krav
#### 1.1. Användbarhet
1.1.1. Applikationens design ska vara responsiv.
1.1.2. Lämpliga fel- och rättmeddelanden ska presenteras för användaren.

#### 1.2. Pålitlighet
1.2.1. Applikationen ska testas med hjälp av automatiska tester.
1.2.2. Applikationen ska testas med manuella tester.
1.2.3. Applikationen ska fungera i de vanligaste webbläsarna. (IE, Firefox, Edge, Safari, Chrome).
1.2.4. Applikationen ska fungera i >= IE 9.

#### 1.3. Underhåll
1.3.1. Applikationen ska vara publicerad på en server i sverige.
1.3.2. Databasen ska ha en backup-lösning.

#### 1.4. Prestanda
1.4.1. Interaktion med applikationens sidor ska i möjligaste mån fungera utan sidomladdningar.
1.4.2. Sökning och annan filtering av resurser ska gå snabbt.

#### 1.5. Säkerhet och integritet
1.5.1. Applikationen ska använda SSL.
1.5.2. Lagring av personuppgifter ska följa personuppgiftslaget (PUL).
&ensp;&ensp; 1.5.2.1. Personuppgifter ska lagras på en server i Sverige.
&ensp;&ensp; 1.5.2.2. Strategi för att inte lagra uppgifter i onödan ska finnas.



## 2. Funktionella krav
#### Användare ska kunna:
|#|Krav                                         |Status|
|-----------------------------------------------|----|------|
|2.1|Ha ett användarkonto|:white_large_square:|
|2.1.1|Logga in med e-post och lösenord.|:heavy_check_mark:|
|2.1.2|Ändra sina uppgifter.|:heavy_check_mark:|
|2.2.3|Återställa lösenord.|:heavy_minus_sign:|
|2.2.4|Bli ihågkommen mellan sessioner.|:heavy_check_mark:|
|2.2.5|Logga ut.|:heavy_check_mark:|

|#|Krav                                         |Status|
|-----------------------------------------------|----|------|
|2.2|Hantera klienter|:heavy_minus_sign:|
|2.2.1|Registera nya klienter med namn och kontaktuppgifter.|:heavy_minus_sign:|
|2.2.2|Få en lista över klienter.|:heavy_check_mark:|
|2.2.2.1|Filtera listan på klienter med sökord.|:heavy_minus_sign:|
|2.2.3|Redigera klienter.|:heavy_minus_sign:|
|2.2.4|Radera klienter.|:heavy_minus_sign:|

|#|Krav                                         |Status|
|-----------------------------------------------|----|------|
|2.3|Hantera juridiska ärenden.|:heavy_minus_sign:|
|2.3.1|Registera ärenden som tillhör en klient.|:heavy_minus_sign:|
|2.3.2|Få en lista över ärenden.|:heavy_minus_sign:|
|2.3.2.1|Filtera listan på ärenden med sökord.|:heavy_minus_sign:|
|2.3.2.2|Välja mellan att visa aktiva och ej aktiva ärenden.|:heavy_minus_sign:|
|2.3.3|Redigera ärende.|:heavy_minus_sign:|
|2.3.4|Radera ärende.|:heavy_minus_sign:|
|2.3.6|Se summering av arbetade timmar med ett ärende.|:heavy_minus_sign:|

|#|Krav                                         |Status|
|-----------------------------------------------|----|------|
|2.4|Hantera tidrapporter.|:heavy_minus_sign:|
|2.4.1|Lägga till tidrapporter med tid i timmar, notering och datum.|:heavy_minus_sign:|
|2.4.2|När man lägger till datum ska dagens datum vara förifyllt.|:heavy_minus_sign:|
|2.4.3|Välja mellan fyra olika prisklasser: arbete, utlägg, tidsspillan låg och tidsspillan hög.|:heavy_minus_sign:|

|#|Krav                                         |Status|
|-----------------------------------------------|----|------|
|2.5|Hantera konstnadsräkningar/rapporter.|:heavy_minus_sign:|
|2.5.1|Få en genererad kostnadsräkning när ärende är avslutat.|:heavy_minus_sign:|
|2.5.2|Rapporten ska genereras och beräknas automatisk men gå att redigera.|:heavy_minus_sign:|

***
*Senast uppdaterad 2016-04-11*
