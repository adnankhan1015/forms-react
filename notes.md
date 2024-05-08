## What's so difficult about forms?

- At the end forms are about two main things you wanna do with them.

  1. Form Submission

  - You wanna hanlde their submission and extract the values entered by the user.
  - SUbmission is relativey `easy`.
  - Enterd values can be manages via `state` by 2-ways binding.
  - ALternatively, they can be extracted via `refs`
  - Built-in feature provided by the browser to extract and getthat data entered by the user into those form fields with help of the `formData object`

  1. Input Validation

  - You typically also want to validate the data thats provided by the user, and show some validation errors to the user. If incorrect data has been provided by the user.
  - Providng a good user experience is `tricky`.

  1. You can `validate` on every `keystroke` -> errors may be shown `too early`.
  2. You can `validate` on `lost focus` -> errors may be shown `too long`
  3. You can `validate` on `form submission` -> errors may be shown `too early`.

#### Resetting form using Refs

- This is the solution that you should use with care, because typically you should leave it up to REACT to update the DOM
- and you should not imperatively perform updates or changes as we are doing it here . e,g:`email.current.value = "";`
- It might be just a small update, but it is an update to the DOM and therefore not really recommended.
