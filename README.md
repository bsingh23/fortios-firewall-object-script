# fortios-firewall-object-script

Fortinet firewall object script

It's a common requirement these days to allow or deny cloud services based on their IP-Address list provided by vendor. 
But many time published list from Vendors for e.g. Microsoft is quite long and adding the address manually to the firewall is a  tedious task.
This script will take input of IP-Address from users and will creates the necessary Fortigate commands.

Script will take the filename (list which conatins IP-Address) from user and will generate a new file that will contain the Fortigate commands.
for e.g.

python3 fortinet_firewall_address.py

Enter the name of file to open: ms_exchange_online

output -> ms_exchange_online_2020-12-28T15\:55\:55.txt

Update script fortinet_firewall_address.py
1. Added error handling to check for correct filename
2. Added error handling to check for correct IP address or IP-Network's
3. Remove whitespaces from IP-Address file
