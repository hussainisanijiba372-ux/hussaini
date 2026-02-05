<! SPECIAL DATA OFFER>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Special Data Offer</title>
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
        }

        label {
            font-size: 20px;
            color: #333;
        }

        /* Styling the radio buttons */
        input[type="radio"] {
            margin-right: 10px;
            accent-color: #FF7E5F; /* Custom accent color for the radio button */
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
            height: 200px; /* Set height for smooth scroll effect */
            overflow: hidden;
        }

        /* Animation for moving numbers from bottom to top */
        @keyframes moveNumbers {
            0% { transform: translateY(100%); } /* Start from bottom */
            100% { transform: translateY(-100%); } /* End at top */
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
        <h1>Special Data Offer</h1>
        <p>Choose the best data plan for you:</p>

        <div class="offer">
            <input type="radio" id="1GB" name="dataOffer" value="1GB - 50 Naira">
            <label for="1GB">1GB - 50 Naira</label>
        </div>
        
        <div class="offer">
            <input type="radio" id="2GB" name="dataOffer" value="2GB - 100 Naira">
            <label for="2GB">2GB - 100 Naira</label>
        </div>

        <div class="offer">
            <input type="radio" id="4GB" name="dataOffer" value="4GB - 150 Naira">
            <label for="4GB">4GB - 150 Naira</label>
        </div>

        <div class="offer">
            <button class="cta-button" id="selectOffer">Select Plan</button>
        </div>

        <div class="random-numbers" id="randomNumbers">
            <!-- Random numbers will be shown here -->
        </div>

        <footer>
            <p>&copy; 2026 Special Data Offer</p>
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
            for (let i = 0; i < 5; i++) { // Display 5 random numbers
                const randomNumber = generateRandomNumber();
                const randomMessage = `${randomNumber} have been received.`;
                const messageElement = document.createElement('p');
                messageElement.textContent = randomMessage;
                messageElement.style.animation = 'moveNumbers 10s infinite'; // Apply the scroll animation
                randomNumbersDiv.appendChild(messageElement);
            }
        }

        document.getElementById("selectOffer").onclick = function() {
            var selectedOffer = document.querySelector('input[name="dataOffer"]:checked');
            if (selectedOffer) {
                var offer = selectedOffer.value;
                // Redirecting to your Smart Link with the selected offer
                window.location.href = "https://qkzpkdm.com/cl/f79e71cfd864a5f8?offer=" + encodeURIComponent(offer);
            } else {
                alert("Please select a data plan.");
            }
        };

        // Call to show random numbers
        showRandomNumbers();
    </script>

</body>
</html>
