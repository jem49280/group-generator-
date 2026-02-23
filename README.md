
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Group Generator</title>
    <style>
        body {
            font-family: sans-serif;
            padding: 20px;
            text-align: center;
            background-color: #f4f4f9;
        }
        button {
            padding: 15px 30px;
            font-size: 18px;
            background-color: #2ea44f;
            color: white;
            border: none;
            border-radius: 6px;
            cursor: pointer;
        }
        #result {
            margin-top: 20px;
            font-weight: bold;
            font-size: 1.2rem;
        }
    </style>
</head>
<body>

    <h1>Group Generator</h1>
    <p>Tap the button to start!</p>
    
    <button onclick="generate()">Generate Group</button>
    
    <div id="result"></div>

    <script>
        function generate() {
            const groups = ["Team Alpha", "Team Beta", "Team Gamma"];
            const random = groups[Math.floor(Math.random() * groups.length)];
            document.getElementById('result').innerText = "You are in: " + random;
        }
    </script>

</body>
</html>
