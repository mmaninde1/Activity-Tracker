# Activity Tracker

This Web app is an activity tracker. It allows you to track time that you spend on some activities.<br/>
You can create, edit and delete category.<br/>
Then you can create activity and choose below details:<br/>
-> Name<br/>
-> Date<br/>
-> Description<br/>
-> Time <br/>
-> Category (If any)<br/>
<br/>
You can create, edit and delete activity also.<br/>
You can Signup and Login.<br/>
<br/>
You can use it for your own purpose and you can take any functionality from it.<br/>

# Example PHP Docker project

Do not use in production.

This is a simple project to make you development with PHP simpler.

## License - MIT License

Copyright 2020 Alexandre Quessy

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.


## How to use

```
docker-compose up -d --build
```

Go to http://localhost:8883

If you deploy this on a server, make sure to change the port of the web service, if more than one project uses
this boilerplate. You must edit the docker-compose.yml to do so. See the documentation for Docker Compose.

You should change the environment variables in the docker-compose.yml
One thing that is really important, is that if you write some client-side JavaScript code, either to GET HTTP
requests using a relative path, or use the full domain name for the server where it's installed.
Hence, when you deploy it to a server, **you should change the value of CONFIG_BACKEND_HOST to match the IP address**
of your server.

Happily, you can simply edit the files under www, and the changes will be reflected in your application.

This docker-compose.yml file also provides some SQL management tools. Note that they are quite unsecure, since
the password for your MySQL user are exposed in cleartext in the docker-compose.yml, and anyone can then change
the contents of your database easily.

Do not use as is in production! 
