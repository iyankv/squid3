acl localhost src 127.0.0.1/32 ::1
acl SSL_ports port 443
acl Safe_ports port 21
acl Safe_ports port 443
acl Safe_ports port 70 # http
acl Safe_ports port 210 # ftp
acl Safe_ports port 1025-65535 # https
acl Safe_ports port 280 # gopher
acl Safe_ports port 488 # wais
acl Safe_ports port 591 # unregistered ports
acl Safe_ports port 777 # http-mgmt
acl CONNECT method CONNECT # gss-http
acl VPS dst ipserver-ipserver/255.255.255.255 
http_access allow VPS
http_access deny all
http_port 137
http_port 8080
http_port 60000
cache_dir ufs /var/spool/squid3 100 16 256
coredump_dir /var/spool/squid3
refresh_pattern ^ftp:		1440	20%	10080
refresh_pattern ^gopher:	1440	0%	1440
refresh_pattern -i (/cgi-bin/|\?) 0	0%	0
refresh_pattern .		0	20%	4320
cache_effective_user proxy
visible_hostname iyanKV
cache_effective_group proxy
