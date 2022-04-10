# Getting started with P5JS and tramontana:

* Download tramontana for iOS or Android
* Download the [tramontana library](https://pierdr.github.io/Tramontana-for-Javascript/lib/tramontana_min.js) for javascript
* Download the [p5js library](https://cdnjs.cloudflare.com/ajax/libs/p5.js/0.5.4/p5.min.js)

Load the libraries in your html file:

```html
<!-- import jquery -->
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.0/jquery.min.js"></script>
<!-- import p5js -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/p5.js/0.5.4/p5.min.js"></script>
<!-- import tramontana -->
<script src="tramontana_min.js"></script>
```	

Now you can create a new tramontana object that links to your device.

```javascript
var device = new tramontana();  
```	
In the setup function you can call the start function of tramontana, that accepts 2 parameters. The first one is the ipAddress of your device (that you can see on your device, and the second is a callback function that is called if the connection succeed or fails. If the error is undefined the connection is successful and you can do a lot of things with tramontana, like for instance trigger the haptic engine of the device.

```javascript
function setup(){ 				
	createCanvas(600, 600); 				
	device.start("192.168.1.23",  function(e){
		if(e==undefined){
			//SUCCESS TRAMONTANA CONNECTED
			device.makeVibrate();
		}
	});
}

function draw()
{
	rect(10,10,100,100);
}
```	


You can check more examples here:
[ tramontana and p5js](https://github.com/pierdr/Tramontana-for-Javascript/blob/gh-pages/examples/D-example-p5-1.html)
[tramontana and p5js alternate example](https://github.com/pierdr/Tramontana-for-Javascript/blob/gh-pages/examples/E-example-p5-2.html)