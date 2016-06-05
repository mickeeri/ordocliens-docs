# Kravspecifikation

## 1. Ej funktionella krav
#### 1.1. Användbarhet
1.1.1. Applikationens design ska vara responsiv. </br>
1.1.2. Lämpliga fel- och rättmeddelanden ska presenteras för användaren. </br>

#### 1.2. Pålitlighet
1.2.1. Applikationen ska testas med hjälp av automatiska tester. </br>
1.2.2. Applikationen ska testas med manuella tester. </br>
1.2.3. Applikationen ska fungera i de vanligaste webbläsarna. (IE, Firefox, Edge, Safari, Chrome). </br>

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


## 2. Funktionella krav

#### 2.1. Användarkonto
|#     |Krav                                    |                    |Test |
|------|----------------------------------------|--------------------|-------|
|2.1.1|Logga in med e-post och lösenord.        |:white_check_mark:  |A, M   |
|2.1.2|Ändra användaruppgifter.                 |:white_check_mark:  |A      |
|2.2.3|Återställa lösenord.                     |:white_check_mark:  |M      |
|2.2.4|Bli ihågkommen mellan sessioner.         |:white_check_mark:  |M      |
|2.2.5|Logga ut.                                |:white_check_mark:  |A, M   |

#### 2.2. Hantera klienter
|#      |Krav                                                                |                   |Test|
|-------|--------------------------------------------------------------------|-------------------|-------|
|2.2.1|Skapa klienter.                                                       |:white_check_mark:  |M     |
|2.2.2|Få en lista över klienter.                                            |:white_check_mark:  |M     |
|--2.2.2.1|Filtera listan på klienter med sökord.                            |:white_check_mark:  |M, A  |
|2.2.3|Redigera klienter.                                                    |:white_check_mark:  |M, A  |
|2.2.4|Radera klienter.                                                      |:white_check_mark:  |M, A  |
|2.2.5|Välja mellan att visa alla firmans klienter eller bara egna klienter. |:white_check_mark:  |M     |

#### 2.3. Hantera juridiska ärenden
|#     |Krav                                                  |                    |Test  |
|-----|-------------------------------------------------------|--------------------|------|
|2.3.1|Registera ärenden som tillhör en klient.               |:white_check_mark:  |M, A  |
|2.3.2|Få en lista över ärenden.                              |:white_check_mark:  |M     |
|--2.3.2.1|Filtera listan på ärenden med sökord.              |:white_check_mark:  |M     |
|--2.3.2.2|Välja mellan att visa aktiva och ej aktiva ärenden.|:white_check_mark:  |M     |
|2.3.3|Redigera ärende.                                       |:white_check_mark:  |M, A  |
|2.3.4|Radera ärende.                                         |:white_check_mark:  |M, A  |
|2.3.5|Arkivera ärende                                         |:white_check_mark: |M, A  |

#### 2.4. Hantera motparter
|#     |Krav                                                  |                    |Test  |
|-----|-------------------------------------------------------|--------------------|------|
|2.4.1|Lägga till motparter till ärende                       |:white_check_mark:  |M, A  |
|2.4.2|Få en lista över motparter.                            |:white_check_mark:  |M     |
|--2.4.2.1|Filtera listan på motparter med sökord.            |:white_check_mark:  |M     |
|2.4.3|Redigera motpart.                                      |:white_check_mark:  |M, A  |
|2.4.4|Radera motpart helt och hållet                         |:white_check_mark:  |M, A  |
|2.4.5|Radera motpart från ärende.                            |:white_check_mark:  |M, A  |
|2.4.6|Lista över motparter ska visas på klients sida         |:white_check_mark:  |M     |
|2.4.7|Motpart ska ha en lista över ärenden och klienter.     |:white_check_mark:  |M     |

#### 2.5. Hantera tidrapporter
|#     |Krav                                                                                    |                  |Test |
|------|----------------------------------------------------------------------------------------|------------------|-----|
|2.5.1|Lägga till arbete eller tidsspillan till tidrapport.                                     |:white_check_mark:|M, A |
|--2.5.1.1|När man lägger till datum ska dagens datum vara förifyllt.                           |:white_check_mark:|M    |
|--2.5.1.2|Välja mellan tre olika prisklasser.                                                  |:white_check_mark:|M    | 
|2.5.2|Redigera arbetsrad                                                                       |:white_check_mark:|M, A |
|2.5.3|Ta bort arbetsrad                                                                        |:white_check_mark:|M, A|
|2.5.4|Lägga till utlägg till tidrapport                                                        |:white_check_mark:|M, A|
|2.5.5|Redigera utläggsrad                                                                      |:white_check_mark:|M, A|
|2.5.6|Ta bort utläggsrad från tidrapport                                                       |:white_check_mark:|M, A |
|2.5.7|Arbete och utlägg ska visas i en tabell                                                  |:white_check_mark:|M |
|2.5.8|Tabellen ska kunna konverteras till ett .docx-dokument                                   |:white_check_mark:|M      |
|--2.5.8.1|Arbetade timmar ska summeras efter priskategori.                                     |:white_check_mark:|M      |
|--2.5.8.2|Utlägg i kronor ska summeras.                                                        |:white_check_mark:|M      |

#### 2.6. Hantera konstnadsräkningar/rapporter
|#     |Krav                                                                |                    |Testas?|
|------|--------------------------------------------------------------------|--------------------|------|
|2.6.1 |Få en genererad kostnadsräkning när ärende är avslutat.             |:white_large_square:|M |
|2.6.2 |Rapporten ska genereras och beräknas automatisk men gå att redigera.|:white_large_square:|M|

