<?php
// Function to convert a word to leet speak
function toLeetSpeak($word) {
    $leet = [
        'a' => '4', 'e' => '3', 'i' => '1', 'o' => '0', 's' => '5',
        't' => '7', 'b' => '8', 'g' => '9', 'z' => '2'
    ];
    return strtr(strtolower($word), $leet);
}

// Function to generate a random word from a predefined list
function getRandomWord() {
    $words = [
        "Phoenix", "Nebula", "Quantum", "Eclipse", "Cipher", "Vortex", "Nexus",
        "Enigma", "Paradox", "Syntax", "Zenith", "Matrix", "Phantom", "Reactor", "Aether"
    ];
    return $words[array_rand($words)];
}

// Generate username based on input or random word
function generateUsername($input = '') {
    $word = empty($input) ? getRandomWord() : $input;
    return toLeetSpeak($word);
}

// Handle form submission
$generatedUsername = '';
if ($_SERVER["REQUEST_METHOD"] == "POST") {
    $input = $_POST['input'] ?? '';
    $generatedUsername = generateUsername($input);
}
?>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Telegram Username Generator</title>
    <script src="https://telegram.org/js/telegram-web-app.js"></script>
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
            background-color: var(--tg-theme-bg-color, #ffffff);
            color: var(--tg-theme-text-color, #000000);
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .container {
            width: 90%;
            max-width: 400px;
        }
        h1 {
            color: var(--tg-theme-button-color, #3390ec);
            text-align: center;
        }
        input, button {
            width: 100%;
            padding: 12px;
            margin: 8px 0;
            box-sizing: border-box;
            border: none;
            border-radius: 8px;
            font-size: 16px;
        }
        input {
            background-color: var(--tg-theme-secondary-bg-color, #f0f0f0);
            color: var(--tg-theme-text-color, #000000);
        }
        button {
            background-color: var(--tg-theme-button-color, #3390ec);
            color: var(--tg-theme-button-text-color, #ffffff);
            cursor: pointer;
            transition: opacity 0.3s;
        }
        button:hover {
            opacity: 0.8;
        }
        #result {
            margin-top: 20px;
            text-align: center;
            font-size: 18px;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Username Generator</h1>
        <form method="post">
            <input type="text" name="input" placeholder="Enter a word (optional)">
            <button type="submit" name="generate">Generate Username</button>
            <button type="submit" name="random">Random Username</button>
        </form>
        <?php if (!empty($generatedUsername)): ?>
            <div id="result">
                Generated: <span id="username"><?php echo htmlspecialchars($generatedUsername); ?></span>
                <button onclick="copyToClipboard()">Copy</button>
            </div>
        <?php endif; ?>
    </div>

    <script>
        let tg = window.Telegram.WebApp;

        tg.expand();

        tg.MainButton.setText('CLOSE').show().onClick(function(){ tg.close(); });

        function copyToClipboard() {
            const username = document.getElementById('username').textContent;
            navigator.clipboard.writeText(username).then(() => {
                tg.showAlert('Username copied to clipboard!');
            });
        }

        // Inform the Telegram app that the Web App is ready to be displayed
        tg.ready();
    </script>
</body>
</html>
