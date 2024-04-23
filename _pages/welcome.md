---
permalink: /
layout: home
title: Welcome
# list_title: My blog posts
---

```html
<!DOCTYPE html>
<html>
<head>
  <style>
    @keyframes flow {
      0% { background-position: 0 0; }
      100% { background-position: 20px 0; }
    }

    td {
      background-image: linear-gradient(90deg, rgba(255,255,255,0) 50%, rgba(255,255,255,0.5) 50%);
      background-size: 20px 20px;
      animation: flow 1s infinite linear;
    }
  </style>
</head>
<body>
  <div style="font-family: monospace;">
    <table>
      <tr>
        <td>Process A</td>
        <td style="color: #00FF00;">▊</td>
      </tr>
      <tr>
        <td>Process B</td>
        <td style="color: #00FF00;">▊</td>
      </tr>
      <tr>
        <td>Process C</td>
        <td style="color: #00FF00;">▊</td>
      </tr>
      <tr>
        <td>Process D</td>
        <td style="color: #00FF00;">▊</td>
      </tr>
      <tr>
        <td>Process E</td>
        <td style="color: #00FF00;">▊</td>
      </tr>
    </table>
  </div>
</body>
</html>
