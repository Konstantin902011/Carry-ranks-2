<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Open in Browser</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 50px;
            background-color: #f0f0f0;
        }
        h1 {
            font-size: 24px;
            margin-bottom: 20px;
        }
        p {
            font-size: 16px;
            margin-bottom: 30px;
        }
        a.button {
            display: inline-block;
            padding: 15px 25px;
            font-size: 18px;
            background-color: #007bff;
            color: white;
            text-decoration: none;
            border-radius: 5px;
        }
        a.button:hover {
            background-color: #0056b3;
        }
    </style>
    <script>
        window.onload = function() {
            // Проверяем, открыт ли сайт в Instagram (через его встроенный браузер)
            var ua = navigator.userAgent || navigator.vendor || window.opera;
            if (/instagram/i.test(ua)) {
                // Если в Instagram, просим пользователя открыть в стандартном браузере
                document.getElementById("manualRedirect").style.display = 'block';
            } else {
                // Если не в Instagram, перенаправляем сразу на основной сайт
                window.location.href = "https://konstantin902011.github.io/Carry-ranks-/";
            }
        }
    </script>
</head>
<body>

    <h1>Open in Your Browser</h1>
    <p>If you are viewing this page inside Instagram, please open the link below in your regular browser.</p>
    
    <!-- Эта кнопка появляется только если сайт открыт в Instagram -->
    <div id="manualRedirect" style="display:none;">
        <a class="button" href="https://konstantin902011.github.io/Carry-ranks-/" target="_blank">Open in Browser</a>
    </div>

</body>
</html>