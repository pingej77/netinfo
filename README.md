# netinfo
Bash script to provide network information in a  dense, legible, and useful way. <br>
Lists MAC, IP addresses, network ID, and default gateway by default.  Includes DHCP and DNS information plus UUID with options.

<b>Options:</b>
<br>&emsp;-a &nbsp; show all online and offline interfaces and include DNS and DHCP information
<br>&emsp;-d &nbsp; show DNS and DHCP information without showing offline interfaces
<br>&emsp;-u &nbsp; include UUID
<br>&emsp;-4 &nbsp; only show IPv4 addresses
<br>&emsp;-6 &nbsp; include IPv6 addresses for gateway and DNS
<br>&emsp;-p &nbsp; find the public-facing IPv4 address (for use with NAT)
<br>&nemsp;-A &nbsp; show all (equivalent to -aup6)

<b>Dependencies:</b><br>
&emsp;ip <br>
&emsp;nmcli <br>
&emsp;iw <br>
&emsp;basic utils (bash, sed, awk, head, tail, etc.)

You can also search for specific interface names by passing it as an argument.  Search using wildcards as well to find certain types of interfaces.  Quotes necessary for zsh. <br>
Examples:<br>
&emsp; bash:  `netinfo wl*` <br>
&emsp; zsh:&nbsp;&nbsp;  `netinfo "wl*"`
