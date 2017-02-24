---
layout: default
permalink: /OpenLayers

modified: 2017-02-23
---
<html>
  <head>

    <!-- The line below is only needed for old environments like Internet Explorer and Android 4.x -->
    <script src="https://cdn.polyfill.io/v2/polyfill.min.js?features=requestAnimationFrame,Element.prototype.classList,URL"></script>

    <script src="assets/js/ol.js"></script>
    <script src="assets/js/proj4.js"></script>

    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="chrome=1">
    <meta name="viewport" content="initial-scale=1.0, user-scalable=no, width=device-width">
    <style type="text/css">
      html, body, .map {
        margin: 0;
        padding: 0;
        width: 100%;
        height: 256px;
      }
     </style>
  <style>
  .map:-moz-full-screen {
    height: 100%;
  }
  .map:-webkit-full-screen {
    height: 100%;
  }
  .map:-ms-fullscreen {
    height: 100%;
  }
  .map:fullscreen {
    height: 100%;
  }
  .ol-rotate {
    top: 3em;
  }
</style>
  <link rel="stylesheet" href="assets/css/ol.css" type="text/css">
  </head>
  <body>
    <div id="map" class="map"></div>
    <div id="info" style="display: none;"></div>
    <div class="icon-github"></div>
    <label for="track">
      paikanna sijainti
      <input id="track" type="checkbox"/>
    </label>
    <p>
      sijainti: <code id="position"></code>&nbsp;&nbsp;
      paikannustarkkuus: <code id="accuracy"></code>&nbsp;&nbsp;
      korkeus merenpinnasta: <code id="altitude"></code>&nbsp;&nbsp;
      korkeuden tarkkuus: <code id="altitudeAccuracy"></code>&nbsp;&nbsp;
      suunta: <code id="heading"></code>&nbsp;&nbsp;
      nopeus: <code id="speed"></code>
    </p>

    <script src="assets/js/bundlegeoloc.js" charset="UTF-8"> </script>

  </body>
</html>
