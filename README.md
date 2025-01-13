<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Box</title>
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
            min-width: 150px;
            min-height: 100px;
            background-color: #1A2C38;
            border: 5px solid #00FF00; /* Slightly larger green border */
            border-radius: 10px;
            padding: 20px;
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

        .value svg {
            width: 18px; /* Adjusted size for SVG */
            height: 18px;
            margin-left: 5px;
        }

        .inputs {
            margin-top: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
            color: white;
        }

        .inputs label {
            margin-bottom: 5px;
            font-size: 14px;
        }

        .inputs input {
            margin-bottom: 10px;
            padding: 5px;
            font-size: 14px;
            border: 1px solid #00FF00;
            border-radius: 5px;
            background-color: #1A2C38;
            color: #FFFFFF;
        }

        .inputs button {
            padding: 5px 10px;
            font-size: 14px;
            color: #FFFFFF;
            background-color: #00FF00;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.2s;
        }

        .inputs button:hover {
            background-color: #00CC00;
        }
    </style>
</head>
<body>
    <div>
        <div class="box">
            <div class="multiplier" id="multiplier">1.03×</div>
            <div class="divider"></div>
            <div class="value">
                <span id="dollar-amount">$0.00</span>
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 128 128" fill="#FFFFFF">
                    <path d="M64 8C33.43 8 8 33.43 8 64s25.43 56 56 56 56-25.43 56-56S94.57 8 64 8zm0 104c-
