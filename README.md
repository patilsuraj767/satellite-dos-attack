# Satellite-dos-attack

satellite-dos-attack is the ruby program developed to trigger the http requests and register the fake servers to the satellite. Http requests are triggered in asynchronous fashion so that it creates the load on the satellite and passenger request queue bumps up. Using this you can test the performance of the satellite server.

Note - Not recommended to use this on production systems.


## Installation

To run the satellite-dos-attack ruby package and httpclient gem is needed. 

```bash
# yum install ruby -y
# gem install httpclient
# git clone https://github.com/patilsuraj767/satellite-dos-attack.git
```

## Usage

```
./satellite-dos-attack -s satellite.example.com -p mypasseord -n 50
```
```
$ ./satellite-dos-attack --help
Usage: ./satellite-dos-attack [options]
    -s, --satellite hostname         Hostname or IP address of satellite server
    -p, --password password          Admin Password of satellite server
    -n, --numberofhosts hosts        Number of fake hosts to register to the satellite server

```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.



