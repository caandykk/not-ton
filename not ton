<html>
    <head>
        <style>
            body {
                background-image: url('https://i.ytimg.com/vi/TsTcIj3G2WI/hq720.jpg?sqp=-oaymwEhCK4FEIIDSFryq4qpAxMIARUAAAAAGAElAADIQj0AgKJD&rs=AOn4CLDVe34vq6izfxNEJif9FbVu3alHXg');
                background-repeat: no-repeat;
                background-size: cover;
                font-family: 'Courier New', monospace;
            }
            .clicker {
                position:relative;
                top: 50%;
                left: 50%;
                width:200px;
                height:200px;
                background-color: #0000FF;
                border-radius: 50%;
                transform: translate(-50%, -50%);
                display: flex;
                justify-content: center;
                align-items: center;
                color: #FFFFFF;
            }
            #coins_counter {
                position: absolute;
                top: 10px;
                left: 10px;
                width: 200px;
                height: 200px;
                background: white;
                padding: 20px;
                display: flex;
                flex-direction: row;
                align-items: center;
                justify-content: space-around;
            }
            #coins_counter img {
                width: 50px;
                height: 50px;
                margin-left: 20px;
            }
            .coin_amount {
                font-size:20px;
                color: black;
            }
            .clicks_amount {
                font-size:20px;
                color: black;
            }
        </style>
        <script>
            var coins = 0;
            var clicks = 1500;
            
            function clicker() {
                if (clicks > 0) {
                    coins += 1;
                    clicks -= 1;
                    update();
                } else {
                    alert('У вас закончились клики! Подождите пока они восстановятся.');
                }
            }
            function update() {
                document.getElementById("clicks_amount").innerHTML = "Оставшиеся клики: " + clicks;
                document.getElementById("coin_amount").innerHTML = "Монеты: " + coins;
            }
            function refill() {
                if (clicks < 1500) {
                    clicks += 1;
                }
                update();
            }
            
            setInterval(refill, 1000);
        </script>
    </head>
    <body>
        <div onclick="clicker()" class="clicker">
            Click me!
        </div>
        <div id="coins_counter">
            <img src="https://img.freepik.com/premium-vector/coin-for-the-game-isolated-on-white-background_907924-42.jpg" alt="coin">
            <div id="coin_amount" class="coin_amount">Монеты: 0</div>
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTFJA-9oZvp5-5KhSZ1_R-sD5FqpI9h-dypXSPuOOJ9Lg&s" alt="coin2">
            <div id="clicks_amount" class="clicks_amount">Оставшиеся клики: 1500</div>
        </div>
    </body>
</html>
