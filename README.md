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
            min-width: 150px; /* Initial minimum width */
            min-height: 100px; /* Initial minimum height */
            background-color: #1A2C38;
            border: 5px solid #00FF00; /* Slightly larger green border */
            border-radius: 10px;
            padding: 20px; /* Padding for content spacing */
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.5); /* Optional for better look */
            transition: transform 0.2s, width 0.2s, height 0.2s;
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
            margin: 7px 0; /* Adjusted margin to center divider */
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

        .value svg {
            width: 18px; /* Adjusted size for SVG */
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
            <svg fill="none" viewBox="0 0 96 96" class="svg-icon" style="">
                <title>Litecoin</title>
                <path d="M96 48c0 26.51-21.49 48-48 48S0 74.51 0 48 21.49 0 48 0s48 21.49 48 48Z" fill="#BFBBBB"></path>
                <path d="M31.275 57.645 27 59.31 29.07 51l4.32-1.74L39.645 24H55.02l-4.5 18.585 4.23-1.71-2.04 8.25-4.29 1.71-2.535 10.5H69L66.375 72H27.75l3.525-14.355Z" fill="#fff"></path>
            </svg>
        </div>
    </div>
</body>
</html>
