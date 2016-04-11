# Iteration 3 (Vecka 14)

## Analys av föregende iteration
Hade som mål att börja med front-end delen och skapa publicera en körbar version. Gällande front-end var tanken att jag skulle använda Angular, men har istället beslutat mig för att använda React. Detta eftersom det sistnämnda verkar vara bättre integrerat med Rails. Ändå har jag haft stora problem med att få det att fungera. Att jag läste in alla skript i slutet av layout-dokumentet verkade vara det som ställde till det.

Jag har nu också publicerat en version av applikationen på en vps hos Digital Ocean. Det tog en hel dag. Jag ville inte använda en färdig lösning som Heroku eftersom jag kan behöva lägga upp applikationen på en vps i Sverige, pga av PUL.

För övrigt har jag också bytt till att använda en postgreSQL-databas. Detta för att kunna använda dess sökfunktioner.

Det har strulat mycket under den här iterationen, men det positiva är att jag har behandlat flera stora risker och fastslagit vilka tekniker som ska användas. Förhoppningsvis har jag en rakare bana framöver.

## Planering av nästa iteration
Under iteration 4 planerar jag att skapa de modellklasser som är kvar, samt börja med crud-funktionalitet för klienter och juridiska ärenden.

Den här veckan hann jag inte heller med så mycket testning. Så det kommer att jag göra nästa vecka.

### Uppgifter
|Uppgift                                        |Krav||
|-----------------------------------------------|----|------|
|Skapa modellklasser för kontaktuppgifter.      |2.2.1|:white_large_square:|
|Skapa modellklasser för tidrapporter/uppgifter.|2.4.1|:white_large_square:|
|Lägga till klient        |2.2.1|:white_large_square:|
|Redigera klient   |2.2.3|:white_large_square:|
|Ta bort klient.         |2.2.4|:white_large_square:|
|Få ordning på dokumentation                        ||:white_large_square:|
|Få existerande automatiska tester att gå igenom                      |1.2.1|:white_large_square:|
|Testrapport                      ||:white_large_square:|
|Publicering och delleverans                      ||:white_large_square:|
|Iterationsplan för nästa vecka                    ||:white_large_square:|
