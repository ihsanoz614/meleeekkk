<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <title>Melek İçin Güzel Sözler</title>
    <link href="https://fonts.googleapis.com/css2?family=Indie+Flower&family=Open+Sans&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            padding: 0;
            background: linear-gradient(to top right, #ffd1dc, #ffe6f0);
            font-family: 'Open Sans', sans-serif;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            text-align: center;
        }

        h1 {
            font-family: 'Indie Flower', cursive;
            font-size: 3rem;
            color: #d63384;
        }

        #sozel {
            margin: 30px auto;
            font-size: 1.5rem;
            color: #6a0572;
            font-style: italic;
            opacity: 0;
            transition: opacity 0.8s ease-in-out;
            max-width: 500px;
        }

        button {
            padding: 12px 25px;
            font-size: 1rem;
            border: none;
            background-color: #ff66a3;
            color: white;
            border-radius: 20px;
            cursor: pointer;
            box-shadow: 0 4px 10px rgba(0,0,0,0.2);
            transition: background 0.3s;
        }

        button:hover {
            background-color: #e84393;
        }

        footer {
            position: absolute;
            bottom: 10px;
            font-size: 0.9rem;
            color: #555;
        }
    </style>
</head>
<body>

    <h1>💖 Melek İçin Güzel Sözler 💖</h1>

    <button onclick="yeniSoz()">Bir Söz Göster</button>

    <div id="sozel"></div>

    <footer>Senin için hazırlayan: <strong>İhsan</strong> 💌</footer>

    <script>
        const sozler = [
            "Senin gülüşün bu dünyanın en güzel melodisi.",
            "Gözlerin, geceme doğan en parlak yıldız gibi.",
            "Senin varlığın bile yetiyor, huzur buluyorum.",
            "Melek ismin kadar kalbin de meleksi.",
            "Kalbim sana ait, anahtarı sadece sende.",
            "Gülüşünle içimi ısıtıyorsun.",
            "Seninle her an, bir masal gibi.",
            "Bir bakışın bile kalbimi durdurmaya yetiyor.",
            "Seninle geçirdiğim her an sonsuza değer.",
            "İyi ki varsın Melek, iyi ki hayatımdasın."
        ];

        function yeniSoz() {
            const sozel = document.getElementById("sozel");
            const rastgele = sozler[Math.floor(Math.random() * sozler.length)];
            sozel.style.opacity = 0;
            setTimeout(() => {
                sozel.textContent = `"${rastgele}"`;
                sozel.style.opacity = 1;
            }, 300);
        }
    </script>

</body>
</html>
