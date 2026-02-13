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
            <p class="message" id="message">Dear Baby Ira,<br><br>. Hi babyy, HAPPY VALENTINES DAY!!

Wala jud ko kabalo kung unsa or asa ko mag start,
But i'm glad na nakilala kita, Because i found you the most precious gift na receive ko ever!!

I'm queitly sure enough na hindi ko talaga to ginagawa, I'm not really good at words. But I'll try~~

I know loving you isn’t always loud or overly expressive. Sometimes it’s quiet. Sometimes it’s gentle. Sometimes it takes a little space to breathe. And that’s okay. I’ve learned that love doesn’t always have to be big and obvious to be real. What matters to me is that we’re still here, still choosing each other and that means everything.

I know your heart protects itself. I know closeness can feel overwhelming sometimes, and opening up isn’t always easy. I just want you to know I’m not here to rush you, pressure you, or change who you are. I’m here to understand you. To be patient with you. To stay steady beside you, even on the days when things feel complicated.

Every small step you take toward me, I notice it. Every time you let me in, even just a little, I feel it deeply. The quiet efforts, the subtle affection, the moments when you lower your guard they mean more to me than you probably realize. Nothing about your love goes unseen.

We’ve grown through misunderstandings, through silence, through moments that could’ve easily pulled us apart but we stayed. We chose to work through things. We chose to understand each other instead of giving up. And that’s something beautiful. That’s something real.

I love you because you’re you. Soft in your own way. Strong in your own way. Trying in your own way. And I’m genuinely proud of how far we’ve come together.

Loving you has taught me patience, gentleness, and deeper understanding. It’s taught me that real love is steady. It stays. It grows quietly. And I have a lot to learn and know about you. 

No matter how you show love, I see it. I feel it. And I treasure it. I’ll keep choosing you not just today, but every day. Through the quiet, through the growth, through everything, I'll stay beside your side. I'm always here to support you even though and kulet² mo minsan😏, But i understand it.

I really wish i can go out with you, I have more to offer but sadly it requires ticket and passport HAHAHAHAH, I'm sorry love tumatawa lang ako here but naiiyak talaga ako huhu.

But i know soon , We can and we will hehe😚.

I have nothing to offer ako nalang kaya? gawin mokong dessert moHAHAHAHA eme, but here some flowers and chocolates for you: 🌹🍫.

Gusto ko po talaga mag padala nyan pero diko alam kung saan, And if baka mag padala em dry na yung flowers and melt na yung chocolate huhu🥹🥹 Sorry po!!

I love you so much than you know ira, HAPPY VALENTINES DAY again LOVEY!!.</p>
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
