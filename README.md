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
            min-height: 100vh;
            margin: 0;
            background-color: #1e1e2d;
            font-family: Arial, sans-serif;
        }

        .box {
            width: 150px;
            height: 150px;
            background-color: #2a2a40;
            border: 3px solid transparent; /* Placeholder for hover effect */
            border-radius: 12px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: white;
            transition: border-color 0.3s;
        }

        .box:hover {
            border-color: #00ff00; /* Green border on hover */
        }

        .box .multiplier {
            font-size: 1.5rem; /* Dynamic font size for better fit */
            font-weight: bold;
            margin-bottom: 10px;
        }

        .box .divider {
            width: 80%;
            height: 1px;
            background-color: #555;
            margin-bottom: 10px;
        }

        .box .value {
            font-size: 1rem;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .box .value .currency {
            margin-left: 5px;
            width: 16px;
            height: 16px;
        }
    </style>
</head>
<body>

    <div class="box">
        <div class="multiplier">25500x</div>
        <div class="divider"></div>
        <div class="value">
            $0.00 <img src="https://via.placeholder.com/16" alt="Litecoin" class="currency">
        </div>
    </div>

</body>
</html>
