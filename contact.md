---
layout: default
title: "Contact"
---

<style>
  body {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    margin: 0;
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
  }

  form {
    background: white;
    padding: 2em;
    border-radius: 8px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    width: 300px;
  }

  label {
    margin-bottom: 1em;
    display: block;
  }

  input[type="email"], textarea {
    width: 100%;
    padding: 0.8em;
    margin-top: 0.5em;
    border: 1px solid #ccc;
    border-radius: 4px;
  }

  button {
    width: 100%;
    padding: 1em;
    border: none;
    border-radius: 4px;
    background-color: #007BFF;
    color: white;
    cursor: pointer;
    margin-top: 1em;
  }

  button:hover {
    background-color: #0056b3;
  }

  textarea {
    height: 100px;
  }
</style>

<!-- modify this form HTML and place wherever you want your form -->
<form action="https://formspree.io/f/mwkgynyl" method="POST">
  <label>
    Your email:
    <input type="email" name="email">
  </label>
  <label>
    Your message:
    <textarea name="message"></textarea>
  </label>
  <!-- your other form fields go here -->
  <button type="submit">Send</button>
</form>
