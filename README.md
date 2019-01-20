# Python 2

Starter template for a Python 2 Docker application.

To start a new project using the template:
```
git clone git@github.com:dockerrecipes/python2.git my-python2-app
cd my-python2-app
docker build -t my-python2-app:1.0.0 .
docker run --rm my-python2-app:1.0.0
```

Or just copy the `Dockerfile` to your existing python project.

Put your python sources in the root of the project directory. Dependencies in `requirements.txt` are installed using [pip install](https://pip.pypa.io/en/stable/user_guide/). The docker image is configured to run `main.py`, but you can edit the `Dockerfile` to run whatever python script you want. You can provide command line arguments to the python script by adding them to the end of the `docker run` command, like so:

```
docker run --rm my-python2-app:1.0.0 arg1 arg2
```
