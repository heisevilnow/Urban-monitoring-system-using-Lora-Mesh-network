# Urban-monitoring-system-using-Lora-Mesh-network
This system includes 4 Slave(using Arduino Nano) and 1 Master(using ESP8266)
About Master:
- It will send connection request to Slave and then waiting respond from Slave.
- After receiving the respond of Slave. It will store address of Slave to communicate.
About all Slave, it will wait the request from Master. After receiving request, it will collect enviromental value then it will calculate and send that data to Master. 
- Those Slaves will scan to other Slaves which didn't come to connect with the Master and wait to receive data from it.
- After that, it will send that data to Master(this is the intermediate Slave, it can send data of other Slave to the Master).
