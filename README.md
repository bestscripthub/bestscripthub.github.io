<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Random Challenge Generator</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: gray;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        #sentence {
            margin: 20px;
            padding: 20px;
            background: white;
            border-radius: 5px;
            text-align: center;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <h1>Random Challenge Generator</h1>
    <div id="sentence">Press the button to generate a challenge</div>
    <button onclick="generateSentence()">Roll</button>

    <script>
        function generateSentence() {
            const sentences = [
                "Go to a restroom in a school.",
                "Do not wash your hands for 5 days.",
                "Don't wash your hands for 1 day.",
                "Sleep naked for 2 weeks.",
                "Don't drink anything for a whole day.",
                "Eat in a restroom the next chance you get.",
                "Don't wash your hands for 2 days.",
                "Don't wash your hands for 4 days.",
				" do 100 push ups naked."
				
            ];
            const randomIndex = Math.floor(Math.random() * sentences.length);
            document.getElementById('sentence').innerText = sentences[randomIndex];
        }
    </script>
</body>
</html>
