# SEARCHDOX

SEARCHDOX is an advanced open-source intelligence and digital reconnaissance tool developed in Python to map digital footprints and validate username permutations across multiple platforms in real time, featuring a clean CLI reporting environment for Termux and Kali Linux. The system operates by deconstructing the input query, normalizing strings to remove regional characters or spaces, generating a heuristic matrix of potential username variations, and performing parallel live validations via HTTP connection checks and passive DNS resolution vectors to aggregate profile data, network nodes, and connected infrastructure records.

![SEARCHDOX Interface](https://i.postimg.cc/63fbjM48/Novo-projeto-542-E8EAD33.png)

## Termux Deployment

$ pkg update && pkg upgrade -y
$ pkg install git python ndk-sysroot clang make libxml2 libxslt -y
$ git clone https://github.com/mrmaestrox156-debug/SEARCHDOX.git
$ cd SEARCHDOX
$ pip install colorama requests beautifulsoup4 dnspython
$ python searchdox.py

## Kali Linux Deployment

$ sudo apt update && sudo apt upgrade -y
$ sudo apt install git python3 python3-pip -y
$ git clone https://github.com/mrmaestrox156-debug/SEARCHDOX.git
$ cd SEARCHDOX
$ pip3 install colorama requests beautifulsoup4 dnspython
$ python3 searchdox.py

## Technical Requirements

The tool deployment requires functional installations of git and python package managers to pull down the dynamic source folder and resolve core components including colorama for terminal interface rendering, requests for platform queries, beautifulsoup4 for parsing logic, and dnspython for infrastructure mapping operations.
