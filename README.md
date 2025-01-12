<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Styled Box</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #0F1E28; /* Page background */
            font-family: Arial, sans-serif;
        }

        .box {
            width: 200px;
            height: 180px;
            background-color: #1A2C38;
            border: 3px solid #00FF00; /* Green border always visible */
            border-radius: 10px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.5); /* Optional for better look */
        }

        .box:hover {
            transform: scale(1.05); /* Slight zoom effect on hover */
            transition: transform 0.2s;
        }

        .multiplier {
            font-size: 28px; /* Adjusted to match reference */
            font-weight: bold;
            color: #00FF00; /* Green text */
            margin-bottom: 10px;
        }

        .divider {
            width: 70%; /* Adjusted to fit the box */
            height: 1px;
            background-color: #2F4553; /* Dark gray-blue */
            margin: 10px 0;
        }

        .value {
            display: flex;
            align-items: center;
            font-weight: normal; /* Balanced boldness */
            font-size: 20px; /* Increased to align with multiplier */
            line-height: 120%;
            color: #00FF00; /* Green text */
        }

        .value span {
            font-size: 20px;
            line-height: 120%;
        }

        .value img {
            width: 18px; /* Scaled Litecoin logo */
            height: 18px;
            margin-left: 5px;
        }
    </style>
</head>
<body>
    <div class="box">
        <div class="multiplier">1.03×</div>
        <div class="divider"></div>
        <div class="value">
            <span>$0.00</span>
            <img src="https://upload.wikimedia.org/wikipedia/commons/a/a2/Litecoin_Logo.png" alt="Litecoin">
        </div>
    </div>
</body>
</html>
