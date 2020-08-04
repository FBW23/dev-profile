## Secret Mission #1 - Get the form to the president...

Create a mini React app where we can create a developer profile.

The profile for now should just contain these fields:
- firstname
- lastname
- email
- password

Use the Formik library to build and validate the form.

Use the components "Field" and "ErrorMessage" from the Formit Library.

Use the Yup library to create heavy validation rules for your input fields. 

Validation rules: 
- All fields are required 
- All fields must be strings and email must be... well... an email :) 
- The password field should have a minimum length of 3 characters and a max length of 5
- The lastname field should have a min length of 2 characters
- Provide different validation messages for required and format check

Link the schema to your Formik component. On every submit Formik will validate your fields then automatically according to this schema. Isn't that super-friendly of it?

Add a submit handler. Console.log the validated form data. Test a form submit with some dummy values.

Once your schema works: Store it as a code snippet for your reference. Recommendation: Use the VSCode Extension "Snippet Creator" from Ryan Olson.

### Bonus

Format the errors with a CSS class

Add another field: about_me - textarea - not required
- use the "as" prop of the Field component to create the textarea

Provide a format check for firstname & lastname:
- Allow letters only. No numbers and special chars
  - research Yup "match" function for applying a regular expression to a field
  - research the regular expression to match "letters only"
