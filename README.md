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
            width: 160px; /* Square dimensions */
            height: 160px; /* Square dimensions */
            background-color: #1A2C38; /* Inner box background color */
            border: 5px solid #00FF00; /* Green border */
            border-radius: 10px;
            display: flex;
            flex-direction: column;
            justify-content: space-between; /* Distribute items evenly */
            align-items: center;
            padding: 15px; /* Inner spacing */
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.5); /* Subtle shadow */
            transition: transform 0.2s, width 0.2s, height 0.2s;
        }

        .box:hover {
            transform: scale(1.05); /* Slight zoom effect on hover */
        }

        .multiplier {
            font-size: 24px; /* Font size for "1.03×" */
            font-weight: 700;
            color: #00FF00; /* Green text */
            margin: 0; /* No extra margin */
        }

        .divider {
            width: 60%; /* Adjusted divider width */
            height: 2px; /* Adjusted divider thickness */
            background-color: #2F4553; /* Divider color */
            margin: 0; /* No extra margin */
        }

        .value {
            display: flex;
            align-items: center;
            font-size: 16px; /* Font size for $0.00 */
            font-weight: 700; /* Bold style for dollar amount */
            font-variant-numeric: tabular-nums; /* Equal digit spacing */
            color: #00FF00; /* Green text */
            line-height: 120%; /* Proper line height */
            margin: 0; /* No extra margin */
        }

        .value img {
            width: 18px; /* Litecoin logo size */
            height: 18px;
            margin-left: 5px; /* Space between text and logo */
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
