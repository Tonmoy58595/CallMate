
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CallMate - Startup Page</title>
  <style>
    /* General Reset */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    /* Body and Font */
    body {
      font-family: Arial, sans-serif;
      background-color: #4A90E2;  /* Sky Blue */
      color: #fff;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      text-align: center;
    }

    /* Container */
    .container {
      background-color: #333333;  /* Dark Charcoal */
      padding: 40px;
      border-radius: 12px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    }

    /* Heading */
    h1 {
      font-size: 36px;
      margin-bottom: 20px;
      color: #FFBB33;  /* Vibrant Yellow */
    }

    /* Tagline */
    h3 {
      font-size: 22px;
      margin-bottom: 30px;
      font-weight: 300;
    }

    /* Call to Action Button */
    .cta-button {
      padding: 15px 30px;
      font-size: 18px;
      color: #fff;
      background-color: #FFBB33;  /* Vibrant Yellow */
      border: none;
      border-radius: 5px;
      cursor: pointer;
      transition: background-color 0.3s ease;
      width: 100%;
    }

    /* Button Hover Effect */
    .cta-button:hover {
      background-color: #f79e42;
    }

    /* Loading Animation */
    .loader {
      border: 8px solid #f3f3f3; /* Light Gray */
      border-top: 8px solid #4A90E2; /* Sky Blue */
      border-radius: 50%;
      width: 50px;
      height: 50px;
      animation: spin 2s linear infinite;
      margin-top: 20px;
    }

    @keyframes spin {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }

    /* Responsive Design */
    @media (max-width: 600px) {
      .container {
        padding: 20px;
      }

      h1 {
        font-size: 28px;
      }

      h3 {
        font-size: 18px;
      }

      .cta-button {
        font-size: 16px;
      }
    }
  </style>
</head>
<body>

  <!-- Main Container -->
  <div class="container">
    <h1>Welcome to CallMate</h1>
    <h3>Your ultimate communication companion</h3>

    <!-- Call to Action Button -->
     <div>
      <a href="login page.html">
        <button class="cta-button" onclick="startApp()">Start CallMate </button>
      </a>
      
    </div>
    <!-- Loader Animation -->
    <div id="loader" class="loader" style="display: none;"></div>
  <script>
    // Function to simulate the startup action and show the loader
    function startApp() {
      // Hide the button and show the loader
      document.querySelector('.cta-button').style.display = 'none';
      document.getElementById('loader').style.display = 'block';

      // Simulate a short delay before transitioning to the main app
      setTimeout(() => {
        window.location.href = "mainapp.html";  // Redirect to the main app page (replace with your actual app page)
      }, 3000);  // 3 seconds delay
    }
  </script>

