# tcpfastopen

To check if mininet is correctly installed and to debug the host connectivity,

ubuntu@ip-172-31-31-175:~/project-copy/master$ sudo mn
*** Creating network
*** Adding controller
*** Adding hosts:
h1 h2
*** Adding switches:
s1
*** Adding links:
(h1, s1) (h2, s1)
*** Configuring hosts
h1 h2
*** Starting controller
c0
*** Starting 1 switches
s1 ...
*** Starting CLI:
mininet>
mininet>
mininet> ping 10.0.0.1
*** Unknown command: ping 10.0.0.1
mininet> h1
*** Please enter a command for node: h1 <cmd>
mininet> h1 ping 10.0.0.1
PING 10.0.0.1 (10.0.0.1) 56(84) bytes of data.
64 bytes from 10.0.0.1: icmp_seq=1 ttl=64 time=0.035 ms
64 bytes from 10.0.0.1: icmp_seq=2 ttl=64 time=0.050 ms
64 bytes from 10.0.0.1: icmp_seq=3 ttl=64 time=0.051 ms
^C
--- 10.0.0.1 ping statistics ---
3 packets transmitted, 3 received, 0% packet loss, time 2055ms
rtt min/avg/max/mdev = 0.035/0.045/0.051/0.007 ms
mininet> h1 ping 10.0.0.2
PING 10.0.0.2 (10.0.0.2) 56(84) bytes of data.
64 bytes from 10.0.0.2: icmp_seq=1 ttl=64 time=2.04 ms
64 bytes from 10.0.0.2: icmp_seq=2 ttl=64 time=0.331 ms
^C
--- 10.0.0.2 ping statistics ---
2 packets transmitted, 2 received, 0% packet loss, time 1001ms
rtt min/avg/max/mdev = 0.331/1.183/2.036/0.852 ms
mininet>
