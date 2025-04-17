# Money-s-<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Subscribe & Earn</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f0f4f8;
      margin: 0;
      padding: 0;
    }

    .container {
      max-width: 500px;
      margin: 40px auto;
      background-color: #fff;
      padding: 30px;
      border-radius: 12px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }

    h2 {
      text-align: center;
      color: #333;
    }

    label {
      display: block;
      margin-top: 15px;
      margin-bottom: 5px;
    }

    input, select {
      width: 100%;
      padding: 10px;
      border-radius: 6px;
      border: 1px solid #ccc;
      margin-bottom: 15px;
    }

    button {
      width: 100%;
      padding: 12px;
      background-color: #00b14f;
      color: white;
      font-weight: bold;
      border: none;
      border-radius: 6px;
      cursor: pointer;
    }

    button:hover {
      background-color: #008a3f;
    }

    .result {
      margin-top: 20px;
      font-weight: bold;
      text-align: center;
      color: #2e7d32;
    }
  </style>
</head>
<body>
  <div class="container">
    <h2>Subscribe Now</h2>
    <form>
      <label for="phone">Phone Number (M-Pesa):</label>
      <input type="tel" id="phone" name="phone" placeholder="07XXXXXXXX" required />

      <label for="amount">Select Package Amount:</label>
      <select id="amount" name="amount" required>
        <option value="">-- Choose an amount --</option>
        <option value="100">Ksh 100</option>
        <option value="250">Ksh 250</option>
        <option value="500">Ksh 500</option>
        <option value="1000">Ksh 1000</option>
      </select>

      <button type="submit">Pay with M-Pesa</button>
    </form>

    <hr style="margin: 30px 0;">

    <h2>Trivia Quiz - Earn Ksh 25 Per Correct Answer</h2>
    <form id="quizForm">
      <label>1. What is the capital of Kenya?</label>
      <input type="text" name="q1" required />

      <label>2. What is 5 + 3?</label>
      <input type="text" name="q2" required />

      <label>3. Which animal is known as the king of the jungle?</label>
      <input type="text" name="q3" required />

      <button type="button" onclick="checkAnswers()">Submit Answers</button>
    </form>

    <div class="result" id="result"></div>
  </div>

  <script>
    function checkAnswers() {
      const answers = {
        q1: "nairobi",
        q2: "8",
        q3: "lion"
      };

      let score = 0;
      const form = document.forms["quizForm"];
      
      if (form["q1"].value.trim().toLowerCase() === answers.q1) score++;
      if (form["q2"].value.trim() === answers.q2) score++;
      if (form["q3"].value.trim().toLowerCase() === answers.q3) score++;

      const total = score * 25;
      document.getElementById("result").innerText = `You got ${score} correct! You earned Ksh ${total}.`;
    }
  </script>
</body>
</html>
