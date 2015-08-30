# LearningNodeJS with Express

Creating and setting up our initial node project with Express

1. Create a node project initial set up - type **npm init** (result will create package.json file containing all the details of your node app)
2. Install Express - While inside the project folder, **npm install express --save**. For info, express is a web framework use for node.js - http://expressjs.com/
3. Create your main JS file - usually then name is app.js or index.js (make sure it is the same name written in your package.json)
4. Inside the main JS file
	
		a. Require the module that will be using (here is it Express) then assign it to a variable so you can easily access it later
			var express = require('express');
		b. Create our app variable passing in the express method
			var app = express();
		c. Set up the development server using the listen method with the parameter of the port of your choice.
			app.listen(3000);

		>to run this, go to your console, make sure you are in your project folder and then type node app.js or node app (node then the name of the main js file)
		>go a browser and type in localhost:3000 (since we use 3000 as our port, if you use app.listen(8080), then run it at localhost:8000)
		>result will be a blank page that is running since we didn't request anything yet

		>To close the node serve - Control C

		>We can also add in a second parameter on the listen method. Here we are adding a callback function that tells the console to log "I'm Running".
		
			app.listen(3000, function(){
		  	  console.log("I'm running");
			}
		  Once you run the node app.js again, your terminal or console would show the word, I'm running.

Shortcut: use the express generator
http://expressjs.com/starter/generator.html
