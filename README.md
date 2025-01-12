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
            background-color: #0F1E28; /* Page background */
            font-family: Helvetica, "Helvetica Neue", Arial, sans-serif;
        }

        .box {
            min-width: 150px; /* Initial minimum width */
            min-height: 100px; /* Initial minimum height */
            background-color: #1A2C38;
            border: 5px solid #00FF00; /* Slightly larger green border */
            border-radius: 10px;
            padding: 20px; /* Padding for content spacing */
            display: flex;
            flex-direction: column;
            justify-content: space-evenly; /* Centers elements with equal spacing */
            align-items: center;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.5); /* Optional for better look */
            transition: transform 0.2s, width 0.2s, height 0.2s;
        }

        .box:hover {
            transform: scale(1.05); /* Slight zoom effect on hover */
        }

        .multiplier {
            font-size: 24px; /* Adjusted font size for consistency */
            font-weight: 700;
            color: #00FF00; /* Green text */
            margin: 0; /* Removed extra spacing */
        }

        .divider {
            width: 70%; /* Adjusted divider width */
            height: 3px; /* Increased thickness */
            background-color: #2F4553; /* Dark gray-blue */
            margin: 0; /* No extra margin for centering */
        }

        .value {
            display: flex;
            align-items: center;
            font-size: 16px; /* Updated font size for $0.00 */
            font-weight: 700; /* Match Helvetica bold weight */
            font-variant-numeric: tabular-nums; /* For equal spacing between digits */
            color: #00FF00; /* Green text */
            line-height: 120%; /* Proper line height */
            margin: 0; /* No extra spacing */
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
