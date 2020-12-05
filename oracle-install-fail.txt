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

# https://docs.oracle.com/en/database/oracle/oracle-database/18/ladbi/running-rpm-packages-to-install-oracle-database.html#GUID-BB7C11E3-D385-4A2F-9EAF-75F4F0AACF02

# Download oracle-database-xe-18c-1.0-1.x86_64.rpm
curl -o oracle-database-preinstall-18c-1.0-1.el7.x86_64.rpm https://yum.oracle.com/repo/OracleLinux/OL7/latest/x86_64/getPackage/oracle-database-preinstall-18c-1.0-1.el7.x86_64.rpm

# Run 
yum install -y oracle-database-preinstall-18c # 안됨
yum -y localinstall oracle-database*18c*

# 위치 다름 
# Run “/etc/init.d/oracle-xe-18c configure”


/etc/sysconfig/oracle-database-preinstall-18c







출처: https://hwoarang757.tistory.com/entry/CentOS-7-Oracle-18c-Express-설치-진행 [허접한 실력에 형편없는 개발자의 블로그]

curl -o oracle-database-preinstall-18c-1.0-1.el7.x86_64.rpm https://yum.oracle.com/repo/OracleLinux/OL7/latest/x86_64/getPackage/oracle-database-preinstall-18c-1.0-1.el7.x86_64.rpm

# yum -y localinstall oracle-database-preinstall-18c-1.0-1.el7.x86_64.rpm

# 없음
# yum -y localinstall oracle-database-xe-18c-1.0-1.x86_64.rpm

# 안됨
/etc/init.d/oracle-database-preinstall-18c-firstboot configure
/etc/init.d/oracle-database-preinstall-18c-firstboot start



curl https://download.oracle.com/otn-pub/otn_software/db-express/oracle-database-xe-18c-1.0-1.x86_64.rpm

curl -o oracle-database-preinstall-18c-1.0-1.el7.x86_64.rpm https://yum.oracle.com/repo/OracleLinux/OL7/latest/x86_64/getPackage/oracle-database-preinstall-18c-1.0-1.el7.x86_64.rpm
yum -y localinstall oracle-database-preinstall-18c-1.0-1.el7.x86_64.rpm
# cd /tmp
# yum -y localinstall oracle-database-ee-18c-1.0-1.x86_64.rpm
# /etc/init.d/oracledb_ORCLCDB-18c configure

