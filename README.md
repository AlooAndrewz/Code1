<!DOCTYPE html>
<html>
<head>
  <title>accordionTaps2|ByAndy</title>
  <style type="text/css">
    * {
      box-sizing: border-box;
    }
    html, body {
      margin: 0;
      padding: 0;
    }
    .container {
      margin: 15px;
    }
    input[type="radio"] {
      display: none;
    }
    .container {
      border: 1px solid black;
      border-radius: 5px;
    }
    label {
      display: block;
      padding: 10px;
      border-bottom: 1px solid black;
      color: white;
      background: #0076ff;
      z-index: 2; /* put it above the accordion content */
    }
    .accordion:last-child > label, .accordion:last-child > .accordion-content {
      border: none;
    }
    .accordion-content {
      border-bottom: 1px solid black;
      padding: 0;
      opacity: 0;
      max-height: 0;
      overflow: hidden;
      z-index: -1;
      transition: 0.3s linear;
    }
    input:checked ~ .accordion-content {
      padding: 15px;
      opacity: 1;
      max-height: 500px;
      z-index: 1;
    }
  </style>
</head>
<body>
  <div class="container">
  
  <div class="accordion">
    <input type="radio" name="accordion" id="accordion1" checked>
      <label for="accordion1"> » Accordion #1 </label>
      <div class="accordion-content">
        Hello, I am Aloo
      </div>
  </div>
  
  <div class="accordion">
    <input type="radio" name="accordion" id="accordion2">
      <label for="accordion2"> » Accordion #2 </label>
      <div class="accordion-content">
      I'm just from Kisumu Kenya 
      </div>
  </div>
  
  <div class="accordion">
    <input type="radio" name="accordion" id="accordion3">
      <label for="accordion3"> » Accordion #3 </label>
      <div class="accordion-content">
        Nd this is my first HTML CSS "project"
      </div>
  </div>
  
  <div class="accordion">
    <input type="radio" name="accordion" id="accordion4">
      <label for="accordion4"> » Accordion #4 </label>
      <div class="accordion-content">
        Well, With time I will develop cool staff
      </div>
  </div>
  
  </div>
</body>
</html>
