# Testspecifikation

### Allmänna testprocedurer
Testningen kommer främst att ske med automatisk testning. Det gäller både back-end- och front-end-delen av applikationen. Det kommer att ske tester av modellklasser, controllers samt integrationstestning.

Manuella tester kommer även att utföras gällande större delar av systemet, där jag med hjälp av systemtester testar en större del av tjänsten, exempelvis ett baskkrav.

### Testmiljö
Testningen av back-end-delen kommer att testas med testramverket [RSpec](http://rspec.info/) för Ruby on Rails, samt med manuella tester.

Testning av React-komponenter sker med manuella tester.

Manuell testning kommer att ske på olika moderna webbläsare i flera enheter.

### Manuell testning

### Automatisk testning
Testerna körs genom komandot `rspec`. För att skapa rapport, ange: `rspec --format html --out report.html`.
***

