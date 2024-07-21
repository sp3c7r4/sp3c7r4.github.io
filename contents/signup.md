---
layout: default
title: Home
---


<style>
 .contain {
    max-width: 500px;
    margin: 40px auto;
    padding: 20px;
    background-color: #2f343f; /* dark gray background */
    border: 1px solid #b5e853; /* green border */
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
  }
 .form-group {
    margin-bottom: 20px;
  }
 .form-control {
    background-color: #3b4048; /* dark gray input background */
    border: 1px solid #b5e853; /* green border */
    color: #fff; /* white text */
    padding: 10px;
  }
 .form-control::placeholder {
    color: #999; /* light gray placeholder text */
  }
 .btn {
    background-color: transparent; /* green button background */
    color: #fff; /* white button text */
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    outline: 2px solid #b5e853; /* add an outline around the button */
    outline-offset: 2px;
  }
 .btn:hover {
    background-color: #8bc34a; /* lighter green button background on hover */
  }
</style>
<script>
  document.getElementById('myForm').addEventListener('submit', function(e) {
    e.preventDefault();
    fetch(e.target.action, {
      method: 'POST',
      body: new FormData(e.target),
    }).then(() => {
      window.location.href = 'http://127.0.0.1:4000/contents/thankyou.html';
    });
  });
</script>
<style>
        /* Expand the width of the input box */
        input[type="text"], button, textarea, input[type="email"] {
            width: 100%; /* Full width of the container */
            max-width: 600px; /* Max width of the input box */
            padding: 10px;
            margin: none; /* Border color */
            border-radius: 5px; /* Rounded corners */
            box-sizing: border-box; /* Include padding and border in width */
            font-size: 16px; /* Font size */
        }
        input[type="text"] {
            margin-bottom: 10px;
        }
</style>

<form id="myForm"  action="https://formsubmit.co/69a44903436fc486d48c98f3d78a2b0d" method="POST">
<input type="hidden" name="_next" value="{{ 'https://sp3c7r4.github.io/contents/thankyou' | relative_url }}">
  <div class="contain">
    <h1 id="edits" style="color: #b5e853;"><b>Sp3c7r4 - Contact Form</b></h1>
    <div class="form-group">
      <div class="form-row">
        <div class="col">
          <input id=name type="text" name="name" class="form-control" placeholder="Full Name" required>
        </div>
        <div class="col">
          <input id="email" type="email" name="email" class="form-control" placeholder="Email Address" required>
        </div>
      </div>
    </div>
    <div class="form-group">
      <textarea placeholder="Your Message" class="form-control" name="message" rows="10" required></textarea>
    </div>
    <button type="submit" class="btn">Submit Form</button>
  </div>
</form>