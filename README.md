# netinfo
Bash script to provide network information in a  dense, legible, and useful way. <br>
Lists MAC, IP addresses, network ID, and default gateway by default.  Includes DHCP and DNS information with options.

<b>Options:</b>
    <br>-a  show all online and offline interfaces and include DNS and DCHP information
    <br>-u  include UUID
    <br>-4  only show IPv4 addresses
    <br>-6  include IPv6 addresses for gateway and DNS
    <br>-A  show all (equivalent to -au6)
    <br>-b  show a brief output
    

<b>Dependencies:</b><br>
    * ip <br>
    * nmcli <br>
    * iw <br>
    * basic utils (bash, sed, awk, head, tail, etc.)
