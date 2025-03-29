<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Project Zero</title>
    <style>
        body {
            background: linear-gradient(135deg, #000 25%, transparent 25%) -50px 0, linear-gradient(225deg, #000 25%, transparent 25%) -50px 0, linear-gradient(315deg, #000 25%, transparent 25%), linear-gradient(45deg, #000 25%, transparent 25%);
            background-size: 100px 100px;
            background-color: #222;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            color: white;
            text-align: center;
            animation: moveBackground 20s linear infinite; /* Add animation */
        }
        .moon {
            width: 200px;
            height: 200px;
            background-color: red;
            border-radius: 50%;
            box-shadow: 0 0 50px 20px rgba(255, 0, 0, 0.5); /* Red light effect */
            position: relative;
            top: 100px; /* Move the moon down */
            transform: rotate(-45deg); /* Rotate the moon to the left */
        }
        .button-container {
            display: flex;
            gap: 20px;
            position: relative;
            top: 90px; /* Move the buttons slightly up */
            left: 20px; /* Move the buttons slightly to the right */
            animation: fadeIn 2s infinite alternate; /* Add animation */
        }
        .button {
            display: inline-block;
            padding: 10px 20px;
            font-size: 16px;
            color: white;
            background-color: black;
            border: none;
            border-radius: 5px;
            text-decoration: none;
            cursor: pointer;
        }
        .main-page-button {
            display: inline-block;
            padding: 10px 20px;
            font-size: 16px;
            color: white;
            background-color: black;
            border: none;
            border-radius: 5px;
            text-decoration: none;
            cursor: pointer;
            margin-top: 20px;
        }
        h1 {
            margin: 0;
            font-size: 5em; /* Make the text larger */
            color: white;
            text-align: center;
            position: relative;
            top: 50px; /* Adjust position to align with the moon */
            animation: fadeIn 2s infinite alternate; /* Add animation */
        }
        .description {
            margin-top: 20px;
            font-size: 1.5em;
            color: white;
            position: relative;
            top: 80px; /* Move the description text slightly up */
            animation: fadeIn 2s infinite alternate; /* Add animation */
        }
        .tos-content {
            display: none;
            margin-top: 20px;
            font-size: 1.2em;
            color: white;
            text-align: left;
            animation: slideIn 1s ease-out forwards; /* Add different animation */
        }
        @keyframes fadeIn {
            0% { opacity: 0; }
            100% { opacity: 1; }
        }
        @keyframes moveBackground {
            0% { background-position: 0 0, 0 0, 0 0, 0 0; }
            100% { background-position: 100px 100px, 100px 100px, 100px 100px, 100px 100px; }
        }
        @keyframes slideIn {
            0% { transform: translateX(-100%); opacity: 0; }
            100% { transform: translateX(0); opacity: 1; }
        }
    </style>
</head>
<body>
    <div class="moon"></div>
    <h1>Project Zero</h1>
    <div class="description">Roblox #1 ServerSide On The Market<br>Good TOS and Cheap<br>Buy Now!</div>
    <div class="button-container">
        <a href="https://discord.gg/jsfCbVMM" class="button">Discord</a>
        <a href="https://www.youtube.com/@Cendicate" class="button">YouTube</a>
        <a class="button" onclick="showTOS()">TOS</a>
    </div>
    <div class="tos-content">
        <p>Follow Our TOS Or You Will Be Blacklisted</p>
        <p>#1 - No External Executors<br>Serversided external executors disallow staff from reviewing scripts executed, granting users to execute scripts and potentially destroy a game.</p>
        <p>#2 - No Script Viewers<br>Scripts such as Dex are prohibited since users can modify the game itself in anyway including deleting the entire map and mass killing players in-game.</p>
        <p>#3 - No NSFW Scripts<br>Scripts such as GKV4 and Nekos are strictly prohibited as they can lead to our games getting moderated.</p>
        <p>#3 - No Map Changers<br>Modifying the entire game map itself to load in a different map is highly prohibited.</p>
        <p>#4 - No mass kicking/banning<br>Mass Kicking users from games leads to our game's player count to decrease. Mass banning players from games prevents them from joining any other server from the game.</p>
        <p>#5 - No Snitching</p>
        <p>#6 - No things like k00pgui Or C00lguis or Destructive GUIS</p>
        <a class="main-page-button" onclick="showMainPage()">MAIN PAGE</a>
    </div>
    <script>
        function showTOS() {
            document.querySelector('.moon').style.display = 'none';
            document.querySelector('h1').style.display = 'none';
            document.querySelector('.description').style.display = 'none';
            document.querySelector('.button-container').style.display = 'none';
            document.querySelector('.tos-content').style.display = 'block';
        }

        function showMainPage() {
            document.querySelector('.moon').style.display = 'block';
            document.querySelector('h1').style.display = 'block';
            document.querySelector('.description').style.display = 'block';
            document.querySelector('.button-container').style.display = 'flex';
            document.querySelector('.tos-content').style.display = 'none';
        }
    </script>
</body>
</html>
