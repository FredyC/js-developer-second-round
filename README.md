# Zadání:
Jako uživatel, který si chce půjčit peníze, chci mít možnost vybrat si částku a dobu splácení, abych viděl jaká bude moje měsíční splátka a úrok.

# Features:
- 2 slidery
  - 1. slider ovládá částku (amount)
  - 2. slider ovládá počet měsíců (term)
- u každého slideru je `<select>`, který zobrazuje všechny možné hodnoty
- `<select>` je propojený se sliderem - pokud se změní jeden, automaticky se mění i druhý

# Poznámky
API je dostupné na https://js-developer-second-round.herokuapp.com/api/v1/
  - https://js-developer-second-round.herokuapp.com/api/v1/application/constraints dodá hodnoty pro nastavení kalkulačky (min, max, default value, step)
  - https://js-developer-second-round.herokuapp.com/api/v1/application/first-loan-offer?amount=XX&term=YY na základě parametrů `amount` a `term` odpoví JSON objektem který obsahuje info o půjčce

# Bonus
- Use Flux (Redux) to capture the state of the application
- Use Immutable.js or Ramda to save and manipulate the state
- Use some boilerplate to kick off the project (e.g. [Este](https://github.com/este/este))
- Cache all requests so the application is more responsive to user input
- Server rendering
- Use inline styles

Example of a production application: https://www.vivus.com.mx/
