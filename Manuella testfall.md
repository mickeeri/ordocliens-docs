# Manuella testfall

## 1. Användare
### TF 1.1. Logga in med korrekta uppgifter
#### Krav som testas
2.1.1: Logga in med e-post och lösenord.

#### Förkrav
En användare finns i databasen.

#### Scenario
1. Besök startsidan.
2. Ange e-postadress: micke@mail.com
3. Ange lösenord: password
4. Klicka på "Logga in"

#### Efterkrav
* Användaren är inloggad.
* Ser lista på klienter.

## 2. Klienter
### TF 2.1. Skapa klient
#### Krav som testas
* 2.2.1. Skapa klienter.
* 2.2.2. Få en lista över klienter.

#### Förkrav
* TF 1.1. Användaren är inloggad.

#### Scenario
1. Klicka på "Lägg till klient"
2. Fyll i formuläret med följande uppgifter:
```
Förnamn: Test
Efternamn: Användare
Personnummer: 9810154556
E-post: mail@exempel.se
Telefonnummer: 070-87822131
Gatuadress: Södra gatan 10
Postnummer: 21311
Ort: Exempelort
Anteckningar: Lorem ipsum
```
3. Klicka på "Spara"

#### Efterkrav
* Omdirigeras till den skapade klientens sida `/clients/:id`.
* Meddelande "Klient skapad!" visas.
* Information om klienten som motsvarare ifyllda uppgifter visas.
* Klienten visas i listan över klienter `/clients`.

***

### TF 2.1.1 Skapa klient utan att ange nödvändiga fält
#### Krav som testas
* 2.2.1. Skapa klienter.
* 1.1.2. Lämpliga fel- och rättmeddelanden ska presenteras för användaren.

#### Förkrav
* TF 1.1. Användaren är inloggad.

#### Scenario
1. Klicka på "Lägg till klient".
2. Fyll i samma uppgifter som i TF 2.1 men lämna fältet "Förnamn" tomt.
3. Klicka på "Spara".
4. Fyll i fältet "Förnamn" men lämna "Efternamn" tomt.
5. Klicka på "Spara".
4. Fyll i alla fält utom "Personnummer" som lämnas tomt.
5. Klicka på "Spara"

#### Efterkrav
* Felmeddelande visas.
* Kvar på formulär för att skapa klient.
* Klient har inte blivit skapad.

***

### TF 2.2. Redigera klient
#### Krav som testas
2.2.3	Redigera klienter.

#### Förkrav
* TF 1.1. Användaren är inloggad.
* TF 2.1. Klient skapad och befinner sig på klientens sida. Url: `clients/:id`.

#### Scenario
1. Klicka på "Redigera klient"
2. Kontrollera att uppgifter är ifyllda i input-fälten.
3. Ändra fältet förnamn till "Redigerat förnamn".
4. Ändra fältet "Ort" till "Ändrad ort".
5. Ändra uppgifter i valfria fält.
6. Klicka på "Spara".

#### Efterkrav
* Klienten har uppdaterats med angivna uppgifter.
* I "Breadcrumb-listen" har namnet ändrats.
* Inga input-fält syns och knappen "Redigera klient" är inte aktiv.

***

### TF 2.2.1 Redigera klient utan att ange nödvändiga fält
#### Krav som testas
* 2.2.3	Redigera klienter.
* 1.1.2. Lämpliga fel- och rättmeddelanden ska presenteras för användaren.

#### Förkrav
* TF 1.1. Användaren är inloggad.
* TF 2.1. Klient skapad och befinner sig på klientens sida, url: `clients/:id`.

#### Scenario
1. Klicka på "Redigera klient".
2. Klicka på "Spara" utan att ange "Förnamn".
3. Klicka på "Spara" utan att ange "Efternamn".
4. Klicka på "Spara" utan att ange "Personnummer".

#### Efterkrav
* Felmeddelande visas.
* Kvar på samma formulär.
* Om man klickar på "Avbryt" är uppgifterna ej uppdaterade.

***

### TF 2.2.2 Redigera klient navigering
Testa att knappar på redigeringssidan uppvisar förväntat beteende.
#### Krav som testas
* 2.2.3	Redigera klienter.

#### Förkrav
* TF 1.1. Användaren är inloggad.
* TF 2.1. Klient skapad och befinner sig på klientens sida, url: `clients/:id`.

#### Scenario
1. Klicka på "Redigera klient".
2. Klicka på "Avbryt"
3. Klicka på "Redigera klient".
4. Klicka på samma knapp "Redigera klient".

#### Efterkrav
Att klicka på knapparna gör att sidan ändrar mellan redigeringsläge och visningsläge.

***

### TF 2.3 Ta bort klient
#### Krav som testas
2.2.4	Radera klienter.

