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