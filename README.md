Osmedeus
============
Automatic Reconnaisance and Scanning in Penetration Testing

# What is Osmedeus?
Osmedeus allow you to doing boring stuff in Pentesting automatically like reconnaissance and scanning the target by run the collection of awesome tools.

# Installation
```
git clone https://github.com/j3ssie/Osmedeus
cd Osmedeus
chmod +x install.sh
./install.sh
```

# How to use

* Doing normal routine include: Subdomain Scanning, Subdomain TakeOver Scanning, Port Scanning and ScreenShot the target.
```
./osmedeus.py -t example.com
```

* Scanning subdomain and Subdomain TakeOver
```
./osmedeus.py -m subdomain -t example.com
```

* Screenshot the list of domain and do Port Scan on it
```
./osmedeus.py -m portscan -t example.com
```

* Doing blind directory search on the target 
```
./osmedeus.py -m dirbrute -t example.com
```


* Doing brute force on the service result from scanning service
```
./osmedeus.py -m brute -t example.com
```


* Git repo scanning
```
./osmedeus.py -m git --git https://github.com/whatever/repo
```

* Doing some stuff with Burp State file
```
./osmedeus.py -m burp -t example.com --burp yourburpstate.xml
```


* List all module 
```
./osmedeus.py -M
```

* Update 
```
./osmedeus.py --update
```




# Available modules with list tool being used
* Subdomain Scanning
  * [amass](https://github.com/caffix/amass)
  * [subfinder](https://github.com/subfinder/subfinder)
  * [massdns](https://github.com/blechschmidt/massdns)

* Subdomain TakeOver Scanning
  * [subjack](https://github.com/haccer/subjack)
  * [SubOver](https://github.com/Ice3man543/SubOver)

* IP Discovery
  * [IPOsint](https://github.com/j3ssie/IPOsint)

* Port Scanning and ScreenShot the target
  * [aquaton](https://github.com/michenriksen/aquatone)
  * [EyeWitness](https://github.com/FortyNorthSecurity/EyeWitness)
  * [masscan](https://github.com/robertdavidgraham/masscan)

* Git repo scanning
  * [truffleHog](https://github.com/dxa4481/truffleHog)
  * [gitrob](https://github.com/michenriksen/gitrob)

* Doing some stuff with Burp State file
  * [sqlmap](https://github.com/sqlmapproject/sqlmap)
  * [SleuthQL](https://github.com/RhinoSecurityLabs/SleuthQL)
  * [LinkFinder](https://github.com/GerbenJavado/LinkFinder)

* Directory search
  * [dirhunt](https://github.com/Nekmo/dirhunt)
  * [dirsearch](https://github.com/maurosoria/dirsearch)
  * [gobuster](https://github.com/OJ/gobuster)

* Bruteforce services
  * [brutespray](https://github.com/x90skysn3k/brutespray)

* Wordlists
  * [domain](https://gist.githubusercontent.com/jhaddix/86a06c5dc309d08580a018c66354a056/raw/96f4e51d96b2203f19f6381c8c545b278eaa0837/all.txt)
  * [web-content](https://gist.githubusercontent.com/jhaddix/b80ea67d85c13206125806f0828f4d10/raw/c81a34fe84731430741e0463eb6076129c20c4c0/content_discovery_all.txt)

# Contribute
This is just beta version if you have any problem or an idea, feel free to create an issue or contact me.

# Demo
[![asciicast](https://asciinema.org/a/ZudWoY9mRbXaqmYqHwB6Ky6lm.svg)](https://asciinema.org/a/ZudWoY9mRbXaqmYqHwB6Ky6lm)

[![Osmedeus](https://img.youtube.com/vi/SnGPedyJvig/0.jpg)](https://www.youtube.com/watch?v=SnGPedyJvig)

# Disclaimer
Most of this tool done by the authors of the tool that you can see in the module folder.
I just put all the pieces together, plus some extra boring stuff that we don't wanna do everyday.

This tool is for educational purposes only. You are responsible for your own actions. If you mess something up or break any laws while using this software, it's your fault, and your fault only.


# Contact
[@j3ssiejjj](https://twitter.com/j3ssiejjj)