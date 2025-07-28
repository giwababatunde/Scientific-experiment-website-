# Scientific-experiment-website-
It teaches about sciencentific experiment 
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Balloon on a Bed of Pins Experiment</title>

  <!-- Font Awesome for icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background-color: #f4faff;
      color: #222;
      padding: 20px;
      line-height: 1.6;
    }

    h1 {
      color: #0a4d8c;
    }

    h2 {
      color: #1d73be;
      margin-top: 30px;
    }

    .formula {
      background: #e8f3ff;
      border-left: 6px solid #1a73e8;
      padding: 12px;
      margin: 20px 0;
      font-size: 20px;
      font-style: italic;
    }

    .note {
      background: #fff3cd;
      border-left: 6px solid #ffc107;
      padding: 15px;
      margin: 20px 0;
    }

    .login {
      text-align: right;
      margin-bottom: 15px;
    }

    .login a {
      text-decoration: none;
      color: #1d73be;
      font-weight: bold;
      font-size: 16px;
      cursor: pointer;
    }

    .login a i {
      margin-right: 5px;
    }

    .ai-buttons {
      display: flex;
      gap: 15px;
      margin-top: 15px;
    }

    .ai-buttons button {
      padding: 10px 20px;
      border: none;
      border-radius: 8px;
      color: white;
      font-size: 15px;
      cursor: pointer;
      box-shadow: 0 2px 5px rgba(0,0,0,0.2);
    }

    .chatgpt-btn {
      background: #10a37f;
    }

    .grok-btn {
      background: #4b6cb7;
    }

    /* Login popup styles */
    #loginBox {
      display: none;
      position: fixed;
      top: 20%;
      left: 50%;
      transform: translateX(-50%);
      background: #ffffff;
      padding: 25px;
      border-radius: 12px;
      box-shadow: 0 0 15px rgba(0, 0, 0, 0.3);
      z-index: 999;
      width: 300px;
    }

    #loginBox input {
      width: 100%;
      padding: 10px;
      margin-bottom: 12px;
      border: 1px solid #ccc;
      border-radius: 6px;
    }

    #loginBox button {
      padding: 10px 15px;
      margin-right: 10px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    #loginBox .submit-btn {
      background-color: #1a73e8;
      color: white;
    }

    #loginBox .close-btn {
      background-color: #ccc;
    }
  </style>
</head>
<body>

  <!-- Login Icon -->
  <div class="login">
    <a onclick="openLogin()"><i class="fas fa-sign-in-alt"></i>Login</a>
  </div>

  <!-- Login Form Popup -->
  <div id="loginBox">
    <h3>Login</h3>
    <input type="text" id="username" placeholder="Username">
    <input type="password" id="password" placeholder="Password">
    <button class="submit-btn" onclick="submitLogin()">Submit</button>
    <button class="close-btn" onclick="closeLogin()">Close</button>
  </div>

  <h1>🎈 Balloon on a Bed of Pins Experiment</h1>

  <h2>🎯 Objective:</h2>
  <p>To demonstrate how pressure is reduced when force is distributed over a larger area.</p>

  <h2>🧪 Materials:</h2>
  <ul>
    <li>1 Balloon (inflated)</li>
    <li>A board or surface with many sharp pins (arranged close together)</li>
    <li>Flat table or platform</li>
  </ul>

  <h2>🧠 What Happens?</h2>
  <p>If you press a balloon on a single pin, it pops due to high pressure on one point. But if you gently place it on many pins, it doesn't burst. Why?</p>

  <h2>📘 Explanation:</h2>
  <p>The balloon doesn’t pop because the force is spread across many pins. Each pin applies only a small portion of pressure to the surface of the balloon.</p>

  <div class="formula">
    Pressure (P) = Force (F) ÷ Area (A)
  </div>

  <p>When the area increases (many pins), the pressure at each point decreases, making it less likely for the balloon to burst.</p>

  <h2>🧪 Conclusion:</h2>
  <p>This experiment teaches the principle of pressure. It's the same reason a person can lie on a bed of nails — their weight is distributed over many points, lowering the pressure on each nail.</p>

  <div class="note">
    ⚠️ <strong>Important Safety Note:</strong><br><br>
    This is a fun experiment that also teaches real-world science! When force is spread over a large surface area, the pressure at any one point is reduced. This helps us understand the design of tools, safety gear, and surfaces like snowshoes or beds of nails.<br><br>
    However, always be careful when working with sharp objects like pins. Even though the balloon doesn't burst easily with many pins, it can still pop if too much force is applied or if pins are uneven. Make sure to test carefully and always have adult supervision if you're a student.
  </div>

  <h2>🤖 Try Our AI Helpers:</h2>
  <div class="ai-buttons">
    <button class="chatgpt-btn" onclick="window.open('https://chat.openai.com/', '_blank')">
      <i class="fas fa-robot"></i> Chat with ChatGPT
    </button>
    <button class="grok-btn" onclick="window.open('https://grok.x.com', '_blank')">
      <i class="fas fa-brain"></i> Ask Grok
    </button>
  </div>

  <!-- JavaScript Functions -->
  <script>
    function openLogin() {
      document.getElementById("loginBox").style.display = "block";
    }

    function closeLogin() {
      document.getElementById("loginBox").style.display = "none";
    }

    function submitLogin() {
      const username = document.getElementById("username").value.trim();
      const password = document.getElementById("password").value.trim();

      if (username === "" || password === "") {
        alert("Please enter both username and password.");
      } else {
        alert("Login Successful!");
        closeLogin(); // Close popup after login
      }
    }
  </script>

</body>
</html>
