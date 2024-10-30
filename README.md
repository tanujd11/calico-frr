apt-get update -y
apt update -y
apt-get install -y vim iputils-ping net-tools
apt install -y python3-pip frr frr-pythontools
pip install docker-systemctl-replacement
sysctl -w net.ipv4.ip_forward=1

$ # Update the file /etc/frr/daemons

/usr/local/bin/systemctl.py start frr
vtysh
