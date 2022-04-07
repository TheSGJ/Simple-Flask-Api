## Steps required for configuring the project.
> Clone the repository using the git bash :
```bash
git clone https://github.com/TheSGJ/Simple-Flask-Api.git
```
> Move to the project directory :
```bash
cd Simple-Flask-Api

```

> Create a virtual environment :
```bash
# Let's install virtualenv first
pip install virtualenv

# if you want isolate your project then you can create virtual environment to run your flask app separately. (Optional)
virtualenv env

```

> Activate the virtual environment :
```bash
env\scripts\activate

```

> Install the requirements or install flask directly using pip install flask :
```bash
pip install -r requirements.txt

```



### Running the Flask App:

--> To run the App, we use :
```bash
flask run

```

> Then, the development server will be started at http://127.0.0.1:5000/
## Get Request using the Http Client:
![Get Request](https://cdn.jsdelivr.net/gh/thesgj/Simple-Flask-Api/img/GetR_ApiClient.jpg)
### About Flask:
Flask is a minimal Python framework that helps you create a web server. 

Let's take a look at the example code we have:

```python
from flask import Flask

app = Flask(__name__)

@app.route("/")
def hello_world():
    return "<h1>Hello, World!</h1>"
```
	
What did that code do?

First we `import` the `Flask` class. An instance of this class will be our WSGI application.

Next we create an instance of this class. The first argument is the name of the application’s module or package. `__name__` is a convenient shortcut for this that is appropriate for most cases. This is needed so that Flask knows where to look for resources such as templates and static files.

We then use the `route()` decorator to tell Flask what URL should trigger our function. In this case we use `/` routh, which is the default route of any website.

The function returns the message we want to display in the user’s browser. The default content type is HTML, so HTML in the string will be rendered by the browser.

To learn more, checkout the [official guide](https://flask.palletsprojects.com/en/2.0.x/quickstart/).

# License

[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)

