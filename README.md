# granscan
A simplified way to run various Linux diagnostic tools

### N.B - I am re-writing this in Golang so the readme is not up to date at the moment.

```
Usage: granscan [OPTION] [COMMAND]

A simplified way to run various Linux diagnostic tools

Options:
  -h        Print usage
  -a        Run all diagnostic tools

Commands:
  help      Print usage
  check     Check what tools can be run and what missing tools can be installed
  cpu       Run CPU diagnostic tools
  memory    Run memory diagnostic tools
  network   Run network diagnostic tools
  storage   Run storage diagnostic tools
  info      Get various information about the current system
  all       Run cpu, memory, network and storage diagnostic tools
```

# Usage
```
git clone https://github.com/adampie/granscan
cd granscan && chmod +x granscan.sh
./granscan.sh
```
or
```
wget https://raw.githubusercontent.com/adampie/granscan/master/granscan.sh
chmod +x granscan.sh && sudo mv granscan.sh /usr/bin/granscan
granscan
```

## List of tools used
- top
- ps
- free
- vmstat
- ip
- ifconfig
- netstat
- ss
- nicstat
- df
- lsblk
- lsof
- uptime
- w
- lscpu
- lshw
- lsscsi
- lsusb

# Contributing
Feel free to contribute, submit a pull request or open an Issue.

# License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

# Acknowledgments
Brendan Gregg - http://www.brendangregg.com/linuxperf.html
