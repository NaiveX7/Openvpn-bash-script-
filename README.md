# Openvpn-bash-script-
automatic openvpn login

#!/usr/bin/expect -f

spawn sudo openvpn FILE.ovpn

expect "Enter Auth Username:" 
    send "USERNAME\n" 

expect "Enter Auth Password:" 
    send "PASSWORD\n"
    
interact
