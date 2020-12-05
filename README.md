# CentOS7

# 7에선 사용 불가
ifconfig

# 
ip addr

# 
shutdown -s 0
shutdown -r 0

# 네트워크 설정
ll /etc/sysconfig/network-scripts//ifcfg-*
vi /etc/sysconfig/network-scripts//ifcfg-eth0

# 네트워크 자동 설정 원할시
# ONBOOT=no 를 yes 로 변경
