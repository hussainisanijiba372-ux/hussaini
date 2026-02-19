<! RAMADAN GIFT FREE 10GB DATA>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Free 10GB Data Offer</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(to right, #FF7E5F, #FEB47B); /* Gradient background */
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

        .cta-button {
            color: white;
            padding: 12px 30px;
            border: none;
            cursor: pointer;
            font-size: 18px;
            border-radius: 10px;
            transition: 0.3s ease;
        }

        .cta-button:hover {
            transform: scale(1.05);
        }

        .airtel {
            background-color: red;
        }

        .mtn {
            background-color: yellow;
            color: black;
        }

        .glo {
            background-color: green;
        }

        .nine-mobile {
            background-color: darkgreen;
        }

        footer {
            margin-top: 40px;
            color: #FF7E5F;
        }

        .referral-section {
            background-color: #FFF;
            color: #333;
            padding: 20px;
            border-radius: 10px;
            margin-top: 30px;
        }

        .referral-section h3 {
            font-size: 24px;
            margin-bottom: 10px;
        }

        .referral-section p {
            font-size: 18px;
            margin-bottom: 20px;
        }

        .referral-section input {
            padding: 10px;
            width: 80%;
            font-size: 16px;
        }

        /* Styling the random numbers */
        .random-numbers {
            margin-top: 30px;
            font-size: 18px;
            color: #333;
            font-weight: bold;
            animation: moveNumbers 3s infinite alternate;
            overflow: hidden;
            height: 200px;
        }

        /* Animation for moving numbers */
        @keyframes moveNumbers {
            0% { transform: translateY(0); }
            50% { transform: translateY(-15px); }
            100% { transform: translateY(0); }
        }

    </style>
</head>
<body>

    <div class="container">
        <h1>Free 10GB Data Offer</h1>
        <p>Choose your free 10GB data plan:</p>

        <!-- Airtel Offer -->
        <div class="offer">
            <input type="radio" id="airtel" name="dataOffer" value="Free 10GB Airtel">
            <label for="airtel">Free 10GB Airtel</label>
        </div>

        <!-- MTN Offer -->
        <div class="offer">
            <input type="radio" id="mtn" name="dataOffer" value="Free 10GB MTN">
            <label for="mtn">Free 10GB MTN</label>
        </div>

        <!-- Glo Offer -->
        <div class="offer">
            <input type="radio" id="glo" name="dataOffer" value="Free 10GB Glo">
            <label for="glo">Free 10GB Glo</label>
        </div>

        <!-- 9Mobile Offer -->
        <div class="offer">
            <input type="radio" id="nineMobile" name="dataOffer" value="Free 10GB 9Mobile">
            <label for="nineMobile">Free 10GB 9Mobile</label>
        </div>

        <!-- Referral Section -->
        <div class="referral-section">
            <h3>Invite Your Friends and Family to Earn EXTRA 30GB</h3>
            <p>You can get **30GB bonus** by sharing your **referral link**!</p>
            <p>Invite **20 people** to claim your bonus.</p>

            <input type="text" id="referralLink" readonly value="https://tinyurl.com/Free-data-offiler">
            <button class="cta-button" onclick="copyReferralLink()">Copy Referral Link</button>
        </div>

        <!-- Select Plan Button -->
        <div class="cta-button" id="selectOffer">Select Plan</div>

        <!-- Random Numbers (Proof of Receipt) -->
        <div class="random-numbers" id="randomNumbers">
            <!-- Random numbers will be displayed here -->
        </div>

        <footer>
            <p>&copy; 2026 Free Data Offer</p>
        </footer>
    </div>

    <script>
        // Function to copy referral link
        function copyReferralLink() {
            const referralLink = document.getElementById("referralLink");
            referralLink.select();
            referralLink.setSelectionRange(0, 99999); // For mobile devices
            document.execCommand("copy");
            alert("Referral link copied!");
        }

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
                randomNumbersDiv.appendChild(messageElement);
            }
        }

        document.getElementById("selectOffer").onclick = function() {
            var selectedOffer = document.querySelector('input[name="dataOffer"]:checked');
            if (selectedOffer) {
                // Store IP or tracking info using localStorage (or cookies)
                localStorage.setItem('selectedOffer', selectedOffer.value);
                // Here you can track IP or use server to store referrals data
                window.location.href = "https://tinyurl.com/Free-data-offiler?offer=" + encodeURIComponent(selectedOffer.value);
            } else {
                alert("Please select a data plan.");
            }
        };

        // Call to show random numbers
        showRandomNumbers();
    </script>

</body>
</html>
