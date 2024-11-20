<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Robe Secondary School - Student Info System</title>
  <style>
    /* Base CSS Reset */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Arial', sans-serif;
      background-color: #f2f4f9;
      color: #333;
      line-height: 1.6;
    }

    /* Header Styling */
    header {
      background: linear-gradient(to right, #4b6cb7, #182848);
      padding: 20px;
      position: relative;
      z-index: 10;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    }

    .profile {
      position: absolute;
      top: 20px;
      right: 20px;
      display: flex;
      align-items: center;
      color: white;
      font-weight: bold;
      font-size: 18px;
    }

    .profile img {
      width: 40px;
      height: 40px;
      border-radius: 50%;
      margin-right: 10px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.3);
    }

    nav ul {
      display: flex;
      justify-content: center;
      list-style-type: none;
      padding: 10px 0;
    }

    nav ul li {
      margin: 0 20px;
    }

    nav ul li a {
      text-decoration: none;
      color: white;
      font-size: 18px;
      font-weight: bold;
      padding: 5px 15px;
      border-radius: 4px;
      transition: background-color 0.3s ease;
    }

    nav ul li a:hover {
      background-color: #ff7f50;
    }

    /* Main Hero Section */
    .hero {
      background: url('https://via.placeholder.com/1500x700') no-repeat center center/cover;
      color: white;
      text-align: center;
      padding: 100px 20px;
      position: relative;
    }

    .hero h1 {
      font-size: 48px;
      text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
      margin-bottom: 20px;
    }

    .hero p {
      font-size: 20px;
      max-width: 800px;
      margin: 0 auto;
      text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.3);
    }

    /* Section Styling */
    section {
      padding: 60px 20px;
      margin: 30px 0;
      background-color: #fff;
      border-radius: 8px;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
      text-align: center;
    }

    h1 {
      font-size: 30px;
      color: #333;
      margin-bottom: 20px;
    }

    p {
      font-size: 18px;
      color: #555;
      margin-bottom: 20px;
    }

    /* Books Section */
    .books ul {
      list-style-type: none;
      padding: 0;
    }

    .books ul li {
      background-color: #f9f9f9;
      margin: 10px 0;
      padding: 15px;
      border-radius: 5px;
      box-shadow: 0 3px 5px rgba(0, 0, 0, 0.1);
      font-size: 18px;
      display: flex;
      justify-content: space-between;
      transition: all 0.3s ease;
    }

    .books ul li:hover {
      background-color: #f1f1f1;
      transform: translateY(-5px);
    }

    /* Contact Form */
    form {
      display: flex;
      flex-direction: column;
      max-width: 500px;
      margin: 0 auto;
      background-color: #f9f9f9;
      padding: 20px;
      border-radius: 8px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    }

    form input, form textarea {
      margin-bottom: 15px;
      padding: 15px;
      font-size: 16px;
      border: 1px solid #ddd;
      border-radius: 4px;
    }

    form button {
      padding: 15px;
      background-color: #4b6cb7;
      color: white;
      border: none;
      font-size: 18px;
      cursor: pointer;
      transition: background-color 0.3s ease;
      border-radius: 4px;
    }

    form button:hover {
      background-color: #182848;
    }

    footer {
      background-color: #333;
      color: white;
      text-align: center;
      padding: 20px;
    }

    /* Smooth Scrolling */
    html {
      scroll-behavior: smooth;
    }

    /* Media Queries for Mobile Responsiveness */
    @media (max-width: 768px) {
      .hero h1 {
        font-size: 36px;
      }

      .hero p {
        font-size: 18px;
      }

      nav ul {
        flex-direction: column;
      }

      nav ul li {
        margin: 10px 0;
      }

      .profile {
        font-size: 16px;
        top: 10px;
        right: 10px;
      }
    }
  </style>
</head>
<body>
  <header>
    <!-- Profile section in the top right corner -->
    <div class="profile">
      <img src="https://via.placeholder.com/40" alt="Profile Picture">
      <span>Your Name</span> <!-- Replace 'Your Name' with your actual name -->
    </div>

    <nav>
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#contact">Contact</a></li>
        <li><a href="#books">Books</a></li>
        <li><a href="#login">Login</a></li>
      </ul>
    </nav>
  </header>

  <!-- Home Section -->
  <section id="home" class="hero">
    <h1>Welcome to Robe Secondary School</h1>
    <p>Your gateway to quality education and student management. Discover, learn, and grow with us!</p>
  </section>

  <!-- About Section -->
  <section id="about">
    <h1>About Robe Secondary School</h1>
    <p>Robe Secondary School is committed to fostering a learning environment that nurtures academic excellence and personal growth. We offer a variety of academic and extracurricular activities for students.</p>
  </section>

  <!-- Contact Section -->
  <section id="contact">
    <h1>Contact Us</h1>
    <form id="contact-form">
      <input type="text" id="name" name="name" placeholder="Your Name" required>
      <input type="email" id="email" name="email" placeholder="Your Email" required>
      <textarea id="message" name="message" placeholder="Your Message" required></textarea>
      <button type="submit">Submit</button>
    </form>
  </section>

  <!-- Books Section -->
  <section id="books" class="books">
    <h1>Recommended Books</h1>

    <h2>Grade 9</h2>
    <ul>
      <li><span>Math: "Algebra I" by John Doe</span><span>Price: $50</span></li>
      <li><span>Science: "Biology Basics" by Jane Smith</span><span>Price: $40</span></li>
      <li><span>History: "World History - A New Era" by David Brown</span><span>Price: $45</span></li>
      <li><span>English: "Literary Classics" by Robert White</span><span>Price: $30</span></li>
    </ul>

    <h2>Grade 10</h2>
    <ul>
      <li><span>Math: "Geometry Essentials" by Alice Johnson</span><span>Price: $55</span></li>
      <li><span>Science: "Physics Fundamentals" by Emily Green</span><span>Price: $50</span></li>
      <li><span>History: "Modern History" by Steve Lee</span><span>Price: $40</span></li>
      <li><span>English: "Advanced Literature" by Sarah Johnson</span><span>Price: $35</span></li>
    </ul>
  </section>

  <!-- Login Section -->
  <section id="login">
    <h1>Login to the Student Portal</h1>
    <form id="login-form">
      <input type="text" id="username" name="username" placeholder="Username" required>
      <input type="password" id="password" name="password" placeholder="Password" required>
      <button type="submit">Login</button>
    </form>
  </section>

  <footer>
    <p>&copy; 2024 Robe Secondary School | All rights reserved</p>
  </footer>

  <script>
    // Simple form validation for login
    document.getElementById('login-form').addEventListener('submit', function(e) {
      e.preventDefault();
      const username = document.getElementById('username').value;
      const password = document.getElementById('password').value;

      if (username === 'student' && password === 'password123') {
        alert('Login successful!');
        // Redirect to homepage after successful login
        window.location.href = '#home';
      } else {
        alert('Invalid username or password');
      }
    });

    // Simple contact form submission alert
    document.getElementById('contact-form').addEventListener('submit', function(e) {
      e.preventDefault();
      alert('Your message has been submitted.');
    });
  </script>
</body>
</html>
