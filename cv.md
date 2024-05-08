---
layout: default
title: "Your Page Title"
---

<style>
  .pdf-viewer-container {
    text-align: center;
    margin-bottom: 20px;
  }

  .download-button {
    background-color: #007BFF;
    color: white;
    padding: 10px 20px;
    text-decoration: none;
    border-radius: 5px;
    cursor: pointer;
  }

  .download-button:hover {
    background-color: #0056b3;
  }

  embed {
    width: 100%;
    height: 500px;
  }
</style>

<div class="pdf-viewer-container">
  <embed src="{{ '/assets/cv_cha_2024.pdf' | relative_url }}" width="100%" height="500px" type="application/pdf">
  <a href="{{ '/assets/cv_cha_2024.pdf' | relative_url }}" class="download-button" download>Download PDF</a>
</div>
