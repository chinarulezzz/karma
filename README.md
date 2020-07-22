
<p align="center">
 <img alt="karma" src="https://i.imgur.com/C3zISlU.gif"/>
 <p align="center">
  <a href="https://github.com/chinarulezzz/karma/releases/latest">
   <img alt="Release" src="https://img.shields.io/github/tag/chinarulezzz/karma.svg">
  </a>
 </p>
</p>

---

##### About

This is the fork of the decoxvii's karma. )

The sources and the author's GitHub profile was removed.
So... I've adopted karma by the same name.

##### API: pwndb2am4tzkvold (dot) onion

Find leaked emails with your passwords.

---

#### Run without installation

Install runtime dependencies (Kali/Debian/Ubuntu):
```
sudo apt install tor python3 python3-socks python3-texttable python3-docopt python3-requests
git clone https://github.com/chinarulezzz/karma.git
sudo service tor start
./karma/bin/karma --help
```

#### Installation

Install dependencies (Debian/Ubuntu):
```
sudo apt install tor python3 python3-pip
```

Install with `pip3`:
```
sudo -H pip3 install git+https://github.com/chinarulezzz/karma.git
karma --help
```

---

#### Building from Source

Clone this repository, and:
```
git clone https://github.com/chinarulezzz/karma.git
cd karma
sudo -H pip3 install -r requirements.txt
python3 setup.py build
sudo python3 setup.py install
```

---

#### Update

To update this tool to the latest version, run:
```
sudo -H pip3 install git+https://github.com/chinarulezzz/karma.git --upgrade
karma --version
```

---

#### Usage

Start by printing the available actions by running `karma --help`.
It's also necessary to restart the **Tor** service `sudo service tor restart`.
Then you can perform the following tests:

1. Search emails with the password: `123456789`
```
karma search '123456789' --password -o test1
```

2. Search emails with the local-part: `johndoe`
```
karma search 'johndoe' --local-part -o test2
```

3. Search emails with the domain: `hotmail.com`
```
karma search 'hotmail.com' --domain -o test3
```

4. Search email password: `johndoe@unknown.com`
```
karma target 'johndoe@unknown.com' -o test4
```

---

#### Disclaimer

Usage this program for attacking targets without prior consent is illegal.
It's the end user's responsibility to obey all applicable local, state and
federal laws. Developers assume no liability and are not responsible for any
misuse or damage caused by this program.

---

#### Thanks

The original author:
+ Sergio SA (decoxviii)

This program is inspired by the projects:
+ [pwndb_api](https://github.com/M3l0nPan/pwndb_api) by: M3l0nPan
+ [pwndb](https://github.com/davidtavarez/pwndb)     by: davidtavarez

---

© Sergio SA (decoxviii)

**[MIT](https://github.com/chinarulezzz/karma/blob/master/LICENSE)**
