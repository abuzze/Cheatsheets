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

Mobile Backups on Macbook Pro

	On a MPB with Lion or Mountain Lion the mobile Backups 
	under /Volumes/MobileBackups can consume a lot of space.
	You can confirm this by looking into the Storage tab via about
	my mac. This backup is matched against a time maschine backup, but there is no switch in the sys prefs to disable it. But you can via terminal. Reboot afterwards and the mobile backups are gone.

	sudo tmutil disablelocal