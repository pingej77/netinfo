# netinfo
Bash script to provide network information in a  dense, legible, and useful way. <br>
Lists MAC, IP addresses, network ID, and default gateway by default.  Includes DHCP and DNS information plus UUID with options.

<b>Options:</b>
<br>&nbsp;&nbsp;-a &nbsp; show all online and offline interfaces and include DNS and DHCP information
<br>&nbsp;&nbsp;-d &nbsp; show DNS and DHCP information without showing offline interfaces
<br>&nbsp;&nbsp;-u &nbsp; include UUID
<br>&nbsp;&nbsp;-4 &nbsp; only show IPv4 addresses
<br>&nbsp;&nbsp;-6 &nbsp; include IPv6 addresses for gateway and DNS
<br>&nbsp;&nbsp;-p &nbsp; find the public-facing IPv4 address (for use with NAT)
<br>&nbsp;&nbsp;-A &nbsp; show all (equivalent to -aup6)

<b>Dependencies:</b><br>
&nbsp;&nbsp;ip <br>
&nbsp;&nbsp;nmcli <br>
&nbsp;&nbsp;iw <br>
&nbsp;&nbsp;basic utils (bash, sed, awk, head, tail, etc.)

You can also search for specific interface names by passing it as an argument.  Search using wildcards as well to find certain types of interfaces.  Quotes necessary for zsh. <br>
Examples:<br>
&emsp; bash:  `netinfo wl*` <br>
&emsp; zsh:&nbsp;&nbsp;  `netinfo "wl*"`
