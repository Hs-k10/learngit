# SDN密网
　　我们的系统由五个主要组件组成，一个 SDN 控制器负责动态生成和管理流规则以引导和控制网络流量，一个欺骗服务器来操纵网络流量并考虑特定用户策略模拟某些虚拟网络资源，一个蜜罐服务器模拟虚拟蜜罐节点，虚拟网络视图生成器，提供虚拟网络组件及其连接性和流量排队的描述，以控制链路延迟和带宽。  
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;实验环境是基于ubuntu系统、并部署SDN网络模拟器mininet，SDN控制器POX、SDNCtroller组件、DecepServertion欺骗服务器、honeyd蜜罐服务器、nv虚假配置文件生成器ViewGenerator。
#### 需用户自行部署环境
##### SDN网络模拟器mininet    
     sudo apt-getinstall git   #更新git
     git clone git://github.com/mininet/mininet  #下载软件包
     cd mininet
     sudo git check out 2.2.1  #选择版本
     sudo  ./util/install.sh  -nfv  #安装Mininet、基于OpenFlow的交换机和Open vSwitch
     mn --version   #测试 
     (详细可参考：https://blog.csdn.net/linyixiao88/article/details/65651390?utm_source=debugrun&utm_medium=referral )
##### POX控制器   
    git clone git://github.com/noxrepo/pox
    cd pox
    git checkout carp
    ./pox.py
    
  
  
