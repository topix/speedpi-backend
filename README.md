SpeedPi-Backend
==============

**Gateway**
We use [MicroServiceBus.com](https://microservicebus.com) to deploy and manage nodes in our network. It provides us with the framework to focus on deployment and data analysis. Data collections is fairly simple and one way, that way the focus can be put to analysis rather than maintenance.


----------


**Data storage**
We chose to use MySQL to store our data for later analysis. The reason is for quick deployment. All the data 


----------


**Data analysis**
We plan to use TensorFlow to analyze the health of all the factors over time. We aim to get all the data collected down to one single value that can be compared to other ISP's, other nodes or areas.

Datapoints for health:

 - WAN speed to specified hosts ([Ookla](http://www.speedtest.net/sv/))
 - Latency ([ICMP](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol)) - Measured from simple Ping and later with more 
 - Trace route ([ICMP](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol)) - Count amount of hop measure time between hops and create a global map of hops to triangulate location.
 - Packetloss when using ping or traceroute
 - Jitter - Collected from Ping or Traceroute

Plans:
We plan to analyse the quality drop off from watching Netflix and YouTube. The intention is to know if either the ISP might throttle or that the area has to bad uplink.