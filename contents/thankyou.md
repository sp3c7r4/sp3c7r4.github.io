---
layout: default
title: Home
---

<body>
<div class="containers">
      <section id="main_content">
        <style>
          body {
            font-family: Arial, sans-serif;
            background-color: #f9f9f9;
          }         
          .title {
            font-size: 24px;
            font-weight: bold;
            color: #fff;
          }
          .message {
            font-size: 18px;
            color: #666;
          }
          .btn { 
            background-color: transparent;
            border: 2px solid #b5e853;
            padding: 10px 20px;
            color: #b5e853;
            cursor: pointer;
          }
          .btn:hover {
            background-color: #b5e853;
            color: #fff;
          }
        </style>
<div class="contain">
          <h2 class="title">Thank You!</h2>
          <p class="message">We appreciate your submission. We'll be in touch soon.</p>
          <button class="btn" onclick="window.location.href='{{ '/' | relative_url }}'">Return to Homepage</button>
        </div>
      </section>
    </div>
  </body>