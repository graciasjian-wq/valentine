# valentine-card
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Valentine's Day Invitation</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #ffe6e6;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .card {
            width: 400px;
            height: 300px;
            background-color: #fff;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
            position: relative;
            overflow: hidden;
            cursor: pointer;
            transition: transform 0.5s;
        }
        .card.flipped {
            transform: rotateY(180deg);
        }
        .front, .back {
            position: absolute;
            width: 100%;
            height: 100%;
            backface-visibility: hidden;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            text-align: center;
        }
        .front {
            background: linear-gradient(45deg, #ff6b6b, #feca57);
            color: white;
        }
        .back {
            background-color: #fff;
            transform: rotateY(180deg);
            padding: 20px;
        }
        .message {
            font-size: 18px;
            margin-bottom: 20px;
        }
        .link {
            color: #ff6b6b;
            text-decoration: none;
            font-weight: bold;
        }
        .link:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <div class="card" id="card">
        <div class="front">
            <h1>Happy Valentine's Day!</h1>
            <p>Click to open your special invitation</p>
        </div>
        <div class="back">
            <p class="message" id="message">Dear [Girlfriend's Name],<br><br>This is my special Valentine's Day message to you. I love you more than words can say! Edit this message to make it personal.</p>
            <a href="https://example.com" class="link" id="link">Click here for a surprise!</a>
        </div>
    </div>

    <script>
        const card = document.getElementById('card');
        card.addEventListener('click', () => {
            card.classList.toggle('flipped');
        });
    </script>
</body>
</html>
