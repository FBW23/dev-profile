## Secret Mission #2 - Make the form heavier...

Let's add some fields specific for a developer profile.

Add a checkbox group with technologies:
- you can choose from: HTML / CSS, SCSS, Bootstrap, React, ExpressJS, JWT, Formik, Git... and whatever else you find learn-worthy :)

Add a SelectBox "specialization" with possible fields: noob, frontend, backend, fullstack 

Check on submit if you receive your entered values.

## Bonus 2

Provide a password format check:
- Password must start with a letter and must end with a number
- Use the Yup "match" function and research which regular expression to apply

Research how to do a password confirmation field (so matching your password against a password confirm field) using the `Yup.ref()` helper.

The masterclass: Research a "password strength" regex and test it out

## Bonus 3

We want to be able to store our profile info.

We do not have an API for now. So we store it locally.

OnSubmit: Store your developer profile values in localStorage 
=> localStorage.setItem(....) => you remember that localStorage can only store STRINGS, right? JSON.stringify will be your friend...

On load of your form: Load the initial form data from localStorage into your initialValues object.

Eeeeh.... how to load data again "after first render"?

In class components: componentDidMount
In functional component: useEffect hook

