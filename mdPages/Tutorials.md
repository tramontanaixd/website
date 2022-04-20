# Tutorials

<iframe width="560" height="315" src="https://www.youtube.com/embed/soQeHfPz668" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/cU_FQ7WaDII" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/x3KTCXundFo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/brbJFCR0BAI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/8S401sWb-vc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/13HzT9ng5LA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### How to host media on tramontana

#### iOS
To add files to tramontana iOS you can use the file sharing between iOS and macOS (it used to be between iOS and iTunes, now it happens directly in [Finder](https://support.apple.com/en-us/HT210598)):
 [youtube video](https://www.youtube.com/watch?v=x3KTCXundFo&lc=UgxqHPghCUz2BM6l9214AaABAg&feature=em-comments))

#### iOS and Android
1. You need to host a local HTTP server. One of the ways is to do it with python. If you are running OSX or Linux, you should already have python installed. If you are running Windows then head over to https://www.python.org/ to install it. 

2. Open your command prompt (Windows)/ terminal (macOS/ Linux). To check Python is installed, enter the following command: 

	```python 
	python -V
	# Or you might have the py command available,
	# in which case try py -V
	```	

3. This should return a version number. If this is OK, navigate to the directory that your example is inside, using the cd command. 

	```python
	# include the directory name to enter it, for example
	cd Desktop
	# use two dots to jump up one directory level if you need to
	cd ..
	```	

4. Enter the command to start up the server in that directory: 

	```python
	# If Python version returned above is 3.X
	python3 -m http.server
	# On windows try "python" instead of "python3", or "py -3"
	# If Python version returned above is 2.X
	python -m SimpleHTTPServer
	```	

5. By default, this will run the contents of the directory on a local web  server, on port 8000. You can go to this server by going to the URL localhost:8000 in your web browser. Here you'll see the contents of the directory listed — click the HTML file you want to run.

6. Use the url of the media you want to play or use in your processing sketch or javascript code or p5js code. 
