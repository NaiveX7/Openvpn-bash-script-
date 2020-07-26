# Openvpn-bash-script-
automatic openvpn login

#!/usr/bin/expect -f

# automatic openvpn login
spawn sudo openvpn FILE.ovpn

# script will enter username/password automatic. 
expect "Enter Auth Username:" 
    send "USERNAME\n" 

expect "Enter Auth Password:" 
    send "PASSWORD\n"
    
interact

# end script
