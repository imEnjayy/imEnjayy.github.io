<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Crypto Multiplier</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #1c1f26;
            font-family: Arial, sans-serif;
        }

        .crypto-card {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            width: 150px;
            height: 150px;
            background-color: #2a2d37;
            border: 3px solid #00ff66;
            border-radius: 10px;
            box-shadow: 0 0 10px #00ff66;
            color: white;
        }

        .crypto-card input {
            background: none;
            border: none;
            outline: none;
            color: white;
            text-align: center;
            font-size: 1.5rem;
            width: 80%;
        }

        .crypto-card input.amount {
            font-size: 1.2rem;
        }

        .crypto-card input:focus {
            border-bottom: 1px solid #00ff66;
        }

        .crypto-symbol {
            display: flex;
            align-items: center;
            font-size: 1rem;
            margin-top: 5px;
        }

        .crypto-symbol img {
            width: 16px;
            height: 16px;
            margin-left: 5px;
        }
    </style>
</head>
<body>
    <div class="crypto-card">
        <input id="multiplier" type="text" value="1.03×" />
        <div class="crypto-symbol">
            <input id="amount" class="amount" type="text" value="$0.00" />
            <img src="https://cryptologos.cc/logos/litecoin-ltc-logo.png" alt="Litecoin Symbol">
        </div>
    </div>

    <script>
        // JavaScript if needed for future interactivity
        const multiplierInput = document.getElementById("multiplier");
        const amountInput = document.getElementById("amount");

        multiplierInput.addEventListener("input", () => {
            console.log("Multiplier updated to:", multiplierInput.value);
        });

        amountInput.addEventListener("input", () => {
            console.log("Amount updated to:", amountInput.value);
        });
    </script>
</body>
</html>
