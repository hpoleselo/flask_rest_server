# flask_rest_server
Small example of a REST server implemented in Python.

Name the main application as `app.py`or `main.py`. 

## Auto-reload when developing in Flask

Instead of setting env variables manually, we create a `.flaskenv` with the following content:
```
DEBUG=true
FLASK_APP=app
FLASK_ENV=development
```

When you run `$ flask run` it will automatically use `load-dotenv` to load `.flaskenv`, for that we must:

`$ pip install python-dotenv`

Set environment variables to enable auto-reload: (Windows)

```
$ setx FLASK_APP main.py
$ setx FLASK_ENV development
```

To see changes:

` $ gci env:*`

To run:
`$ flask run --debugger`

se nao der certo, $env:FLASK_APP = "main.py" ou set FLASK_APP = run.py
