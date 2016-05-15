## Manuella integraionstest
### 1. Klienter och motparter
Test som kontrollerar att det går att skapa klienter och att kopplingen mellan klienter, ärenden och motparter fungerar som den ska. Alla motparter som är inblandade i ett ärende som klienter deltar i ska nämligen hamna på klientens lista över motparter.

#### Förkrav
Måste vara inloggad.

#### Testar krav
* 2.2.1 Skapa klient
* 2.3.1 Registera ärende.
* 2.4.1 Lägga till motpart till ärende.
* 2.4.6 Lista över motparter på klientens sida.
* 2.4.7 Motpart ska ha en lista över ärenden och klienter.

#### Scenario
1. Skapa en ny klient.
2. Skapa ett nytt ärende.
3. Skapa en motpart med “Lägg till ny motpart”.
4. Klicka på länken till klients sida. Kontrollera att motparten visas under rubriken motparter.
5. Skapa en till klient.
6. Skapa ett ärende från den klientens sida.
7. Gå in på ärendet. Lägg till en motpart till ärendet med “Lägg till befintlig motpart”.
8. Kontrollera att motparten ligger på klientens sida.
9. Gå in på ärendet igen. Skapa en ny klient genom “Lägg till ny klient”.
10. Kontrollera att även denna klient har motparten på sin sida.
11. Från samma ärende. Skapa en helt ny motpart och kontrollera att båda klienterna frå denna på sin sida.
12. Lägg till den tredje klienten (punkt 1) genom lägg till befintlig klient.
13. Kontrollera även denna klienten från motparterna på sin sida.
14. Gå in på en av motparternas sida. Den bör ha ärendet och klienterna i en lista.

***

### 2. Arkivera ärenden

#### Förkrav
* Måste vara inloggad.
* Har skapat minst ett ärende.

#### Testar krav
* 2.3.5 Arkivera ärende

#### Scenario
1. Gå in på ett nyskapat ärende.
2. Skapa ett nytt ärende.
3. Skapa en motpart med “Lägg till ny motpart”.
4. Klicka på länken till klients sida. Kontrollera att motparten visas under rubriken motparter.
5. Skapa en till klient.
6. Skapa ett ärende från den klientens sida.
7. Gå in på ärendet. Lägg till en motpart till ärendet med “Lägg till befintlig motpart”.
