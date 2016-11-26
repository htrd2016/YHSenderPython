# YHSenderPython
#username password cisco_ip ip_to_ping zabbix_server_ip zb_host_name
nohup python ./pingByTelnetSwitch.py test test 100.168.103.230 192.168.103.51 192.168.103.112 "cisco switch WS-C3750X-48" > /dev/null 2> pingByTelnetSwitch.log &

nohup python ./pingBySSHRouter.py test test 100.195.96.254 192.168.103.51 192.168.103.112 "cisco router" > /dev/null 2> pingBySSHRouter.log &


#前置机使用
nohup python ./sendSessionNumber.py > /dev/null 2> sendSessionNumber.log &
