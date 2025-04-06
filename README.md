# Only-for-you
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>For You</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #fce4ec;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
    }
    .box {
      background: #fff0f5;
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.2);
      text-align: center;
    }
    button {
      margin: 10px;
      padding: 10px 20px;
      border: none;
      background: #ec407a;
      color: white;
      font-size: 16px;
      border-radius: 10px;
      cursor: pointer;
    }
    input {
      margin-top: 15px;
      padding: 8px;
      width: 80%;
      border-radius: 8px;
      border: 1px solid #ccc;
    }
  </style>
</head>
<body>
  <div class="box" id="questionBox">
    <h2>Hey love, are you okay?</h2>
    <button onclick="answerYes()">Yes</button>
    <button onclick="answerNo()">No</button>
  </div>

  <script>
    function answerYes() {
      const box = document.getElementById('questionBox');
      box.innerHTML = `
        <h2>What can I do for you?</h2>
        <input type="text" placeholder="Tell me anything..." />
      `;
    }

    function answerNo() {
      const box = document.getElementById('questionBox');
      box.innerHTML = `
        <h2>I'm always here for you.</h2>
        <p>Take your time. I’m just a message away.</p>
      `;
    }
  </script>
</body>
</html>
