<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Game Result Box</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #2c2f38;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }

    .game-result-wrap {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      background-color: #3a3f51;
      border-radius: 10px;
      width: 200px;
      padding: 20px;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3);
      color: #fff;
    }

    .number-multiplier {
      font-weight: bold;
      font-size: 1.5rem;
      white-space: nowrap;
      overflow: hidden;
      text-overflow: ellipsis;
      text-align: center;
      width: 100%;
      max-width: 180px; /* Increase this or remove to avoid truncation */
    }

    .divider {
      width: 80%;
      height: 1px;
      background-color: #5c6379;
      margin: 10px 0;
    }

    .payout-result {
      display: flex;
      align-items: center;
      font-size: 1rem;
    }

    .currency {
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .currency svg {
      width: 24px;
      height: 24px;
      margin-left: 5px;
    }

    /* Dynamic font size scaling */
    .number-multiplier span {
      font-size: calc(1.5rem + 0.25vw); /* Adjust size based on screen width */
    }
  </style>
</head>
<body>
  <div class="game-result-wrap">
    <div class="game-result-content">
      <span class="number-multiplier">
        <span>25500x</span>
      </span>
      <div class="divider"></div>
      <span class="payout-result">
        <div class="currency">
          <span class="content">$0.00</span>
          <svg fill="none" viewBox="0 0 96 96" class="svg-icon">
            <path d="M96 48c0 26.51-21.49 48-48 48S0 74.51 0 48 21.49 0 48 0s48 21.49 48 48Z" fill="#BFBBBB"></path>
            <path d="M31.275 57.645 27 59.31 29.07 51l4.32-1.74L39.645 24H55.02l-4.5 18.585 4.23-1.71-2.04 8.25-4.29 1.71-2.535 10.5H69L66.375 72H27.75l3.525-14.355Z" fill="#fff"></path>
          </svg>
        </div>
      </span>
    </div>
  </div>
</body>
</html>
