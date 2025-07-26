<!DOCTYPE html>
<html lang="el">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Kanavos Play</title>
<style>
  body {
    background: linear-gradient(to bottom right, #ff9a9e, #fad0c4);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100vh;
    margin: 0;
    font-family: 'Arial', sans-serif;
    color: #fff;
  }
  #playButton {
    padding: 20px 50px;
    font-size: 48px;
    background-color: #fff;
    border: none;
    border-radius: 20px;
    color: #ff4d6d;
    box-shadow: 0 5px 15px rgba(0,0,0,0.3);
    cursor: pointer;
    transition: background-color 0.3s ease;
  }
  #playButton:hover {
    background-color: #ffe6e9;
  }
  #siteName {
    margin-top: 15px;
    font-size: 18px;
    color: #fff;
    opacity: 0.7;
  }
  #message {
    margin-top: 40px;
    font-size: 36px;
    display: none;
    animation: fadeIn 1s ease forwards;
  }
  @keyframes fadeIn {
    from {opacity: 0; transform: translateY(20px);}
    to {opacity: 1; transform: translateY(0);}
  }
</style>
</head>
<body>

  <button id="playButton">Play</button>
  <div id="siteName">kanavos.github.io</div>
  <div id="message">Τι κάνεις ρε μεγάλε ❤️</div>

  <script>
    document.getElementById('playButton').addEventListener('click', function() {
      this.style.display = 'none';
      document.getElementById('message').style.display = 'block';
    });
  </script>

</body>
</html>
