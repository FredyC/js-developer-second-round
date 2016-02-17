# Zadání
Jako uživatel, který si chce půjčit peníze, chci mít možnost vybrat si částku a dobu splácení, abych viděl jaká bude moje měsíční splátka a úrok.

## Features
- 2 slidery
  - slider ovládá částku (amount)
  - slider ovládá počet měsíců (term)
- u každého slideru je `<select>`, který zobrazuje všechny možné hodnoty
- `<select>` je propojený se sliderem - pokud se změní jeden, automaticky se mění i druhý

## Poznámky
API je dostupné na https://js-developer-second-round.herokuapp.com/api/v1/
  - https://js-developer-second-round.herokuapp.com/api/v1/application/constraints dodá hodnoty pro nastavení kalkulačky (min, max, default value, step)
  - https://js-developer-second-round.herokuapp.com/api/v1/application/first-loan-offer?amount=1000&term=5 na základě parametrů `amount` a `term` odpoví JSON objektem který obsahuje info o půjčce

  - https://js-developer-second-round.herokuapp.com/api/v1/application/real-first-loan-offer?amount=1000&term=5 tento endpoint funguje úplně stejně jako `/api/v1/application/first-loan-offer` s tím, že vrací odpovědi jako normální server (včetně nějaké latence)

## Bonus
- Use Flux (Redux) to capture the state of the application
- Use Immutable.js or Ramda to save and manipulate the state
- Use some boilerplate to kick off the project (e.g. [Este](https://github.com/este/este))
- Use `/api/v1/application/real-first-loan-offer` and offer should be rendered correctly (so your selected amount and term will allways correspond with shown offer)
- Cache all requests so the application is more responsive to user input
- Server rendering
- Use inline styles

Example of a production application: https://www.vivus.com.mx/
