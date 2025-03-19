<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Japan Clock Widget</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            font-size: 24px;
            margin-top: 20%;
        }
    </style>
</head>
<body>
    <h2 id="clock"></h2>
    <script>
        function updateClock() {
            const options = { timeZone: 'Asia/Tokyo', hour12: false };
            const now = new Date().toLocaleTimeString('ja-JP', options);
            document.getElementById('clock').innerText = now;
        }
        setInterval(updateClock, 1000);
        updateClock();
    </script>
</body>
</html>
