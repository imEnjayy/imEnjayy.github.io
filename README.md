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
            height: 150px;
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
            font-size: 30px;
            font-weight: bold;
            color: #00FF00; /* Green text */
        }

        .value {
            font-size: 20px;
            color: #00FF00; /* Green text */
            display: flex;
            align-items: center;
            margin-top: 5px;
        }

        .value img {
            width: 20px;
            height: 20px;
            margin-left: 5px;
        }
    </style>
</head>
<body>
    <div class="box">
        <div class="multiplier">25500x</div>
        <div class="value">
            $0.00
            <img src="litecoin-icon.png" alt="Litecoin Icon">
        </div>
    </div>
</body>
</html>
