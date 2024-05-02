---
layout: default
title: "Contact"
---

<style>
  .form-container {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background-color: #f4f4f4;
  }

  form {
    background: white;
    padding: 3em; /* Increased padding to create more space inside the border */
    border-radius: 8px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    width: 60%; /* Adjust width to suit the new padding */
    max-width: 500px; /* Adjust maximum width for aesthetic */
  }

  label {
    margin-bottom: 1em;
    display: block;
    font-size: 20px;
  }

  input[type="email"], textarea {
    width: calc(100% - 1em); /* Adjust width to be slightly smaller than form width */
    padding: 1em; /* Standard padding for a tactile area */
    margin-top: 0.5em;
    border: 1px solid #ccc;
    border-radius: 4px;
    font-size: 16px; /* Adjust font size */
  }

  button {
    width: calc(100% - 1em); /* Slightly extended width to better align with text boxes */
    padding: 1em;
    border: none;
    border-radius: 4px;
    background-color: #007BFF;
    color: white;
    cursor: pointer;
    margin-top: 1em;
    font-size: 16px;
  }

  button:hover {
    background-color: #0056b3;
  }

  textarea {
    height: 150px; /* Adjusted height */
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
