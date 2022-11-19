# Setup and Initialization:

## In Kali Linux
```
# Commands to Install tor and the tor browser
sudo apt install tor
sudo apt install tor-browser

# Running the tor browser
Command Line: Open the terminal and type tor-browser

A new window will appear loading the tor browser
```

Configuring

## Browsers: 
Brave: https://brave.com/
I2P: https://geti2p.net/en/ 
Tor Broswer: https://www.torproject.org
Whonix: https://www.whonix.org/
Zeronet: https://zeronet.io/


# Dark Web Scanners:

Katana: https://github.com/TebbaaX/Katana

Installation: 
```
git clone https://github.com/TebbaaX/Katana
cd Katana
python3 -m pip install -r requirements.txt
python3 kds.py
```

Onion Search: https://github.com/megadose/OnionSearch
 ```
git clone https://github.com/megadose/OnionSearch
cd onionseach
python3 setup.py install
onionsearch
```

Darkdump: https://github.com/josh0xA/darkdump
Note: Darksearch.io now forbids public queries so this tool may not work

```
git clone https://github.com/josh0xA/darkdump
cd darkdump
python3 -m pip install -r requirements.txt
python3 darkdump.py --help
```

# Other tools to crawl the TOR network
- https://github.com/DedSecInside/TorBot

# Commands to verify if onion links are active:
Note: You will needed to be connected or proxied into the tor network to check if the site.
nmap:
```
nmap -sT -PN -n -p 80,443 facebookcorewwwi.onion

proxychains4 -f /etc/proxychains.conf /usr/bin/nmap -sT -PN -n -p 80,443 facebookcorewwwi.onion
```
curl:
```
curl -I https://facebookcorewwwi.onion
```
netcat (nc):
```
nc -z 80 facebookcorewwwi.onion
nc -z 443 facebookcorewwwi.onion
```

# Resources: 
Installing Tor on Kali Linux: https://www.kali.org/docs/tools/tor/
