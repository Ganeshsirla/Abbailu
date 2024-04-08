<html>
<head>
  <meta charset="UTF-8">
  <title>Paragraph at Top</title>
  <link rel="stylesheet" href="style.css">
  <style>
    .thank-you {
      position: fixed;
      top: 10px;
      right: 10px;
      background-color: #f0f0f0;
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
  </style>
</head>
<body>

<div class="container" onclick="navigateToPage()">
  <span class="text">CLICK HERE👇</span>
  <svg class="fingerprint fingerprint-base" xmlns="http://www.w3.org/2000/svg" width="100" height="100" viewBox="0 0 100 100">
    <!-- SVG paths for fingerprint animation -->
  </svg>
  <svg class="fingerprint fingerprint-active" xmlns="http://www.w3.org/2000/svg" width="100" height="100" viewBox="0 0 100 100">
    <!-- SVG paths for active fingerprint animation -->
  </svg>
  <svg class="ok" xmlns="http://www.w3.org/2000/svg" width="100" height="100" viewBox="0 0 100 100"><path d="M34.912 50.75l10.89 10.125L67 36.75" fill="none" stroke="#fff" stroke-width="6"/></svg>
</div>

<div id="thankYouMessage" class="thank-you" style="display:none;">
  Thank you for visiting!
</div>

<div class="welcome-message" style="position: fixed; bottom: 500px; font-size: 8px;width: 50%;">
  <h1> HI...This is GANESH SIRLA
  Welcome to my website</h1>
</div>

<script>
  function navigateToPage() {
    // Change the URL to the desired page
    window.location.href = "https://ganeshsirla.github.io/Jntu-gv/";
    
    // Show the thank you message
    document.getElementById("thankYouMessage").style.display = "block";
  }
</script>

</body>
</html>
