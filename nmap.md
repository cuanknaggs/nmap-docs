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