#### Förkrav
* TF 1.1. Användaren är inloggad.
* TF 2.1. Klient skapad och befinner sig på klientens sida, `/clients/:id`.

#### Scenario
1. Klicka på "Ta bort klient".
2. Klicka på "Avbryt" i den popup-ruta som visas.
3. Klicka på "Ta bort klient" igen.
4. Klicka på krysset i hörnet på rutan.
5. Klicka på "Ta bort klient" ännu en gång.
6. Klicka på "Ja".

#### Efterkrav
* Omdirigeras till startsidan. Url: `/clients`.
* Ett meddelande "Klienten har raderats" visas.


## 3. Juridiska ärenden
### TF 3.1 Skapa juridiskt ärenden
#### Krav som testas
* 2.3.1. Registera ärenden som tillhör en klient.
* 2.3.2. Få en lista över ärenden.

#### Förkrav
* TF 1.1. Användaren är inloggad.
* TF 2.1. Klient skapad och befinner sig på klientens sida: `clients/:id`.

#### Scenario
1. Klicka på "Lägg till ärende".
2. Klicka på "Avbryt".
3. Klicka på "Lägg till ärende" igen.
4. Skriv "Ett nytt ärende" i fältet "Ärendenamn".

#### Efterkrav
* Ärende med ifyllt namn visas. Ärendet är aktivt.
* Ärendet skall finnas i listan över ärenden på klientens sida.

***

### TF 3.1.2 Skapa juridiskt ärenden utan att fylla i namn.
#### Krav som testas
* 2.3.1. Registera ärenden som tillhör en klient.
* 1.1.2. Lämpliga fel- och rättmeddelanden ska presenteras för användaren.

#### Förkrav
* TF 1.1. Användaren är inloggad.
* TF 2.1. Klient skapad och befinner sig på klientens sida: `clients/:id`.

#### Scenario
1. Klicka på "Lägg till ärende".
2. Klicka på "Spara" utan att ange "Ärendenamn".

#### Efterkrav
* Kvar på samma formulär.
* Felmeddelande visas.
* Ärende är ej sparat.

***

### TF 3.2 Redigera juridiskt ärende.
Testar att det går att redigera ett ärende. Testar även att det är skifta mellan redigeringsläge och visningsläge.
#### Krav som testas
2.3.3	Redigera ärende.

#### Förkrav
* TF 1.1. Användaren är inloggad.
* TF 2.1. Klient skapad och befinner sig på klientens sida: `clients/:id`.
* TF 3.1. Juridiskt ärende finns och användaren befinner sig på ärendets sida: `clients/:id/legal_cases/:id`.

#### Scenario
1. Klicka på "Redigera ärende".
2. Kontrollera att tidigare värde är förifyllt.
3. Klicka på "Avbryt".
4. Klicka på "Redigera ärende".
5. Klicka på "Redigera ärende" igen.
6. Klicka på "Redigera ärende" ännu en gång för att få upp formuläret.
7. Ange "Ett redigerat ärende" i fältet "Ärendenamn".

#### Efterkrav
* Ärendets sida befinner sig i visningsläge.
* Meddelande om att ärende har skapats visas.
* Ärendets namn, uppdaterat-datum och "breadcrumb-länken" är uppdaterade.

***

### TF 3.2.1 Redigera juridiskt ärende utan att ange nödvändiga fält.
#### Krav som testas
* 2.3.3	Redigera ärende.
* 1.1.2. Lämpliga fel- och rättmeddelanden ska presenteras för användaren.

#### Förkrav
* TF 1.1. Användaren är inloggad.
* TF 3.1. Juridiskt ärende finns och användaren befinner sig på ärendets sida: `clients/:id/legal_cases/:id`.

#### Scenario
1. Klicka på "Redigera ärende".
2. Radera tidigare värde så att fältet "Ärendenamn" är tomt.
3. Klicka på "Spara".

#### Efterkrav
* Kvar på samma formuläret.
* Ett felmeddelande visas.
* Uppgifterna har inte uppdaterats.

***

### TF 3.3 Ta bort juridiskt ärende
#### Krav som testas
2.3.4	Radera ärende.

#### Förkrav
* TF 1.1. Användaren är inloggad.
* TF 2.1. Klient skapad och befinner sig på klientens sida: `clients/:id`.
* TF 3.1. Juridiskt ärende finns och användaren befinner sig på ärendets sida: `clients/:id/legal_cases/:id`.

#### Scenario
1. Klicka på "Ta bort ärende".
2. Klicka på "Avbryt".
3. Klicka på "Ta bort ärende" igen.
4. Klicka på "Ja".

#### Efterkrav
* Omdirigeras till ärendets klient sida: `/clients/:id`.
* Meddelande "Ärendet har raderats" visas.
* Ärendet visas inte i listan på klientens ärenden.
