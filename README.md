<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>For Arshia</title>
  <style>
    body { margin:0; display:flex; justify-content:center; align-items:center; height:100vh; background:#eee; }
    #button { padding:20px 30px; font-size:24px; color:#333; background:#fff; border:2px solid #333; cursor:pointer; border-radius:8px; }
    #scare { display:none; position:absolute; top:0; left:0; width:100%; height:100%; background:#000; justify-content:center; align-items:center; flex-direction:column; }
    #scare img { max-width:90%; max-height:90%; }
  </style>
</head>
<body>
  <div id="button">Hey Arshia, click here!</div>
  <div id="scare">
    <img src="https://cdn.pixabay.com/photo/2020/04/30/15/36/ghost-face-5116835_1280.png" alt="Horror Face" />
    <audio id="scream" src="https://actions.google.com/sounds/v1/alarms/beep_short.ogg"></audio>
  </div>

  <script>
    document.getElementById('button').onclick = () => {
      const scare = document.getElementById('scare');
      const scream = document.getElementById('scream');
      scare.style.display = 'flex';
      scream.play();
    };
  </script>
</body>
</html>
