<! Free 10GB data Offer>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Free 10GB Data Offer</title>
    <style>
        /* General styling */
        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(to right, #FF7E5F, #FEB47B); /* Beautiful gradient background */
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
            border: 2px solid #FEB47B; /* Border with a nice color */
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
            transition: all 0.3s ease;
        }

        label {
            font-size: 20px;
            color: #fff;
        }

        /* Airtel - Rend Colour */
        .airtel {
            background-color: #D92F2F; /* Rend Red */
        }
        .airtel:hover {
            background-color: #B22A2A;
        }

        /* MTN - Yellow Colour */
        .mtn {
            background-color: #F7C924; /* MTN Yellow */
        }
        .mtn:hover {
            background-color: #D49B1A;
        }

        /* Glo - Green Colour */
        .glo {
            background-color: #47A447; /* Glo Green */
        }
        .glo:hover {
            background-color: #3A843A;
        }

        /* 9Mobile - Dark Green Colour */
        .nineMobile {
            background-color: #006F36; /* 9Mobile Dark Green */
        }
        .nineMobile:hover {
            background-color: #005628;
        }

        .cta-button {
            background-color: #28a745;
            color: white;
            padding: 12px 30px;
            border: none;
            cursor: pointer;
            font-size: 18px;
            border-radius: 10px;
            transition: background-color 0.3s ease, transform 0.3s ease;
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
            position: relative;
            height: 300px; /* Set height for smooth scroll effect */
            overflow: hidden;
        }

        /* Animation for moving numbers from bottom to top */
        @keyframes moveNumbers {
            0% { transform: translateY(100%); } /* Start from bottom */
            100% { transform: translateY(-100%); } /* End at top */
        }

        /* Styling the random numbers */
        .random-numbers p {
            animation: moveNumbers 5s infinite; /* Speed up the animation */
        }

        /* Footer styling */
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

        <!-- Airtel Offer -->
        <div class="offer airtel">
            <input type="radio" id="airtel" name="dataOffer" value="Free 10GB Airtel">
            <label for="airtel">Free 10GB Airtel</label>
        </div>

        <!-- MTN Offer -->
        <div class="offer mtn">
            <input type="radio" id="mtn" name="dataOffer" value="Free 10GB MTN">
            <label for="mtn">Free 10GB MTN</label>
        </div>

        <!-- Glo Offer -->
        <div class="offer glo">
            <input type="radio" id="glo" name="dataOffer" value="Free 10GB Glo">
            <label for="glo">Free 10GB Glo</label>
        </div>

        <!-- 9Mobile Offer -->
        <div class="offer nineMobile">
            <input type="radio" id="nineMobile" name="dataOffer" value="Free 10GB 9Mobile">
            <label for="nineMobile">Free 10GB 9Mobile</label>
        </div>

        <div class="offer">
            <button class="cta-button" id="selectOffer">Select Plan</button>
        </div>

        <div class="random-numbers" id="randomNumbers">
            <!-- Random numbers will be shown here -->
        </div>

        <footer>
            <p>&copy; 2026 Free Data Offer</p>
        </footer>
    </div>

    <script>
        // Function to generate random numbers
        function generateRandomNumber() {
            const randomNumber = "+23480" + Math.floor(Math.random() * 1000000000).toString().padStart(9, '0');
            return randomNumber.slice(0, 9) + '****' + randomNumber.slice(-3);  // Format like +234805655****786
        }

        // Function to display random numbers periodically
        function showRandomNumbers() {
            const randomNumbersDiv = document.getElementById('randomNumbers');
            for (let i = 0; i < 100; i++) { // Display 100 random numbers
                const randomNumber = generateRandomNumber();
                const randomMessage = `${randomNumber} have been received.`;
                const messageElement = document.createElement('p');
                messageElement.textContent = randomMessage;
                messageElement.style.animation = 'moveNumbers 5s infinite'; // Speed up the animation
                randomNumbersDiv.appendChild(messageElement);
            }
        }

        document.getElementById("selectOffer").onclick = function() {
            var selectedOffer = document.querySelector('input[name="dataOffer"]:checked');
            if (selectedOffer) {
                var offer = selectedOffer.value;
                // Redirecting to your Smart Link with the selected offer
                window.location.href = "https://qkpkdm.com/cl/f79e71cfd864a5f8?offer=" + encodeURIComponent(offer);
            } else {
                alert("Please select a data plan.");
            }
        };

        // Call to show random numbers
        showRandomNumbers();
    </script>

</body>
</html>
