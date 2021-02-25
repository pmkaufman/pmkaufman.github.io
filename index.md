<!-- <!doctype html> -->

<html lang="en">
<head>
  <meta charset="utf-8">

  <title>The HTML5 Herald</title>
  <meta name="description" content="The HTML5 Herald">
  <meta name="author" content="SitePoint">

  <link rel="stylesheet" href="css/styles.css?v=1.0">

</head>

<body>
  
    <audio controls id="music">
     <source src="Sit.mp3" type="audio/mpeg" id='audioFile'>
    </audio>
    
    <p>Which word do you hear?</p>

    <div>
      <input type="radio" id="seat" name="word" value="seat"
             checked>
      <label for="seat">Seat</label>
    </div>

    <div>
      <input type="radio" id="sit" name="word" value="sit">
      <label for="sit">Sit</label>
    </div>

    <div>
      <input type="radio" id="set" name="word" value="set">
      <label for="set">Sett</label>
    </div>

  <script>
  
  var files = ['Seat.mp3', 'Sit.mp3', 'Sett.mp3'];
  var myAudio = document.getElementById("AudioFile");
  myAudio.src = files[Math.random(3)];
  
  var myMusic= document.getElementById("music");
  
  function play() {
  myMusic.play();
  }

  function pause() {
  myMusic.pause();
  }
  </script>

</body>
</html>
