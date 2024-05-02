---
layout: default
title: "Contact"
---

<style>
  /* Minimal CSS for centering the form */
  .form-container {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
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
    font-size: 16px; /* Larger font for readability */
  }

  input[type="email"], textarea {
    width: 100%;
    padding: 0.8em;
    margin-top: 0.5em;
    border: 1px solid #ccc;
    border-radius: 4px;
    font-size: 16px; /* Larger font for readability */
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
    font-size: 16px; /* Larger font for readability */
  }

  button:hover {
    background-color: #0056b3;
  }

  textarea {
    height: 150px; /* Larger textarea for more message space */
  }
</style>

<!-- Container for the form to center it -->
<div class="form-container">
  <form action="https://formspree.io/f/mwkgynyl" method="POST">
    <label>
      Your email:
      <input type="email" name="email">
    </label>
    <label>
      Your message:
      <textarea name="message"></textarea>
    </label>
    <button type="submit">Send</button>
  </form>
</div>
