# 📑 Forms Cheat Sheet

## 📌 Terms

- **Check boxes**
- **CSS frameworks**
- **Data validation**
- **Data lists**
- **Fieldsets**
- **Hidden fields**
- **HTTP method**
- **Input fields**
- **Input controls**
- **Radio buttons**
- **Sliders**
- **Text areas**

---

## 📋 Summary

- **Label elements** improve accessibility. Clicking a label will focus the associated input field.
- The `<input>` element is used to collect user data. The `type` attribute determines the input field type, such as:
  - `text`
  - `password`
  - `email`
  - `checkbox`
  - `radio`
  - `range`
  - `date`
  - `file`
  - etc.
- **Data lists** provide a suggestion list for autocompletion.
- **Dropdown lists** use the `<select>` element, containing `<option>` elements.
- **Fieldsets** (`<fieldset>`) and `<legend>` group related input fields. The `<section>` element can also be used for grouping.
- **Hidden fields** store data without displaying it. Do not store sensitive information in hidden fields, as they can be accessed via the page source.
- **Always validate form data** to prevent security risks and data corruption.
- **HTML5 Built-in Validation:** Common validation attributes:
  - `required`
  - `minlength`
  - `maxlength`
  - `min`
  - `max`
- **Form Submission:**
  - The `action` attribute defines where data is sent.
  - The `method` attribute specifies how data is sent (`GET` or `POST`).
- **GET vs POST Methods:**
  - **GET:** Form data is included in the URL as query parameters. Ideal for bookmarking pages.
  - **POST:** Form data is included in the request body. Best for updating or sending sensitive data.
- **Form Backend Service:** Use [Formspree](https://formspree.io) to handle form submissions easily.

---

## 🎨 CSS Cheat Sheet

### 📌 Forms

```html
<form action="https://formspree.io/..." method="POST">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name" required />
  <button type="submit">Register</button>
</form>
```

### 📌 Inputs

```html
<input type="email" placeholder="Enter your email" />
<input type="password" placeholder="Enter your password" />
<input type="checkbox" /> Subscribe to newsletter
<input type="radio" name="gender" value="male" /> Male
<input type="radio" name="gender" value="female" /> Female
<input type="range" min="0" max="100" />
<input type="date" />
<input type="file" />
```

### 📌 Grouping Fields

```html
<fieldset>
  <legend>Contact</legend>
  <input type="text" placeholder="First Name" />
  <input type="text" placeholder="Last Name" />
</fieldset>
```

### 📌 Data Validation

```html
<input type="number" min="0" max="5" required />
<input type="text" minlength="3" maxlength="50" required />
```
