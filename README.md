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
            font-size: 30px;
            font-weight: bold;
            color: #00FF00; /* Green text */
        }

        .divider {
            width: 60%; /* Shortened length */
            height: 1px;
            background-color: #2F4553; /* Updated to dark gray-blue */
            margin: 10px 0;
        }

        .value {
            display: flex;
            align-items: center;
            font-weight: normal; /* Reduced boldness */
            font-size: 16px;
            line-height: 120%;
            color: #00FF00; /* Green text */
        }

        .value span {
            font-size: 16px;
            line-height: 120%;
        }

        .value img {
            width: 20px;
            height: 20px;
            margin-left: 5px;
        }

        /* Placeholder for the Litecoin icon */
        .litecoin-icon {
            display: inline-block;
            width: 16px;
            height: 16px;
            background-color: #00FF00; /* Placeholder green circle */
            border-radius: 50%;
            margin-left: 5px;
        }
    </style>
</head>
<body>
    <div class="box">
        <div class="multiplier">25500×</div>
        <div class="divider"></div>
        <div class="value">
            <span>$0.00</span>
            <!-- Replace with actual Litecoin icon -->
            <div class="litecoin-icon"></div>
        </div>
    </div>
</body>
</html>
