# Target specification

* Input list of hosts/Networks from file
	* `-iL <fileName.txt>`
* Scan Random Hosts
	* `-iR <number>`
* Exclude host/Networks
	* `--exclude <host>`
* Exclude host/Networks from file
	* `--excludefile <hostFile.txt>`

# Host discovery

* List scan
	* `-sL`
* Ping scan
	* `-sn`
* Treat all hosts as online
	* `-Pn`
* Discovery to given ports: TCP SYN/ACK, UDP, SCTP
	* `-PS/PA/PU/PY <port list>`
* ICMP echo, timestamp, and netmask request discovery probes
	* `-PE/PP/PM`
* IP Protocol ping
	* `PO <protocol list>`
* DNS resolution: never/always (default: sometimes)
	* `-n/R`

# OS detection

* Enable OS detection
	`-O`
* Limit detection to promising targets
	* `--osscan-limit`
* Guess OS more aggressively
	* `--osscan-guess`

# Port specification and scan order

* Specify ports
	* `-p <port>,<port>,<...>/<1-65535>`
* Scan UDP ports
	* `-p U:<port>`
* Fast mode, scans few ports
	* `-F`
* Scan ports consecutively
	* `-r`
* Scan number of top ports
	* `--top-ports <number>`
* Scan ports more common than ratio given
	* `-port-ratio <number>`

# Service version detection

* Probe open ports to determine service/version info
	* `-sV`
* Version intensity
	* `--version-intensity <0-9>`
* Limit to most likely probes (intensity 2)
	* `--version-light`
* Try all probes (intensity 9)
	* `--version-all`
* Show scan activity
	* `--version-trace`

# Firewall / IDS evasion and spoofing
* Fragment IP packets (including ping scans). Can add offset size
	* `-f [--mtu <value>]`
* Cloak scanwith decoys
	* `-D <decoy>,<decoy>`
* Spoof source address
	* `-S`
* Use specified interface
	* `-e`
* Send packets with specified ip option
	* `--ip-options <option>`
* Set IP time to live field
	* `--ttl <value>`

# Script scan
* Script default
	* `-sC`
* Provide NSE script args in a file
	* `–script-args-file=<filename>`
* Show all data sent and received
	* `--script-trace`
* Show script help
	* `--script-help="<Lua scripts>"`
* Potential to crash servers / service
	* `--script-args=unsafe=1`

# Scanning techniques
* Xmas scan
	* `-sX`
* TCP SYN scan
	* `-sS`
* Connect scan
	* `-sT`
* ACK scan
	* `-sA`
* Window scan
	* `-sW`
* Maimon scan
	* `-sM`
* UDP scan
	* `-sU`
* TCP Null scan
	* `-sN`
* FIN scan
	* `-sF`
* SCTP INIT scan
	* `-sY`
* COOKIE-ECHO scan
	* `-sZ`
* IP protocol scan
	* `-sO`

# HTTP service information
* Gather page titles from HTTP services
	* `--script=http-title <host>`
* Get HTTP headers of web services
	* `--script=http-headers <host>`
* Find web apps from known paths
	* `--script=http-enum <host>`

# NMAP output options
* Output normal
	* `-oN`
* Output XML
	* `-oX`
* Output greppable
	* `-oG`
* Output all 3 formats
	* `-oA`
* Verbose
	* `-v`
* Debuggung
	* `-d/-dd`

# Script categories
* ALL
* AUTH
* DEFAULT
* DISCOVERY
* EXTERNAL
* INTRUSIVE
* MALWARE
* SAFE
* VULN, etc

# Timing and performance
* Serial, slowest
	* `-T0`
* Serial, slow
	* `-T1`
* Serial
	* `-T2`
* Parallel
	* `-T3`
* Parallel, fast
	* `-T4`

# Various TCP/IP protocols

## Application layer:
* FTP, HTTP, SNMP, BOOTP, DHCP
## Transport layer:
* TCP, UDP, ICMP, IGMP
## Network layer:
* ARP, IP, RARP
## Data link layer:
* SLIP, PPP