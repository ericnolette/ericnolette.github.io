---
permalink: /about
layout: page
title: About
---

<!DOCTYPE html>
<html>
<head>
  <style>
    @keyframes flow {
      0% { background-position: 0 0; }
      100% { background-position: 20px 0; }
    }

    .green-status {
      color: #00FF00;
      background-image: linear-gradient(90deg, rgba(255,255,255,0) 50%, rgba(255,255,255,0.5) 50%);
      background-size: 20px 20px;
      animation: flow 1s infinite linear;
      padding: 5px; /* Add padding for spacing */
    }

    table {
      border-collapse: collapse; /* Remove border spacing */
    }

    td {
      border: none; /* Remove cell borders */
    }
  </style>
</head>
<body>
  <div style="font-family: monospace;">
    <table>
      <tr>
        <td>Process A</td>
        <td class="green-status">▊</td>
        <td class="green-status">▊</td>
        <td class="green-status">▊</td>
      </tr>
      <tr>
        <td>Process B</td>
        <td class="green-status">▊</td>
        <td class="green-status">▊</td>
        <td class="green-status">▊</td>
      </tr>
      <tr>
        <td>Process C</td>
        <td class="green-status">▊</td>
        <td class="green-status">▊</td>
        <td class="green-status">▊</td>
      </tr>
      <tr>
        <td>Process D</td>
        <td class="green-status">▊</td>
        <td class="green-status">▊</td>
        <td class="green-status">▊</td>
      </tr>
      <tr>
        <td>Process E</td>
        <td class="green-status">▊</td>
        <td class="green-status">▊</td>
        <td class="green-status">▊</td>
      </tr>
    </table>
  </div>
</body>
</html>

