---
layout: default
title: "CV"
---

<style>
  .pdf-viewer-container {
    text-align: center;
    width: 100%;
    max-width: 800px;
    margin: 0 auto;
  }

  canvas {
    width: 100%;
    border: 1px solid #ddd;
    border-radius: 4px;
  }

  .download-button {
    display: inline-block;
    background-color: #007BFF;
    color: white;
    padding: 10px 20px;
    text-decoration: none;
    border-radius: 5px;
    cursor: pointer;
    margin-top: 10px;
  }

  .download-button:hover {
    background-color: #0056b3;
  }
</style>

<div class="pdf-viewer-container">
  <canvas id="pdfViewer"></canvas>
  <a href="{{ '/assets/cv_cha_2024.pdf' | relative_url }}" class="download-button" download>Download PDF</a>
</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/pdf.js/{{PDFJS_VERSION}}/pdf.min.js"></script>
<script>
  const url = '{{ "/assets/cv_cha_2024.pdf" | relative_url }}';

  let pdfjsLib = window['pdfjs-dist/build/pdf'];
  pdfjsLib.GlobalWorkerOptions.workerSrc = '//cdnjs.cloudflare.com/ajax/libs/pdf.js/{{PDFJS_VERSION}}/pdf.worker.min.js';

  let loadingTask = pdfjsLib.getDocument(url);
  loadingTask.promise.then(function(pdf) {
    console.log('PDF loaded');
    
    // Fetch the first page
    var pageNumber = 1;
    pdf.getPage(pageNumber).then(function(page) {
      console.log('Page loaded');
      
      var scale = 1.5;
      var viewport = page.getViewport({scale: scale});

      // Prepare canvas using PDF page dimensions
      var canvas = document.getElementById('pdfViewer');
      var context = canvas.getContext('2d');
      canvas.height = viewport.height;
      canvas.width = viewport.width;

      // Render PDF page into canvas context
      var renderContext = {
        canvasContext: context,
        viewport: viewport
      };
      var renderTask = page.render(renderContext);
      renderTask.promise.then(function () {
        console.log('Page rendered');
      });
    });
  }, function (reason) {
    // PDF loading error
    console.error(reason);
  });
</script>
