# Testspecifikation

### Allmänna testprocedurer
Testning bör ske i slutet av varje iteration. Det genomförs genom att automatiska tester körs och manuella testfall genomgås. 

I största möjligaste mån kommer automatiska tester att användas. Det gäller främst back-end-delen. Front-end-delen som består mest av React-komponenter har visat sig vara svår att testa automatiskt. Därför kommer manuella testfall att skrivas för dessa.

### Testmiljö
Testningen av back-end-delen kommer att testas med testramverket [RSpec](http://rspec.info/) för Ruby on Rails.

Testning av React-komponenter sker med manuella tester.

Manuell testning kommer att ske på olika moderna webbläsare i flera enheter.

### Manuell testning
Manuella testfalls genomförande och resultat presenteras f.r.o.m Iteration 8 i ett [Google Sheets dokument](https://docs.google.com/spreadsheets/d/1rzFkEfqJGzqhJhAANs7PTpTYKmhoc2VUc4Grx-b3ISc/edit?usp=sharing). 

### Automatisk testning
Testerna körs genom komandot `rspec`. För att skapa rapport, ange: `rspec --format html --out report.html`.
***

