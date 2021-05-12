# Install-Drozer-on-Mac

```
# Download the wheel from FSecureLABS drozer repo
$ mkdir drozer
$ wget https://github.com/FSecureLABS/drozer/releases/download/2.4.4/drozer-2.4.4-py2-none-any.whl

# Create virtual environment with pipenv and install required dependencies.
$ pipenv --python 2.7
$ pipenv shell

# Install the dependencies
(drozer) $ pipenv install protobuf
(drozer) $ pipenv install pyOpenSSL
(drozer) $ pipenv install Twisted
(drozer) $ pipenv install drozer-2.4.4-py2-none-any.whl

# Check out the available tools
(drozer) bash-3.2$ drozer console --help
usage: drozer console [OPTIONS] COMMAND

Starts a new drozer Console to interact with an Agent.

The drozer Console connects to an Agent and allows you to interact with the
system from the context of the agent application on the device. The console
can connect directly to an agent, if its embedded server is enabled, or through
a drozer Server that the agent is connected to.

positional arguments:
  command               the command to execute
  device                the unique identifier of the Agent to connect to

optional arguments:
  -h, --help            show this help message and exit
  --server HOST[:PORT]  specify the address and port of the drozer server
  --ssl                 connect with SSL
  --accept-certificate  accept any SSL certificate with a valid trust chain
  --debug               enable debug mode
  --no-color            disable syntax highlighting in drozer output
  --password            the agent requires a password
  -c ONECMD, --command ONECMD
                        specify a single command to run in the session
  -f [FILE [FILE ...]], --file [FILE [FILE ...]]
                        source file

available commands:
  commands    shows a list of all console commands                                                                                                     
  connect     starts a new session with a device                                                                                                       
  devices     lists all devices bound to the drozer server                                                                                             
  disconnect  disconnects a drozer session                                                                                                             
  version     display the installed drozer version 
```
