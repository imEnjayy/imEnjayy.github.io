<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Styled Box</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #000000; /* Page background: black */
            font-family: Helvetica, "Helvetica Neue", Arial, sans-serif;
        }

        .box {
            width: 150px; /* Fixed width */
            height: 150px; /* Fixed height */
            background-color: #1A2C38;
            border: 5px solid #00FF00; /* Green border */
            border-radius: 10px;
            padding: 20px; /* Padding for content spacing */
            display: flex;
            flex-direction: column;
            justify-content: center; /* Center content vertically */
            align-items: center;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.5); /* Optional for better look */
            transition: transform 0.2s;
        }

        .box:hover {
            transform: scale(1.05); /* Slight zoom effect on hover */
        }

        .multiplier {
            font-size: 24px; /* Font size for the multiplier */
            font-weight: 700;
            color: #00FF00; /* Green text */
        }

        .divider {
            width: 60%; /* Divider width */
            height: 3.5px; /* Divider thickness */
            background-color: #2F4553; /* Dark gray-blue */
            margin: 15px 0; /* Adjusted margin to center divider */
        }

        .value {
            display: flex;
            align-items: center;
            font-size: 16px; /* Font size for $0.00 */
            font-weight: 700; /* Match Helvetica bold weight */
            font-variant-numeric: tabular-nums; /* For equal spacing between digits */
            color: #00FF00; /* Green text */
            line-height: 120%; /* Proper line height */
        }

        .value span {
            font-size: 16px;
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
