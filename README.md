<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For Mitali</title>
    <style>
        body { font-family: sans-serif; display: flex; flex-direction: column; align-items: center; background-color: #fce4ec; padding: 20px; }
        .card { background: white; padding: 2rem; border-radius: 20px; box-shadow: 0 10px 25px rgba(0,0,0,0.1); margin-bottom: 20px; text-align: center; max-width: 400px; width: 100%; }
        h1 { color: #d81b60; }
        button { padding: 10px 20px; font-size: 1rem; background-color: #d81b60; color: white; border: none; border-radius: 10px; cursor: pointer; margin: 10px; }
        textarea { width: 100%; height: 100px; margin: 10px 0; border: 2px solid #fce4ec; border-radius: 10px; padding: 10px; box-sizing: border-box; }
        #smile-msg, #vent-result { display: none; margin-top: 15px; font-weight: bold; color: #555; }
    </style>
</head>
<body>

    <!-- Click for a Smile -->
    <div class="card">
        <h1>Hi Mitali! ✨</h1>
        <button onclick="document.getElementById('smile-msg').style.display='block'">Click for a smile</button>
        <div id="smile-msg">Everything will be okay! You're amazing. 🌸💖</div>
    </div>

    <!-- Vent & Release -->
    <div class="card">
        <h3>Need to vent?</h3>
        <textarea id="ventInput" placeholder="Type here to let it all out..."></textarea>
        <button onclick="release()">Let it go</button>
        <div id="vent-result">Everything you wrote is now gone. Take a deep breath—you are stronger than any bad day! 🌟</div>
    </div>

    <!-- Bonus Surprise -->
    <div class="card" style="border-top: 5px solid #d81b60;">
        <p><em>P.S. I believe your hands are the prettiest! </em> 💖✨🌈🌟🎈🎉🎊🍭🍬🦋🌸🌻💫🎀🤩🥳🎈🙌✨💖🥰🫶💖💫💫💖 </p>
    </div>

    <script>
        function release() {
            document.getElementById('ventInput').value = '';
            document.getElementById('vent-result').style.display = 'block';
        }
    </script>
</body>
</html>
