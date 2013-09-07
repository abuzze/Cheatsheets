### speed up cifs/smb
	
	sudo sysctl -w net.inet.tcp.delayed_ack=0

change in
	
	/etc/sysctl.conf


### netzwerkverkehr sniffen

alles auf der Netzwerkkarte

	sudo tcpdump -n -i en0

### DNS Cache löschen

Mac OS X Lion, Mountain Lion (10.7, 10.8)

	sudo killall -HUP mDNSResponder

Mac OS X Leopard, Snow Leopard (10.5, 10.6)

	sudo dscacheutil -flushcache