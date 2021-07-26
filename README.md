# bukan_gombalan
 seruseruan
<html>
    <body>
        <h1>Heiii kaum tersesat</h1>
        <img src="https://images.pojoksatu.id/2016/12/dr-zakir-naik-1.jpg">
        <h1>
            Mau muallaf tidak?
        <button id='btn_music' onclick='music()'>Play/Pause</button>
        </h1>
        <button id='btn_mau' onclick='alert("Oke ikut saya, Asyhadu an laa ilaaha illallaahu, wa asyhaduanna muhammadar rasuulullah ")'>Mau bangeett</button>&nbsp;
        <button id='btn_gamau' onclick='gamau(this)' style='position:absolute'>Gamau</button>
         <audio id='bgMusic' src='https://media1.vocaroo.com/mp3/14rEFgH9fwA6' loop></audio>
    </body>
    <script>
        function gamau(id){
            var mau = document.getElementById('btn_mau');
            var i = Math.floor(Math.random()*300)+1;
            var j = Math.floor(Math.random()*100)+mau.offsetTop;
            id.style.left = i+'px';
            id.style.top = j+'px';
        }
         var audioPlaying = false;
        function music(){
            var audio = document.getElementById("bgMusic");
            if (!audioPlaying) audio.play();
            else audio.pause();
            audioPlaying = !audioPlaying;
        }
    </script>
</html>
