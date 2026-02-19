<! FREE RAMADAN 1GB DATA GIFTl>
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

            <input type="text" id="referralLink" readonly value="https://kdmjzwq.com/cl/e6af47fc7bfc16bc?referralID=YOUR_UNIQUE_ID">
            <button class="cta-button" onclick="copyReferralLink()">Copy Referral Link</button>
        </div>

        <!-- Select Plan Button -->
        <div class="cta-button" id="selectOffer">Select Plan</div>

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

        // Referral Link Redirection
        document.getElementById("selectOffer").onclick = function() {
            var selectedOffer = document.querySelector('input[name="dataOffer"]:checked');
            if (selectedOffer) {
                // Store IP or tracking info using localStorage (or cookies)
                localStorage.setItem('selectedOffer', selectedOffer.value);
                // Here you can track IP or use server to store referrals data
                window.location.href = "https://kdmjzwq.com/cl/e6af47fc7bfc16bc?offer=" + encodeURIComponent(selectedOffer.value);
            } else {
                alert("Please select a data plan.");
            }
        };
    </script>

</body>
</html>        .
