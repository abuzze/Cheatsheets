##Windows Cheatsheet

To enable Remote Desktop remotely by using the registry

On any computer that is running a version of Windows Server 2003 or Windows XP Professional, click Start, click Run, type regedit, and then click OK.
On the File menu, click Connect Network Registry.
In the Select Computer dialog box, type the computer name and then click Check Names.
In the Enter Network Password dialog box, provide Domain Admins credentials for the domain of the server, and then click OK.
After the computer name resolves, click OK.

In the computer node that appears in the Registry Editor, navigate to HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Terminal Server.
In the console tree, click Terminal Server and then, in the details pane, double-click fDenyTSConnections.
In the Edit DWORD Value box, in Value data, type 0, and then click OK.

To implement the change, reboot the server remotely, as follows:
Open a command prompt, type the following, and then press Enter:
	shutdown -m \\ DomainControllerName -r