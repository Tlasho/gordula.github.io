<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Christmas Wonderland</title>
    <style>
        /* General Styles */
        body {
            font-family: 'Arial', sans-serif;
            margin-top: -50px;
            padding: 0px;
            text-align: center;
            height: 200vh;
            background: url('https://scontent.xx.fbcdn.net/v/t1.15752-9/462577208_1643031869904576_1495850150853641523_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=0024fc&_nc_ohc=4B75baiSZQYQ7kNvgF6fmo7&_nc_ad=z-m&_nc_cid=0&_nc_zt=23&_nc_ht=scontent.xx&oh=03_Q7cD1QFRBPtM3J3dTniU3UzucClKRt5zgAtovqCaPIjGE7XSKQ&oe=6787D448') no-repeat center center fixed; /* Christmas background */
            background-size: cover;
            color: white;
            overflow: hidden;
            position: relative; /* To position snowflakes, boxes, etc. */
        }

        /* Snowflakes Animation */
        .snowflake {
            position: fixed;
            color: white;
            font-size: 2em; /* Increased size of snowflakes */
            z-index: 999;
            animation: fall linear infinite;
        }

        @keyframes fall {
            0% {
                transform: translateY(-100px) translateX(0px);
                opacity: 1;
            }
            100% {
                transform: translateY(100vh) translateX(30px);
                opacity: 0;
            }
        }

        /* Christmas Gift Boxes */
        .gift-box {
            position: absolute;
            bottom: 0;
            width: 150px;
            height: 150px;
            background: url('gift-box.png') no-repeat center center;
            background-size: contain;
            animation: bounce 2s infinite alternate;
            z-index: 5;
        }

        .gift-box-left {
            left: 10%;
        }

        .gift-box-right {
            right: 10%;
        }

        /* Bouncing Animation for Gift Boxes */
        @keyframes bounce {
            0% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-20px);
            }
            100% {
                transform: translateY(0);
            }
        }

        /* Main Section */
        #main {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            flex-grow: 1;
            margin-top: 100px;
            position: relative;
        }

        /* Buttons */
        /* Buttons */
.big-button {
    transition-duration: 400ms;
    margin: 60px; /* Increased the space between buttons */
    padding: 40px;
    font-size: 22px;
    background-color: #000c5b;
    color: white;
    border: none;
    border-radius: 100px;
    cursor: pointer;
    width: 300px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3);
    z-index: 10;
}

.big-button:hover {
    background-color: #cc0000;
}


        /* Christmas Decorations: Stars and Lights */
        .star {
            position: fixed;
            top: 0;
            left: 50%;
            transform: translateX(-50%);
            font-size: 3em;
            color: gold;
            animation: twinkle 1.5s infinite alternate;
        }

        .star:nth-child(2) {
            left: 10%;
            animation-duration: 2s;
        }

        .star:nth-child(3) {
            left: 80%;
            animation-duration: 3s;
        }

        @keyframes twinkle {
            0% {
                opacity: 1;
            }
            100% {
                opacity: 0.5;
            }
        }

        .garland {
            position: absolute;
            top: 20%;
            left: 50%;
            transform: translateX(-50%);
            font-size: 2em;
            color: red;
            animation: swing 3s ease-in-out infinite;
        }

        @keyframes swing {
            0% {
                transform: translateX(-50%) rotate(0deg);
            }
            50% {
                transform: translateX(-50%) rotate(15deg);
            }
            100% {
                transform: translateX(-50%) rotate(0deg);
            }
        }

        /* Christmas Tree Animation */
        .tree {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            font-size: 3em;
            color: green;
            animation: bounce-tree 1.5s infinite alternate;
        }

        @keyframes bounce-tree {
            0% {
                transform: translate(-50%, -50%) rotate(0deg);
            }
            50% {
                transform: translate(-50%, -60%) rotate(10deg);
            }
            100% {
                transform: translate(-50%, -50%) rotate(0deg);
            }
        }
    </style>
</head>
<body>
    <!-- Snowflakes -->
    <div class="snowflake" style="left: 10%; animation-duration: 6s;">❄</div>
    <div class="snowflake" style="left: 20%; animation-duration: 8s;">❅</div>
    <div class="snowflake" style="left: 30%; animation-duration: 10s;">❄</div>
    <div class="snowflake" style="left: 40%; animation-duration: 7s;">❅</div>
    <div class="snowflake" style="left: 50%; animation-duration: 12s;">❄</div>
    <div class="snowflake" style="left: 60%; animation-duration: 9s;">❅</div>
    <div class="snowflake" style="left: 70%; animation-duration: 5s;">❄</div>
    <div class="snowflake" style="left: 80%; animation-duration: 11s;">❅</div>
    <div class="snowflake" style="left: 90%; animation-duration: 15s;">❄</div>
    <div class="snowflake" style="left: 5%; animation-duration: 13s;">❅</div>
    <div class="snowflake" style="left: 15%; animation-duration: 7s;">❄</div>
    <div class="snowflake" style="left: 25%; animation-duration: 14s;">❅</div>
    <div class="snowflake" style="left: 35%; animation-duration: 6s;">❄</div>
    <div class="snowflake" style="left: 45%; animation-duration: 8s;">❅</div>
    <div class="snowflake" style="left: 55%; animation-duration: 9s;">❄</div>
    <!-- Added 15 more snowflakes -->
    <div class="snowflake" style="left: 12%; animation-duration: 10s;">❄</div>
    <div class="snowflake" style="left: 22%; animation-duration: 5s;">❅</div>
    <div class="snowflake" style="left: 32%; animation-duration: 11s;">❄</div>
    <div class="snowflake" style="left: 42%; animation-duration: 6s;">❅</div>
    <div class="snowflake" style="left: 52%; animation-duration: 8s;">❄</div>
    <div class="snowflake" style="left: 62%; animation-duration: 9s;">❅</div>
    <div class="snowflake" style="left: 72%; animation-duration: 7s;">❄</div>
    <div class="snowflake" style="left: 82%; animation-duration: 10s;">❅</div>
    <div class="snowflake" style="left: 92%; animation-duration: 12s;">❄</div>
    <div class="snowflake" style="left: 7%; animation-duration: 8s;">❅</div>
    <div class="snowflake" style="left: 17%; animation-duration: 9s;">❄</div>
    <div class="snowflake" style="left: 27%; animation-duration: 14s;">❅</div>
    <div class="snowflake" style="left: 37%; animation-duration: 6s;">❄</div>
    <div class="snowflake" style="left: 47%; animation-duration: 5s;">❅</div>
    <div class="snowflake" style="left: 57%; animation-duration: 10s;">❄</div>
    <div class="snowflake" style="left: 67%; animation-duration: 11s;">❅</div>
    <div class="snowflake" style="left: 77%; animation-duration: 6s;">❄</div>
    <div class="snowflake" style="left: 87%; animation-duration: 13s;">❅</div>

    <!-- Christmas Decorations: Stars, Garland, Tree -->
    <div class="star">★</div>
    <div class="star">★</div>
    <div class="star">★</div>
    <div class="garland">🎄✨</div>
    <div class="tree">🎄</div>

    <!-- Christmas Gift Boxes -->
    <div class="gift-box gift-box-left"></div>
    <div class="gift-box gift-box-right"></div>

    <!-- Main Section -->
    <div id="main">
        <a href="before.html"><button class="big-button">Before the Exam</button></a>
        <a href="after.html"><button class="big-button">After the Exam</button></a>
        <a href="photos.html"><button class="big-button">Photos</button></a>
    </div>
</body>
</html>
