<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Coder Username Generator</title>
    <script src="https://telegram.org/js/telegram-web-app.js"></script>
    <style>
        :root {
            --tg-theme-bg-color: #ffffff;
            --tg-theme-text-color: #000000;
            --tg-theme-hint-color: #999999;
            --tg-theme-link-color: #2481cc;
            --tg-theme-button-color: #3390ec;
            --tg-theme-button-text-color: #ffffff;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
            background-color: var(--tg-theme-bg-color);
            color: var(--tg-theme-text-color);
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            min-height: 100vh;
            margin: 0;
            padding: 20px;
            box-sizing: border-box;
        }

        .container {
            width: 100%;
            max-width: 400px;
        }

        h1 {
            color: var(--tg-theme-button-color);
            text-align: center;
            margin-bottom: 20px;
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
            background-color: var(--tg-theme-bg-color);
            color: var(--tg-theme-text-color);
            border: 1px solid var(--tg-theme-hint-color);
        }

        button {
            background-color: var(--tg-theme-button-color);
            color: var(--tg-theme-button-text-color);
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

        .contribute {
            margin-top: 20px;
            text-align: center;
        }

        .contribute a {
            color: var(--tg-theme-link-color);
            text-decoration: none;
        }

        .history {
            margin-top: 20px;
            text-align: left;
        }

        .history h3 {
            color: var(--tg-theme-button-color);
        }

        .history ul {
            list-style-type: none;
            padding: 0;
        }

        .history li {
            margin-bottom: 5px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Coder Username Generator</h1>
        <input type="text" id="inputWord" placeholder="Enter a word (optional)">
        <button onclick="generateUsername()">Generate Username</button>
        <button onclick="generateRandomUsername()">Random Username</button>
        <div id="result"></div>
        <div class="history">
            <h3>Recent Usernames</h3>
            <ul id="historyList"></ul>
        </div>
        <div class="contribute">
            <a href="https://github.com/likhonsheikhorg/coder-username/" target="_blank">Contribute on GitHub</a>
        </div>
    </div>

    <script>
        let tg = window.Telegram.WebApp;
        let history = [];

        tg.expand();
        tg.MainButton.setText('CLOSE').show().onClick(() => tg.close());

        const words = [
            "Phoenix", "Nebula", "Quantum", "Eclipse", "Cipher", "Vortex", "Nexus",
            "Enigma", "Paradox", "Syntax", "Zenith", "Matrix", "Phantom", "Reactor", "Aether"
        ];

        function toLeetSpeak(word) {
            const leet = {
                'a': '4', 'e': '3', 'i': '1', 'o': '0', 's': '5',
                't': '7', 'b': '8', 'g': '9', 'z': '2'
            };
            return word.toLowerCase().split('').map(char => leet[char] || char).join('');
        }

        function getRandomWord() {
            return words[Math.floor(Math.random() * words.length)];
        }

        function generateUsername() {
            const input = document.getElementById('inputWord').value;
            const word = input.trim() || getRandomWord();
            const username = toLeetSpeak(word);
            displayResult(username);
        }

        function generateRandomUsername() {
            const username = toLeetSpeak(getRandomWord());
            displayResult(username);
        }

        function displayResult(username) {
            document.getElementById('result').innerHTML = `
                Generated: <span id="username">${username}</span>
                <button onclick="copyToClipboard()">Copy</button>
            `;
            addToHistory(username);
        }

        function copyToClipboard() {
            const username = document.getElementById('username').textContent;
            navigator.clipboard.writeText(username).then(() => {
                tg.showAlert('Username copied to clipboard!');
            });
        }

        function addToHistory(username) {
            history.unshift(username);
            if (history.length > 5) history.pop();
            updateHistoryDisplay();
        }

        function updateHistoryDisplay() {
            const historyList = document.getElementById('historyList');
            historyList.innerHTML = history.map(name => `<li>${name}</li>`).join('');
        }

        // Inform the Telegram app that the Web App is ready to be displayed
        tg.ready();
    </script>
</body>
</html>
