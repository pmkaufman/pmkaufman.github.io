<!doctype html>

<html lang="en">
<head>
  <meta charset="utf-8">

  <title>The HTML5 Herald</title>
  <meta name="description" content="The HTML5 Herald">
  <meta name="author" content="SitePoint">

  <link rel="stylesheet" href="css/styles.css?v=1.0">

</head>

<body>
    <h1> foo bar baz </h1>
  
    <audio controls id="music">
     <source src="Sit.mp3" type="audio/mpeg">
    </audio>

  <script>
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
