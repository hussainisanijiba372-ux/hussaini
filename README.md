<! SPECIAL DATA OFFER >
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Special Data Offer</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            color: #333;
            text-align: center;
            margin: 0;
            padding: 0;
        }
        .container {
            background-color: white;
            padding: 20px;
            border-radius: 8px;
            width: 80%;
            margin: 50px auto;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        h1 {
            color: #007BFF;
        }
        .offer {
            margin: 20px 0;
            font-size: 18px;
        }
        .cta-button {
            background-color: #28a745;
            color: white;
            padding: 10px 20px;
            border: none;
            cursor: pointer;
            font-size: 16px;
            border-radius: 5px;
            transition: background-color 0.3s ease;
        }
        .cta-button:hover {
            background-color: #218838;
        }
        .random-numbers {
            margin-top: 20px;
            font-size: 16px;
            color: #555;
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
            <button class="cta-button" id="selectOffer">Select Plan</button>
        </div>

        <div class="random-numbers" id="randomNumbers">
            <!-- Random numbers will be shown here -->
        </div>
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
                randomNumbersDiv.appendChild(messageElement);
            }
        }

        document.getElementById("selectOffer").onclick = function() {
            var selectedOffer = document.querySelector('input[name="dataOffer"]:checked');
            if (selectedOffer) {
                var offer = selectedOffer.value;
                // Redirect to your Smart Link with the selected offer
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
