## Homework

_You will need to run 2 containers with Nginx._
_Both containers must have nginx page config files in volume._
(_Requirements:_*
	_first container = GREEN page background,_
	_second container = BLUE page background_

_Then you have to create service, which will point to both containers._

_Result:_
	_when we go to service endpoint, and refresh page periodicaly,_
	_we will get different background._
	
*!!!NOTE!!!*

_You should use you'r own docker registry for storing images._
### Deploy registry example: 
	![Setup Docker registry](/images/logo.png)
_Here is example of nginx configuration fail (located in /var/www/html, cald index*.html)_


### FOR GREEN BACKGROUND
```sh
<!DOCTYPE html>
<html>
<head>
<title>Welcome to nginx!</title>
<style>
    body {
        width: 35em;
        margin: 0 auto;
        font-family: Tahoma, Verdana, Arial, sans-serif;
        background: #7FFF00
    }
</style>
</head>
<body>
<h1>Welcome to nginx!</h1>
<p>If you see this page, the nginx web server is successfully installed and
working. Further configuration is required.</p>

<p>For online documentation and support please refer to
<a href="http://nginx.org/">nginx.org</a>.<br/>
Commercial support is available at
<a href="http://nginx.com/">nginx.com</a>.</p>

<p><em>Thank you for using nginx.</em></p>
</body>
</html>
```

### FOR BLUE BACKGROUND
```sh
<!DOCTYPE html>
<html>
<head>
<title>Welcome to nginx!</title>
<style>
    body {
        width: 35em;
        margin: 0 auto;
        font-family: Tahoma, Verdana, Arial, sans-serif;
        background: #0000FF
    }
</style>
</head>
<body>
<h1>Welcome to nginx!</h1>
<p>If you see this page, the nginx web server is successfully installed and
working. Further configuration is required.</p>

<p>For online documentation and support please refer to
<a href="http://nginx.org/">nginx.org</a>.<br/>
Commercial support is available at
<a href="http://nginx.com/">nginx.com</a>.</p>

<p><em>Thank you for using nginx.</em></p>
</body>
</html>
```