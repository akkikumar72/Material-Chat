



## Setup and configuration
1. Make Sure you have IP address for Mac use : <strong>ipconfig getifaddr en0</strong> 

Replace: 
10.24.197.188 with your own IP.


Make sure that you update <strong>server.js</strong>:
and add your own IP address/hostname if required, i.e.:
<pre>server.listen(app.get('port'), "192.168.56.102", function(){
  console.log('Express server listening on port ' + app.get('port'));
});</pre>

(the port is defined in the <code>app.set('port', process.env.PORT || 3000);</code> section.)

Please also update <strong>public/js/client.js</strong>:
<pre>var socket = io.connect("10.24.197.188:3000");</pre>
with the right IP address/hostname.

To install <code>npm install && bower install</code> and to launch run <code>npm start</code>.

