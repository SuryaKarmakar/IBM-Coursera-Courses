# Additional HTML Elements: HTML Fieldset and Legend Tag:

## Special HTML Elements:

In this section, you will explore two tags found within the \<form\> tag, namely the \<fieldset\> and \<legend\> tags.

## fieldset tag:

1. the HTML \<fieldset\> tag is found within the \<form\> tag and is used to group related elements in an HTML form, often by enclosing them within a box.
2. There is no restriction to the kind of elements that can be inside a fieldset, but they are mostly used to group related input type of elements, as shown in the example below.
3. The fieldset element is especially useful in large forms, where readability and ease of access can be improved with segmentation. Browsers will most likely render a frame around the grouped controls.

## Attributes:

1. disabled: It specifies that the elements belonging to the fieldset should be disabled.
2. form: It specifies the id of the form that the fieldset is to be considered a part of.
3. name: It specifies the name for the fieldset.

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>The fieldset element</h1>

    <form>
      <fieldset name="personal_details">
        <label for="fname">First name:</label>
        <input type="text" id="fname" name="fname" /><br />
        <label for="lname">Last name:</label>
        <input type="text" id="lname" name="lname" /><br />
        <label for="email">Email:</label>
        <input type="email" id="email" name="email" /><br />
        <label for="phone">Phone Number:</label>
        <input type="tel" id="phone" name="phone" /><br />
      </fieldset>

      <br />

      <fieldset name="professional_details">
        <label for="occupation">Occupation:</label>
        <input type="text" id="occupation" name="occupation" /><br />
        <label for="company">Company:</label>
        <input type="text" id="company" name="company" /><br />
        <label for="start">Start Date:</label>
        <input type="date" id="start" name="start" /><br />
        <label for="end">End Date:</label>
        <input type="date" id="end" name="end" /><br />
      </fieldset>
      <br />
      <input type="submit" value="Submit" />
    </form>
  </body>
</html>
```

## legend tag:

A fieldset can additionally have a title or name, which can be provided by legend. The \<legend\> tag is used with the \<fieldset\> element as a first child (the first inner tag) to define the caption for the grouped related fields by using the \<legend\> tag with \<fieldset\> elements, it is easy to understand the purpose of grouped form elements.

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>The fieldset element</h1>

    <form>
      <fieldset name="personal_details">
        <legend>Personal Details</legend>

        <label for="fname">First name:</label>
        <input type="text" id="fname" name="fname" /><br />
        <label for="lname">Last name:</label>
        <input type="text" id="lname" name="lname" /><br />
        <label for="email">Email:</label>
        <input type="email" id="email" name="email" /><br />
        <label for="phone">Phone Number:</label>
        <input type="tel" id="phone" name="phone" /><br />
      </fieldset>

      <br />

      <fieldset name="professional_details">
        <legend>Professional Details</legend>

        <label for="occupation">Occupation:</label>
        <input type="text" id="occupation" name="occupation" /><br />
        <label for="company">Company:</label>
        <input type="text" id="company" name="company" /><br />
        <label for="start">Start Date:</label>
        <input type="date" id="start" name="start" /><br />
        <label for="end">End Date:</label>
        <input type="date" id="end" name="end" /><br />
      </fieldset>
      <br />
      <input type="submit" value="Submit" />
    </form>
  </body>
</html>
```
