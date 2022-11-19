### PwnedOrNot (https://github.com/thewhiteh4t/pwnedOrNot)
Installation:
```
Must make a payment to get a haveibeenpwned API key
Obtain an API Key: https://haveibeenpwned.com/API/Key
haveibeenpwned API v3 Documentation: https://haveibeenpwned.com/API/v3

git clone https://github.com/thewhiteh4t/pwnedOrNot.git
cd pwnedOrNot
chmod +x install.sh
./install.sh
```

Using pwnedornot:
Checking for a Single Email
- python3 pwnedornot.py -e <email>
- python3 pwnedornot.py --email <email>

Check Multiple Emails from File
- python3 pwnedornot.py -f <file name>
- python3 pwnedornot.py --file <file name>

Filter Result for a Domain Name [Ex : adobe.com]
- python3 pwnedornot.py -e <email> -d <domain name>
- python3 pwnedornot.py -f <file name> --domain <domain name>

Get only Breach Info, Skip Password Dumps
- python3 pwnedornot.py -e <email> -n
- python3 pwnedornot.py -f <file name> --nodumps

Get List of all Breached Domains
-python3 pwnedornot.py -l
- python3 pwnedornot.py --list

Check if a Domain is Pwned
- python3 pwnedornot.py -c <domain name>
- python3 pwnedornot.py --check <domain name>

### pwned (https://github.com/wKovacs64/pwned)

Installation:
```
Kali Linux:
apt install nodejs
apt install npm
npm install pwned -g
```

Using Pwned: 
Adding your haveibeenpwned API key
- pwned apikey <key>
Obtain all breaches for an account
- pwned ba <account|email>
