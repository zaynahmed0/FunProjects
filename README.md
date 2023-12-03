To run the Tic-Tac-Toe game from your macOS terminal, you need to serve the HTML file you create through a local web server and then open it in a web browser. You can use the built-in Python server if you have Python installed, or alternatively, you can also use Node.js with a package like http-server. I'll describe both methods.

Using Python's Built-in HTTP Server
Python 2.x:

python -m SimpleHTTPServer 8000
Python 3.x:

python3 -m http.server 8000
This will serve files from the current directory at http://localhost:8000.

Using Node.js with http-server
First, you need to install http-server globally on your machine (if you haven't already):

npm install -g http-server
Then you can run the following command in the directory where your HTML file is located:

http-server -p 8000
In both cases, once the server is running, open a web browser and navigate to http://localhost:8000. Your Tic-Tac-Toe game should be visible and playable from there.

Make sure to save the HTML file with the JavaScript and CSS included, and also make sure the terminal is focused on the directory where your game file is stored before you start the server.