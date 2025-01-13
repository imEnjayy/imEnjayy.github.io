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
        height: 2.7px; /* Divider thickness */
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
</style>
