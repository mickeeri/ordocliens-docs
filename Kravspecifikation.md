# Kravspecifikation

## 1. Ej funktionella krav
#### 1.1. Användbarhet
1.1.1. Applikationens design ska vara responsiv. </br>
1.1.2. Lämpliga fel- och rättmeddelanden ska presenteras för användaren. </br>

#### 1.2. Pålitlighet
1.2.1. Applikationen ska testas med hjälp av automatiska tester. </br>
1.2.2. Applikationen ska testas med manuella tester. </br>
1.2.3. Applikationen ska fungera i de vanligaste webbläsarna. (IE, Firefox, Edge, Safari, Chrome). </br>
1.2.4. Applikationen ska fungera i >= IE 9. </br>

#### 1.3. Underhåll
1.3.1. Applikationen ska vara publicerad på en server i sverige. </br>
1.3.2. Databasen ska ha en backup-lösning. </br>

#### 1.4. Prestanda
1.4.1. Interaktion med applikationens sidor ska i möjligaste mån fungera utan sidomladdningar. </br>
1.4.2. Sökning och annan filtering av resurser ska gå snabbt. </br>

#### 1.5. Säkerhet och integritet
1.5.1. Applikationen ska använda SSL. </br>
1.5.2. Lagring av personuppgifter ska följa personuppgiftslaget (PUL). </br>
--1.5.2.1. Personuppgifter ska lagras på en server i Sverige. </br>
--1.5.2.2. Strategi för att inte lagra uppgifter i onödan ska finnas. </br>



## 2. Funktionella krav

#### 2.1. Användarkonto
|#|Krav                                         ||
|-----------------------------------------------|----|------|
|2.1.1|Logga in med e-post och lösenord.|:white_check_mark:|
|2.1.2|Ändra användaruppgifter.|:white_check_mark:|
|2.2.3|Återställa lösenord.|:white_large_square:|
|2.2.4|Bli ihågkommen mellan sessioner.|:white_check_mark:|
|2.2.5|Logga ut.|:white_check_mark:|

#### 2.2. Hantera klienter
|#|Krav                                         ||
|-----------------------------------------------|----|------|
|2.2.1|Skapa klienter.|:white_large_square:|
|2.2.2|Få en lista över klienter.|:white_check_mark:|
|--2.2.2.1|Filtera listan på klienter med sökord.|:white_check_mark:|
|2.2.3|Redigera klienter.|:white_check_mark:|
|2.2.4|Radera klienter.|:white_check_mark:|
|2.2.5|Lägga till kontaktuppgifter till klient.|:white_large_square:|
|--2.2.5.1|Redigera kontaktuppgift.|:white_large_square:|
|--2.2.5.2|Ta bort kontaktuppgift.|:white_large_square:|

#### 2.3. Hantera juridiska ärenden
|#|Krav                                         ||
|-----------------------------------------------|----|------|
|2.3.1|Registera ärenden som tillhör en klient.|:white_large_square:|
|2.3.2|Få en lista över ärenden.|:white_large_square:|
|--2.3.2.1|Filtera listan på ärenden med sökord.|:white_large_square:|
|--2.3.2.2|Välja mellan att visa aktiva och ej aktiva ärenden.|:white_large_square:|
|2.3.3|Redigera ärende.|:white_large_square:|
|2.3.4|Radera ärende.|:white_large_square:|
|2.3.6|Se summering av arbetade timmar med ett ärende.|:white_large_square:|

#### 2.4. Hantera tidrapporter
|#|Krav                                         ||
|-----------------------------------------------|----|------|
|2.4.1|Lägga till tidrapporter med tid i timmar, notering och datum.|:white_large_square:|
|2.4.2|När man lägger till datum ska dagens datum vara förifyllt.|:white_large_square:|
|2.4.3|Välja mellan fyra olika prisklasser: arbete, utlägg, tidsspillan låg och tidsspillan hög.|:white_large_square:|

#### 2.5. Hantera konstnadsräkningar/rapporter
|#|Krav                                         ||
|-----------------------------------------------|----|------|
|2.5.1|Få en genererad kostnadsräkning när ärende är avslutat.|:white_large_square:|
|2.5.2|Rapporten ska genereras och beräknas automatisk men gå att redigera.|:white_large_square:|

***
*Senast uppdaterad 2016-04-11*
