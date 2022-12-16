# Compiladores
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Christmas Tree</title>

    <style>
      img {
        position: absolute;
      }

      .hide {
        opacity: 0;
      }
    </style>
  </head>
  <body>
    <input
      onchange="toggleImage('lightsImage')"
      checked
      type="checkbox"
      name="lights"
    />
    <label>Lights</label>
    <input
      onchange="toggleImage('starsImage')"
      checked
      type="checkbox"
      name="stars"
    />
    <label>Stars</label>
    <input
      onchange="toggleImage('snowmanImage')"
      checked
      type="checkbox"
      name="snowman"
    />
    <label>Snowman</label>
    <input
      onchange="toggleImage('frameworkImage')"
      checked
      type="checkbox"
      name="framework"
    />
    <label>Framework</label>
    <input
      onchange="toggleImage('topperImage')"
      checked
      type="checkbox"
      name="toopper"
    />
    <label>Topper</label>
    <br />
    <img src="images/tree.png" />
    <img id="starsImage" src="images/stars.png" />
    <img id="topperImage" src="images/topper.png" />
    <img id="lightsImage" src="images/lights.png" />
    <img id="snowmanImage" src="images/snowman.png" />
    <img id="frameworkImage" src="images/framework.png" />

    <script>
      function toggleImage(imageId) {
        document.getElementById(imageId).classList.toggle("hide");
      }
    </script>
  </body>
</html>
