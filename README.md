<!doctype html>
<html lang="en">
    <head>
        <title></title>
        <style>
            .card{
                position: relative;
                float: left;
                width: 350px;
                height: 500px;
                text-align: center;
            }

            .wonDeck{
                position: absolute;
                bottom: 0;
                width: 75px;
                height: 100px;
                text-align: center;
            }

            .card{
                margin: 0 5%;
            }

            .card:first-of-type{
                margin-left: 0;
            }

            .card:last-of-type{
                margin-right: 0;
            }

            .card .text{
                position: absolute;
                margin: 0 0 0 -25%;
                left: 35%;
                height: 30%;
                width: 50%;
                font-size: 26px;
                color: rgb(150, 150, 150);
            }

            .wonDeck .text{
                position: absolute;
                margin: 0 0 0 -25%;
                left: 50%;
                height: 30%;
                width: 50%;
                font-size: 16px;
                color: rgb(150, 150, 150);
            }

            .warDeck .text{
                position: absolute;
                margin: 0 0 0 -25%;
                left: 50%;
                height: 30%;
                width: 50%;
                font-size: 16px;
                color: rgb(150, 150, 150);
            }

            .cardHolder{
                position: absolute;
                top: 0;
                left: 0;
                width: 75%;
                height: 350px;
                font-size: 26px;
                color: rgb(0, 0, 0);
                border: 1px dashed black;
                background-color: rgba(0, 0, 0, 0.5);
            }

            .wonCardsHolder, .warCardsHolder{
                position: absolute;
                top: 0;
                left: 0;
                width: 100%;
                height: 100%;
                font-size: 16px;
                color: rgb(0, 0, 0);
                border: 1px dashed black;
                background-color: rgba(0, 0, 0, 0.5);
            }


            .warDeck{
                position: relative;
                float: right;
                width: 75px;
                height: 100px;
            }

            #reshuffle{
                display: none;
            }
        </style>
    </head>
    <body>
        <div id="player1CurrentCard" class="card">
            <div class="warDeck">
                <div class="warCardsHolder"></div>
                <div class="text">
                    <p>War Deck</p>
                </div>
            </div>
            <div class="cardHolder"></div>

            <div class="text">
                <p>Player 1 Card</p>
            </div>
            <div id="player1WonDeck" class="wonDeck">
                <div class="wonCardsHolder"></div>
                <div class="text">
                    <p>Won Deck</p>
                </div>
            </div>
        </div>

        <div id="player2CurrentCard" class="card">
            <div class="cardHolder"></div>
            <div class="warDeck">
                <div class="warCardsHolder"></div>
                <div class="text">
                    <p>War Deck</p>
                </div>
            </div>
            <div class="text">
                <p>Player 2 Card</p>
            </div>
            <div id="player2WonDeck" class="wonDeck">
                <div class="wonCardsHolder"></div>
                <div class="text">
                    <p>Won Deck</p>
                </div>
            </div>
        </div>
        <button id="play">Play</button>
        <button id="reshuffle">Reshuffle</button>
    </body>
    <script src="war.js"></script>
</html>
