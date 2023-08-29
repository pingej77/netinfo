# netinfo
Bash script to provide network information in a  dense, legible, and useful way

Options:
    -a  show all online and offline interfaces and include DNS and DCHP information
    -u  include UUID
    -4  only show IPv4 addresses
    -6  include IPv6 addresses for gateway and DNS
    -A  show all (equivalent to -au6)
    -b  show a brief output

Dependencies:
    ip
    nmcli
    iw
    basic utils (bash, sed, awk, head, tail, etc.)
