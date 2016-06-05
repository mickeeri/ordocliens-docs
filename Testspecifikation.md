# Testspecifikation

### Allmänna testprocedurer
Testning bör ske i slutet av varje iteration. Det genomförs genom att automatiska tester körs och manuella testfall genomgås. För att säkerställa att alla krav testas finns en kolum i kravspecifikationen där det specificeras om kravet har testats. 

I största möjligaste mån kommer automatiska tester att användas. Det gäller främst back-end-delen. Front-end-delen som består mest av React-komponenter har visat sig vara svår att testa automatiskt. Hittade sent en lösning för att testa React-komponenterna och därför utgör de manuella testerna huvuddelen av testningen av front-end-delen. 

### Testmiljö
Automatisk testning sker med testramverket [RSpec](http://rspec.info/) för Ruby on Rails.

Testning av vyer och React-komponenter sker med Rspec tillsammans med [Capybara](https://github.com/jnicklas/capybara). För att kunna testa JavaScript används en driver som heter Poltergeist. Den installeras enligt [dessa](http://stackoverflow.com/questions/8778513/how-can-i-setup-run-phantomjs-on-ubuntu) instruktioner. Ändra till aktuell version och lägg till `gem 'poltergeist'` i projektes Gemfile och kör `bundle install`.

Manuell testning kommer att ske på olika moderna webbläsare.

### Manuell testning
Manuella testfalls genomförande och resultat presenteras f.r.o.m Iteration 8 i ett [Google Sheets dokument](https://docs.google.com/spreadsheets/d/1rzFkEfqJGzqhJhAANs7PTpTYKmhoc2VUc4Grx-b3ISc/edit?usp=sharing).

### Automatisk testning
Testerna körs genom kommandot `rspec`. För att skapa rapport, ange: `rspec --format html --out report.html`. Den kan sedan presenteras genom [Github HTML Preview](https://htmlpreview.github.io/).

