# Install-Drozer-on-Mac

```
$ mkdir drozer
$ wget https://github.com/FSecureLABS/drozer/releases/download/2.4.4/drozer-2.4.4-py2-none-any.whl

# Create virtual environment with pipenv and install required dependencies.
$ pipenv --python 2.7
$ pipenv shell

(drozer) $ pipenv install protobuf
(drozer) $ pipenv install pyOpenSSL
(drozer) $ pipenv install Twisted
(drozer) $ pipenv install drozer-2.4.4-py2-none-any.whl
```
