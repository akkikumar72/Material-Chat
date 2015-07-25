## Setup and configuration
1. Make Sure you have IP address with you. If using Mac use : **ipconfig getifaddr en0**.

Replace: 
10.24.197.188 with your own IP Address.

**2.Node installed in System**

**3.Internet available in latest Browser.
**

Make sure that you update **server.js**
and add your own IP address/hostname if required, i.e.:

```
#!JavaScript

//Please Make sure that you update server.js:
	server.listen(app.get("port"),app.get("10.24.197.188"),
	function(){console.log("Express server listening on  IP: "+app.get("10.24.197.188")+" and port "+app.get("port"))

```


Please also update <strong>public/js/client.js</strong>:


```
#!JavaScript

var socket = io.connect("10.24.197.188:3000");
```

with the right IP address/hostname.

To install <code>**npm install && bower install**</code> and to launch run <code>**npm start**</code>.

## Terms of use:

1. Firstly Enter your Nice Name and click Join Button (Nice Name must be more than 3 letters).
2. ![screenshot-localhost 3000 2015-07-25 15-31-28.png](https://bitbucket.org/repo/KL7ezM/images/3780984539-screenshot-localhost%203000%202015-07-25%2015-31-28.png) Click on it to Create a new Room.
3. ![JoinImage.png](https://bitbucket.org/repo/KL7ezM/images/2184708970-JoinImage.png) Click on any already created Room.
4.  Only Owner can delete room.
5. **You can open [http://localhost:3000/](http://localhost:3000/) in different-different tabs to get real-time chat profile**.

## Suggestion

If your local Computer has dynamic IP, then you might have to change your IP again in **server.js** & **client.js**