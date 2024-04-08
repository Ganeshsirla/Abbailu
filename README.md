<html>
<head>
  <meta charset="UTF-8">
  <title>Paragraph at Top</title>
  <link rel="stylesheet" href="style.css">
  <style>
    body {
  font-family: Arial, sans-serif; /* Change the font family if desired */
  margin: 0;
  padding: 0;
}

.container:hover {
    color: aqua;
    box-shadow: 0 0 10000px #03e9f4,
        0 0 10000px #03e9f4,
        0 0 10000px #03e9f4,
        0 0 10000px #03e9f4;
}

p {
  text-align: center;
  font-size: 18px;
  margin-bottom: 20px;
}
body {
    align-items: center;
    display: flex;
    font-family: sans-serif;
    font-weight: 600;
    font-size: 26px;
    height: 100vh;
    justify-content: center;
    margin: 0;
  }
  .container {
    align-items: center;
    background: #000;
    border-radius: 40px;
    box-shadow: 0 14px 28px rgba(0,0,0,0.25), 0 10px 10px rgba(0,0,0,0.22);
    display: flex;
    height: 80px;
    justify-content: center;
    position: relative;
    width: 200px;
  }
  .text {
    color: white;
    position: absolute;
    transition: opacity 300ms;
    user-select: none;
    -moz-user-select: none;
  }
  .fingerprint {
    /* height: 80px; */
    left: -8px;
    opacity: 0;
    position: absolute;
    stroke: #777;
    top: -9px;
    transition: opacity 1ms;
  }
  .fingerprint-active {
    stroke: #fff;
  }
  .fingerprint-out {
    opacity: 1;
  }
  .odd {
    stroke-dasharray: 0px 50px;
    stroke-dashoffset: 1px;
    transition: stroke-dasharray 1ms;
  }
  .even {
    stroke-dasharray: 50px 50px;
    stroke-dashoffset: -41px;
    transition: stroke-dashoffset 1ms;
  }
  .ok {
    opacity: 0;
  }
  .active.container {
    animation: 6s Container;
  }
  .active .text {
    opacity: 0;
    animation: 6s Text forwards;
  }
  .active .fingerprint {
    opacity: 1;
    transition: opacity 300ms 200ms;
  }
  .active .fingerprint-base .odd {
    stroke-dasharray: 50px 50px;
    transition: stroke-dasharray 800ms 100ms;
  }
  .active .fingerprint-base .even {
    stroke-dashoffset: 0px;
    transition: stroke-dashoffset 800ms;
  }
  .active .fingerprint-active .odd {
    stroke-dasharray: 50px 50px;
    transition: stroke-dasharray 2000ms 1500ms;
  }
  .active .fingerprint-active .even {
    stroke-dashoffset: 0px;
    transition: stroke-dashoffset 2000ms 1300ms;
  }
  .active .fingerprint-out {
    opacity: 0;
    transition: opacity 300ms 4100ms;
  }
  .active .ok {
    opacity: 1;
    animation: 6s Ok forwards;
  }
  @keyframes Container {
    0% { width: 200px }
    6% { width: 80px }
    71% { transform: scale(1); }
    75% { transform: scale(1.2); }
    77% { transform: scale(1); }
  
    94% { width: 80px }
    100% { width: 200px }
  }
  @keyframes Text {
    0% { opacity: 1; transform: scale(1); }
    6% { opacity: 0; transform: scale(0.5); }
  
    94% { opacity: 0; transform: scale(0.5); }
    100% { opacity: 1; transform: scale(1); }
  }
  @keyframes Ok {
    0% { opacity: 0 }
    70% { opacity: 0; transform: scale(0); }
    75% { opacity: 1; transform: scale(1.1); }
    77% { opacity: 1; transform: scale(1); }
    92% { opacity: 1; transform: scale(1); }
    96% { opacity: 0; transform: scale(0.5); }
    100% { opacity: 0 }
  }
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
