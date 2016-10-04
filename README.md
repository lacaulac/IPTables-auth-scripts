# IPTables-auth-scripts
A pack of 4 scripts, allowing sysadmins to easily let people access ports and revoking the accesses without having to directly mess with iptables
For example, in first place you block a specific port(with a REJECT or DROP instruction), and then you want to allow specific IPs to access it.
##Allowing someone to use a port
The command is: iptauth [IP] [Port]
##Revoking access to the port
The command is: iptdeauth [IP] [Port]
##Allowing the sysadmin itself to use the port
It adds the IP of the SSH client (assuming you're connected on the server by SSH) to the whitelist.

The command for allowing is: iptauthme [Port]

The command for revoking is: iptdeauthme [Port]



If you have any question, feel free to contact me at lacaulac@lacaulac.ndlx.io
