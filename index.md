---
layout: page
title: "About Me"
---

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

  img.wrap {
    float: left;
    margin-right: 20px; /* Creates space between the image and text/form */
    width: 150px; /* Set width to your preference */
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

Hi there!

I'm a final year Master's student in Mechanical Engineering at at TU Munich. My research interests include wearable technology, biomechanics, soft robotics and the applications of controls and machine learning in biomedical engineering.

During my Bachelor's, I researched trajectory optimisation strategies for a robotic manipulator, with a particular focus on orientation interpolation. Here, I contributed to a project that developed a new orientation interpolation algorithm and a <a href="(https://ieeexplore.ieee.org/document/10161346)">paper</a> was presented at ICRA2023 in London, UK.

In 2023, I visited the <a href="(https://www.biomechatronicslab.co.uk/)">Biomechatronics Lab</a> (Prof. Ravi Vaidyanathan) at Imperial College London to research control strategies for a lower-limb rehabilitative exoskeleton. A paper has been accepted at ICRA2024 and will be presented in Yokohama, Japan.

Currently, I am a visiting student at the <a href="(https://eng.ox.ac.uk/hbl/)">Healthcare Biorobotics Lab</a> (Prof. Liang He) at the University of Oxford as part of my Master's thesis research. The research involves fabiricating a wearable soft sensor using 3D printing-based ink writing techniques, taking inspiration from recent advances in soft sensing for soft robotics.

Feel free to contact me if you want to chat about research or anything in general! I'm always on the lookout for new ideas and possible collaborations.
