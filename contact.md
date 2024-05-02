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
    padding: 2em;
    border-radius: 8px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    width: 80%; /* Maintains a wider form */
    max-width: 600px; /* Controls maximum width for larger screens */
  }

  label {
    margin-bottom: 1em;
    display: block;
    font-size: 20px; /* Increased font size for better readability */
  }

  input[type="email"], textarea {
    width: 100%;
    padding: 1.5em; /* Increased padding for a bigger, more tactile area */
    margin-top: 0.5em;
    border: 1px solid #ccc;
    border-radius: 4px;
    font-size: 18px; /* Larger font size for inside the fields */
  }

  button {
    width: 100%;
    padding: 1.5em; /* Larger padding for a bigger, more clickable button */
    border: none;
    border-radius: 4px;
    background-color: #007BFF;
    color: white;
    cursor: pointer;
    margin-top: 1em;
    font-size: 18px; /* Larger font size for button text */
  }

  button:hover {
    background-color: #0056b3;
  }

  textarea {
    height: 250px; /* Increased height to allow more text */
  }

  img.wrap {
    float: left;
    margin-right: 20px; /* Maintains space between the image and form */
    width: 150px; /* Set width */
    height: auto; /* Maintains aspect ratio */
  }

</style>

<!-- Image positioned to float left with text wrapping around it -->
<img src="/assets/1698182793744 (1).jpg" alt="Descriptive Text of Image" class="wrap">

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
