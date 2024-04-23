**`code block`**
`import data from....`

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ASCII Animation</title>
<style>
  .ascii-animation {
    font-family: monospace;
    font-size: 11px; /* Adjust the font size */
    line-height: 6px; /* Adjust the line height */
    white-space: pre;
  }
  .white {
    color: #FFFFFF;
  }
</style>
</head>
<body>
<div class="ascii-animation" id="ascii-animation">
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

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ASCII Animation</title>
<style>
  pre {
    font-family: monospace;
    font-size: 11px; /* Adjust the font size */
    line-height: 1.2; /* Adjust the line height */
    border: 1px solid #000; /* Add a border around the ASCII art */
    padding: 10px; /* Add some padding inside the border */
    display: inline-block; /* Make the pre tag size to its content */
    color: #2e37ed; /* Set the text color to iridescent blue */
  }
  .blink {
    animation: blink-animation 1s infinite;
  }
  @keyframes blink-animation {
    50% {
      opacity: 0;
    }
  }
</style>
</head>
<body>
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
</body>
</html>