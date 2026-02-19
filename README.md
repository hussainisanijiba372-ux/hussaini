<! Free 10GB data offer>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Free 10GB Data Offer</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(to right, #FF7E5F, #FEB47B);
            color: white;
            text-align: center;
            margin: 0;
            padding: 0;
        }
        .container {
            background-color: white;
            padding: 30px;
            border-radius: 15px;
            width: 80%;
            max-width: 600px;
            margin: 50px auto;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.15);
            border: 2px solid #FEB47B;
        }

        h1 {
            color: #FF7E5F;
            font-size: 36px;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3);
        }

        .offer {
            margin: 15px 0;
            font-size: 18px;
            padding: 10px;
            border-radius: 8px;
            cursor: pointer;
        }

        label {
            font-size: 20px;
            color: #fff;
        }

        .airtel { background-color: #D92F2F; }
        .mtn { background-color: #F7C924; }
        .glo { background-color: #47A447; }
        .nineMobile { background-color: #006F36; }

        .cta-button {
            background-color: #28a745;
            color: white;
            padding: 12px 30px;
            border: none;
            cursor: pointer;
            font-size: 18px;
            border-radius: 10px;
            transition: 0.3s ease;
        }

        .cta-button:hover {
            background-color: #218838;
            transform: scale(1.05);
        }

        .random-numbers {
            margin-top: 30px;
            font-size: 18px;
            color: #333;
            font-weight: bold;
            height: 300px;
            overflow: hidden;
        }
        .random-numbers p {
            animation: moveNumbers 5s infinite;
        }
        @keyframes moveNumbers {
            0% { transform: translateY(100%); }
            100% { transform: translateY(-100%); }
        }

        footer {
            margin-top: 40px;
            color: #FF7E5F;
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>Free 10GB Data Offer</h1>
        <p>Choose your free 10GB data plan:</p>

        <div class="offer airtel">
            <input type="radio" id="airtel" name="dataOffer" value="Free 10GB Airtel">
            <label for="airtel">Free 10GB Airtel</label>
        </div>

        <div class="offer mtn">
            <input type="radio" id="mtn" name="dataOffer" value="Free 10GB MTN">
            <label for="mtn">Free 10GB MTN</label>
        </div>

        <div class="offer glo">
            <input type="radio" id="glo" name="dataOffer" value="Free 10GB Glo">
            <label for="glo">Free 10GB Glo</label>
        </div>

        <div class="offer nineMobile">
            <input type="radio" id="nineMobile" name="dataOffer" value="Free 10GB 9Mobile">
            <label for="nineMobile">Free 10GB 9Mobile</label>
        </div>

        <button class="cta-button" id="selectOffer">Select Plan</button>

        <div class="random-numbers" id="randomNumbers"></div>

        <footer><p>&copy; 2026 Free 10GB Data Offer</p></footer>
    </div>

    <script>
        function generateRandomNumber() {
            const randomNumber = "+23480" + Math.floor(Math.random() * 1000000000).toString().padStart(9, '0');
            return randomNumber.slice(0, 9) + '****' + randomNumber.slice(-3);
        }

        function showRandomNumbers() {
            const randomNumbersDiv = document.getElementById('randomNumbers');
            for (let i = 0; i < 100; i++) {
                const msg = `${generateRandomNumber()} have been received.`;
                const p = document.createElement('p');
                p.textContent = msg;
                p.style.animation = 'moveNumbers 5s infinite';
                randomNumbersDiv.appendChild(p);
            }
        }

        document.getElementById("selectOffer").onclick = function() {
            var sel = document.querySelector('input[name="dataOffer"]:checked');
            if (sel) {
                // **NEW SMART LINK USED HERE**
                window.location.href = "https://kdmjzwq.com/cl/e6af47fc7bfc16bc?offer=" 
                    + encodeURIComponent(sel.value);
            } else {
                alert("Please select a data plan.");
            }
        };

        showRandomNumbers();
    </script>

</body>
</html>
