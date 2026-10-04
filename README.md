<!DOCTYPE html>
<html>
<head>
    <title>LegalEase - Legal Help</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            background: #f4f6f9;
        }
        header {
            background: #17365d;
            color: white;
            text-align: center;
            padding: 20px;
        }
        nav {
            background: #24527a;
            padding: 12px;
            text-align: center;
        }
        nav a {
            color: white;
            margin: 15px;
            text-decoration: none;
        }
        .container {
            padding: 25px;
            text-align: center;
        }
        .box {
            background: white;
            padding: 20px;
            margin: 15px auto;
            max-width: 500px;
            border-radius: 10px;
            box-shadow: 0 2px 8px #ccc;
        }
        input, textarea, button {
            width: 90%;
            padding: 10px;
            margin: 8px;
        }
        button {
            background: #17365d;
            color: white;
            border: none;
            cursor: pointer;
        }
        footer {
            background: #17365d;
            color: white;
            text-align: center;
            padding: 12px;
        }
    </style>
</head>
<body>

<header>
    <h1>LegalEase</h1>
    <p>Your Simple Legal Information Platform</p>
</header>

<nav>
    <a href="#home">Home</a>
    <a href="#services">Services</a>
    <a href="#contact">Contact</a>
</nav>

<div class="container" id="home">
    <h2>Welcome to LegalEase</h2>
    <p>Understand your legal rights and get basic legal information.</p>
</div>

<div class="box" id="services">
    <h2>Our Services</h2>
    <p>📘 Legal Information</p>
    <p>⚖️ Basic Legal Guidance</p>
    <p>📄 Document Information</p>
    <p>👨‍⚖️ Lawyer Consultation Requests</p>
</div>

<div class="box" id="contact">
    <h2>Contact Us</h2>
    <input type="text" id="name"
           placeholder="Enter your name">
    <input type="email" id="email"
           placeholder="Enter your email">
    <textarea id="message"
              placeholder="Enter your question"></textarea>
    <button onclick="sendMessage()">Submit</button>
    <p id="result"></p>
</div>

<footer>
    <p>© 2026 LegalEase. All Rights Reserved.</p>
</footer>

<script>
function sendMessage() {
    let name = document.getElementById("name").value;
    let email = document.getElementById("email").value;
    let message = document.getElementById("message").value;

    if (name === "" || email === "" || message === "") {
        document.getElementById("result").innerText =
            "Please fill all fields.";
    } else {
        document.getElementById("result").innerText =
            "Thank you, " + name +
            "! Your message has been received.";
    }
}
</script>

</body>
</html>
