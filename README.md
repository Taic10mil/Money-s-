<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Welcome | Money-S</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', sans-serif;
      color: #fff;
      background: url('https://images.unsplash.com/photo-1605902711622-cfb43c4437d2') no-repeat center center fixed;
      background-size: cover;
    }

    .overlay {
      background-color: rgba(10, 10, 10, 0.85); /* darker overlay */
      height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 0 20px;
    }

    h1 {
      font-size: 36px;
      margin-bottom: 20px;
    }

    p {
      font-size: 18px;
      max-width: 500px;
      margin-bottom: 40px;
      color: #ccc;
    }

    .btn {
      padding: 15px 30px;
      background-color: #00b14f;
      border: none;
      border-radius: 8px;
      color: white;
      font-size: 18px;
      cursor: pointer;
      text-decoration: none;
      transition: background-color 0.3s ease;
    }

    .btn:hover {
      background-color: #008b3a;
    }
  </style>
</head>
<body>
  <div class="overlay">
    <h1>Welcome to Money-S</h1>
    <p>Subscribe to a package and start earning cash by completing fun tasks like trivia, spinning the wheel, watching videos, and more.</p>
    <a href="login.html" class="btn">Get Started</a>
  </div>
</body>
</html>
