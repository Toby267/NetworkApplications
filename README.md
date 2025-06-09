# NetworkApplications

## Usefull commands

### To get help
```
To display usage/help information type:
python3 NetworkApplication.py -h
```

### To send ping and traceroutes
```
sudo python3 NetworkApplications.py ping goole.com
sudo python3 NetworkApplications.py traceroute -p udp google.com
sudo python3 NetworkApplications.py traceroute -p icmp google.com
sudo python3 NetworkApplications.py mtroute -p udp google.com
sudo python3 NetworkApplications.py mtroute -p icmp google.com
```

### To use a web server
```
sudo python3 NetworkApplications.py web -p 8080
Then go to 127.0.0.1:8080/index.html on a browser
```

### To use a web proxy
```
sudo python3 NetworkApplications.py proxy -p 8080
export http_proxy=http://127.0.0.1:8080
wget http://neverssl.com
Then check the 'cache' directory that has been created

or:
sudo python3 NetworkApplications.py proxy -p 8080
curl neverssl.com --proxy 127.0.0.1:8000
Then check the 'cache' directory that has been created
```
