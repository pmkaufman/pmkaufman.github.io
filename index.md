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
    

  <script>
 
 function getRandomInt(max) {
    return Math.floor(Math.random() * Math.floor(max));
  }
  
  var files = ['Seat.mp3', 'Sit.mp3', 'Sett.mp3'];
  var myAudio = document.getElementById("AudioFile");
  var rando = getRandomInt(3);
  var file = files[rando];
  
  
  
  document.write("<audio controls id='music'>");
  document.write("<source src='" + file + "' type='audio/mpeg' id='audioFile'>");
  document.write("<\/audio>");
  
  var myMusic= document.getElementById("music");
  
  function play() {
  myMusic.play();
  }

  function pause() {
  myMusic.pause();
  }
  
  var answer = docuemnt.getElementById("answer");
  
  function validate(n) {
    if (n == rando) {
      window.alert ("correct");
      //answer.innerHTML = "correct";
    }
    else {
      window.alert ("incorrect");
      //answer.innerHTML = "incorrect";
    }
  }
  </script>
  
   <p>Which word do you hear?</p>

  <button onclick="validate(0)">Seat</button>
  <button onclick="validate(1)">Sit</button>
  <button onclick="validate(2)">Set</button>
    

</body>
</html>
