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
  
 <!--  <audio controls id="music">
      <source src="Sit.mp3" type="audio/mpeg" id='audioFile'>
    </audio>  -->
    
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
      <label for="set">Set</label>
    </div>

  <script>
 
 function getRandomInt(max) {
    return Math.floor(Math.random() * Math.floor(max));
  }
  
  var files = ['Seat.mp3', 'Sit.mp3', 'Sett.mp3'];
  var myAudio = document.getElementById("AudioFile");
  var file = files[getRandomInt(3)];
  
  
  
  document.write("<audio controls id='music'>");
  document.write("<source src='" + file + "' type='audio/mpeg' id='audioFile'>");
  document.write("<\/audio>");
  
  
  /*var audio = document.createElement('audio');  

    
  var source = document.createElement('source');
  source.setAttribute("src", file);
  source.setAttribute("type", "audio/mpeg");
  source.setAttribute("id", "audioFile");
    
  audio.appendChild(source);
    
  audio.load();*/
  
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
