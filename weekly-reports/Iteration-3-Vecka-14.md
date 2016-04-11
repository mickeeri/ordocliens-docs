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
|Uppgift                                        |Krav|Status|
|-----------------------------------------------|----|------|
|Skapa modellklasser för kontaktuppgifter.      ||:x:|
|Skapa modellklasser för tidrapporter/uppgifter.||:x:|
|Lägga till kontaktuppgifter till klient.      ||:x:|
|Lägga till klient        ||:x:|
|Ta bort klient.         ||:x:|
|Redigera klient   ||:x:|
|Få ordning på dokumentation                        ||:x:|
|Få existerande automatiska tester att gå igenom                      ||:x:|
|Testrapport                      ||:x:|
|Publicering och delleverans                      ||:x:|
|Iterationsplan för nästa vecka                    ||:x:|
