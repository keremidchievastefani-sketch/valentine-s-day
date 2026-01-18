# valentine-s-day
<!DOCTYPE html>
<html lang="bg">
<head>
    <meta charset="UTF-8">
    <title>💖 Валентинка 💖</title>
    <style>
        body {
            background: linear-gradient(135deg, #ff9a9e, #fad0c4);
            font-family: Arial, sans-serif;
            text-align: center;
            height: 100vh;
            margin: 0;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .box {
            background: white;
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.2);
            width: 320px;
        }

        h1 {
            color: #e91e63;
        }

        button {
            padding: 10px 20px;
            font-size: 18px;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            margin: 10px;
        }

        #yes {
            background: #e91e63;
            color: white;
        }

        #no {
            background: #ccc;
            position: absolute;
        }

        #text {
            display: none;
            font-size: 16px;
            margin-top: 20px;
            color: #444;
        }
    </style>
</head>
<body>

<div class="box">
    <h1>💘 Ще ми бъдеш ли Валентинка? 💘</h1>

    <button id="yes" onclick="showText()">ДА 💖</button>
    <button id="no" onmouseover="moveNo()">НЕ 🙃</button>

    <div id="text">
        ❤️  
        От момента, в който се появи в живота ми, всичко стана по-светло.  
        Усмивките ми са повече, дните ми са по-топли  
        и сърцето ми бие малко по-силно, когато си наблизо.  

        Не обещавам съвършенство,  
        но обещавам искреност, смях  
        и много моменти, които си струват.  

        Благодаря ти, че си ти.  
        💖
    </div>
</div>

<script>
    function moveNo() {
        const no = document.getElementById("no");
        const x = Math.random() * (window.innerWidth - 100);
        const y = Math.random() * (window.innerHeight - 100);
        no.style.left = x + "px";
        no.style.top = y + "px";
    }

    function showText() {
        document.getElementById("text").style.display = "block";
    }
</script>

</body>
</html>
