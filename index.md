<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ASCII Animation</title>
<style>
  .container {
    display: flex; /* Use flexbox for layout */
    /* justify-content: space-between; */ /* Remove this line to place elements next to each other */
  }
  .ascii-animation {
    font-family: monospace;
    font-size: 8px; /* Adjust the font size */
    line-height: 6px; /* Adjust the line height */
    white-space: pre;
  }
  .white {
    color: #FFFFFF;
  }
  @keyframes blink {
    0% { opacity: 1; }
    50% { opacity: 0; }
    100% { opacity: 1; }
  }
  .blink {
    animation: blink 1s infinite;
  }
  pre {
    margin: 0; /* Remove default margins */
    color: #2e37ed; /* Set the text color to iridescent blue */
  }
  .second-output {
    margin-top: 6px; /* Move the second output down by 2px */
  }
</style>
</head>
<body>
<div class="container">
  <div>
    <pre>
      ┌───────────────────┐
      │               ─ x │
      ├───────────────────┤
      │                   │
      │ -> STATUS         │
      │ ONLINE            │
      │ DATAMACHINE-001-1 │
      │                   │
      │ -> <span class="blink">▉</span>              │
      └───────────────────┘
    </pre>
  </div>
  <div class="ascii-animation second-output" id="ascii-animation">
    <span>▊▊▊▊▊▊▊▊▊▊▊▊<span class="white">⎕⎕⎕⎕⎕</span>▊▊▊▊▊</span><br>
    <span>▊▊▊▊▊▊▊▊▊▊▊▊▊<span class="white">⎕⎕⎕</span>▊▊⎕⎕⎕⎕</span><br>
    <span>▊▊▊▊▊▊▊▊▊▊<span class="white">⎕⎕⎕⎕⎕⎕⎕⎕</span>▊▊▊▊</span><br>
    <span>▊▊▊▊▊▊▊▊▊ <span class="white">⎕⎕⎕⎕⎕⎕⎕⎕</span>▊▊▊▊</span><br>
    <span>▊▊▊▊▊▊▊▊▊▊<span class="white">⎕⎕⎕⎕⎕⎕⎕⎕</span>▊▊▊▊</span><br>
    <span>▊▊▊▊▊▊▊▊▊▊<span class="white">⎕⎕⎕⎕⎕⎕⎕⎕</span>▊▊▊▊</span><br>
    <span>▊▊▊▊▊▊▊▊▊▊<span class="white">⎕⎕⎕⎕⎕⎕⎕⎕</span>▊▊▊▊</span><br>
    <span>▊▊▊▊▊▊▊▊▊▊<span class="white">⎕⎕⎕⎕⎕⎕⎕⎕</span>▊▊▊▊</span><br>
    <span>▊▊▊▊▊▊▊▊▊▊<span class="white">⎕⎕⎕⎕⎕⎕⎕⎕</span>▊▊▊▊</span><br>
    <span>▊▊▊▊▊▊▊▊▊▊<span class="white">⎕⎕⎕⎕⎕⎕⎕⎕</span>▊▊▊▊</span><br>
    <span>▊▊▊▊▊▊▊▊▊▊<span class="white">⎕⎕⎕⎕⎕⎕⎕⎕</span>▊▊▊▊</span><br>
    
  </div>
</div>
<script>
  const rows = document.querySelectorAll('.ascii-animation span');
  let indices = Array.from({length: rows.length}, () => Math.floor(Math.random() * rows[0].textContent.length));

  function animateRows() {
    rows.forEach((row, rowIndex) => {
      let content = '';
      for (let i = 0; i < row.textContent.length; i++) {
        content += (i === indices[rowIndex]) ? '<span class="white">⎕</span>' : '▊';
      }
      row.innerHTML = content;
    });
    indices = indices.map(index => (index + 1) % rows[0].textContent.length);
  }

  setInterval(animateRows, 200); // Adjust the interval for speed
</script>
</body>
</html>
