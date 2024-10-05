![image](https://github.com/user-attachments/assets/360aa27b-db0f-4442-9d55-a10363c5fd27)This Github repository holds the basic files needed for a TCP IP server or client written in Python. 
There is a lot of clean up that should be done for production quality applications, such as being certain to smoothly close all ports on exit, 
adding try and excepts for errors, system logging for tracking messaged data, and useful parsing of data to actually use. But this was a basic tutorial!



1.
 What is data encapsulation?

The process of adding extra information at each layer of the OSI model while information flows from one host to another.

2.
A company has a teleconferencing system that utilizes VOIP technology. 

This system uses UDP as the transport. 

What will happen if UDP datagrams arrive at their destination out of sequence?


UDP will pass the information in the datagrams up to the next layer in the order they arrived.  

3.

What is one purpose of the TCP three-way handshake?

Synchronizing between source and destination in preparation for data transfer.

4. 
 What is the purpose of a router in the network?


To interconnect networks and choose the best path between them.  

5. What is the difference between HTTP and HTTPs?
   
HTTPs uses encryption.

6.
 What is the meaning of the output MTU 1500 Bytes?  MTU - maximun transmission unit
 
The maximum packet size that can traverse this interface is 1500 bytes.  

7. 
 What is the purpose of a switch in the network?

To provide network attachment to the end systems and intelligent switching of the data within the local network.  

8.  Switch ‘leaf1’ needs to send a frame to a host with the following MAC address of 00b0.d056.efa4.

Based on the MAC address table shown here, what will switch ‘leaf1’ do with the frame?  


 Flood the frame out all of its ports.  

9.  Why will a switch never learn a broadcast address? 


 A broadcast frame is never forwarded by a switch.  

10.  Host A 向 Host B 发送初始帧时，交换机会做的第一件事是什么？
正确答案:

它会将地址 00:0b:db:95:2e
添加到MAC地址表。
解释:

当交换机接收到帧时，它首先会检查源MAC地址，并将其添加到MAC地址表中，这样以后可以更高效地转发数据帧到该源地址的设备。


第11题: 如何在第3层数据中心设计中实现多路径支持？
正确答案:

可以配置BGP和ECMP。
解释:

BGP（边界网关协议）是一种常用于数据中心的路由协议，它支持多路径（ECMP，等价多路径路由）。ECMP允许多个路径在路由表中拥有相同的成本，从而实现负载均衡和更高的冗余性。

第12题: 如何在第2层数据中心设计中实现多路径支持？
正确答案:

可以为每个VLAN组配置MSTP实例。
解释:

MSTP（多实例生成树协议）允许多个生成树实例在一个网络中运行，从而为不同的VLAN提供多路径支持。这在第2层网络中通过防止环路和支持不同路径来实现冗余和负载均衡。


第13题: BGP 作为数据中心协议受欢迎的原因是？（选择两个）
正确答案:

可扩展且稳定。
支持多路径。
解释:

BGP的可扩展性和稳定性使其成为大型网络环境中的首选。它通过支持多路径（ECMP）来提高网络的灵活性和效率，从而在数据中心环境中变得越来越流行。


第14题: 哪两个用于防止第2层网络中的环路？（选择两个）
正确答案:

MLAG
STP
解释:

MLAG（多链路聚合组）和STP（生成树协议）是第2层网络中常用的防止环路的技术。MLAG允许跨设备的链路聚合，而STP则通过阻止冗余链路中的部分链路来防止网络环路。


第15题: IP包中的生存时间（TTL）字段的目的是什么？
正确答案:

防止数据包无限循环。
解释:

TTL（生存时间）字段用于限制数据包在网络中的生存时间。每经过一个路由器，该字段的值就会减少1，当其值减为0时，数据包会被丢弃。这可以防止数据包在网络中无限循环，避免网络拥堵。
