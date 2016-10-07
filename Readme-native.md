# Simple loan calculator

## The task
As a user who needs to get lend some money I would like to have the ability to choose the amount and term of the loan so that I know what will be my monthly instalment and interest.

### Features
- 2 sliders
  - 1st slider controls the `amount`
  - 2nd slider controls the `term` (number of loan)
- The calculator has a configuration. The configuration contains the minimum, maximum and step for both `amount` and `term`. It also contains the default value.
- Each slider has also a picker besides it. The picker contains all possible values (take `step` into account).
- If either of these control elements change the second one must be updated as well (slider changes -> picker is updated and vice versa).
- Display information about the loan (returned from the api) based on the `amount` and `term`.
- Add second screen with simple form (fields: first name, last name, e-mail, password, phone number, address) and third screen with summary of the data from the form and the summary of the loan.

### The API
API is available at https://js-developer-second-round.herokuapp.com/api/v1/

- https://js-developer-second-round.herokuapp.com/api/v1/application/constraints contains the configuration values for the calculator (min, max, default value, step for both `amount` and `term`)
- https://js-developer-second-round.herokuapp.com/api/v1/application/first-loan-offer?amount=1000&term=5 based on the variables `amount` and `term` it responds with a JSON object that contains all information about the offered loan.
- https://js-developer-second-round.herokuapp.com/api/v1/application/real-first-loan-offer?amount=1000&term=5 this endpoint works exactly in the same way as `/api/v1/application/first-loan-offer` the only difference being that it behaves more like a real-life service in the way that it has latency (randomly between 0 and 1000 ms)

### Bonus
- Use Flux (Redux) to capture the state of the application
- Use Immutable.js or Ramda to save and manipulate the state
- Use some boilerplate to kick off the project (e.g. [Este](https://github.com/este/este))
- Use `/api/v1/application/real-first-loan-offer` and offer should be rendered correctly (so your selected amount and term will always correspond with shown offer)

Example of a production application: https://www.vivus.com.mx/
