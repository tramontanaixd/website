# Getting started with Javascript and tramontana:

* Getting started with Javascript and tramontana::

* Download tramontana for iOS or Android
 
* Download the tramontana library for [javascript](https://pierdr.github.io/Tramontana-for-Javascript/lib/tramontana_min.js)

To get started with tramontana for Javascript you need to first import jquery:


```html
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.0/jquery.min.js"></script>
```


And then import the tramontana library:

```html
<script src="../lib/tramontana_min.js"></script>
```

Now you can create a new tramontana object that links to your device (or node).

```html
<script>   var device = new tramontana();  </script>
```
 Open the tramontana app on your phone and check the ip address of your device:
 
```javascript
device.start(“192.168.2.19”)
```	

Now you are ready to send your first command to your device:

```javascript
device.makeVibrate();
```	



This is the html page for the full example: 



```html
	<html>
	<head>
	<!-- import css-->
	<link rel="stylesheet" type="text/css" href="./stylesheet.css">
	<!-- import jquery-->
	 <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.0/jquery.min.js"></script>
	<!-- import tramontana-->
	 <script src="../lib/tramontana_min.js"></script>
	<!-- create a global variable-->
	 <script>
	  var device = new tramontana();
	 </script>
	</head>
	<body>
	 <!--Link to tramontana the app!-->
	 <div>
	 <h4>To get started download the Tramontana App on your iOS device from <a href="https://itunes.apple.com/us/app/tramontana/id1121069555?mt=8">here</a> or on your Android device from <a href="https://itunes.apple.com/us/app/tramontana/id1121069555?mt=8">here</a>.</h4>
	 <p>
	  1. Insert the IP Address of your device and press start.
	 </p>
	 <p>
	  2. Press change color to change the color of the screen of your device.
	 </p>
	 </div>
	 <!-- OPEN SOCKET -->
	 <label>IPAddress:</label>
	 <input type="text" id="ipInput" placeholder="192.168.1.1"><br/>
	 <button onclick="device.start($('#ipInput').val())">start</button>
	 <!-- CHANGE device COLOR -->
	 <button onclick="console.log('change color');device.setColor(Math.random(0,255),Math.random(0,255),Math.random(0,255),255
	 );">change color</button>
	 </p>
	</body>
	</html>
```	

You can check more examples here:

[A. Hello World!](https://github.com/pierdr/Tramontana-for-Javascript/blob/gh-pages/examples/A-example-helloWorld.html)
[B. sensing, subscribe to orientation event.](https://github.com/pierdr/Tramontana-for-Javascript/blob/gh-pages/examples/B-example-subscribeOrientation.html)
[C. sensing, all inputs from device.](https://github.com/pierdr/Tramontana-for-Javascript/blob/gh-pages/examples/C-example-all-sensors.html)
[D. tramontana and p5js (processingjs)](https://github.com/pierdr/Tramontana-for-Javascript/blob/gh-pages/examples/D-example-p5-1.html)
[E. tramontana and p5js alternate example](https://github.com/pierdr/Tramontana-for-Javascript/blob/gh-pages/examples/E-example-p5-2.html)
[F. tramotnana hardware](https://github.com/pierdr/Tramontana-for-Javascript/blob/gh-pages/examples/F-example-hardware.html)