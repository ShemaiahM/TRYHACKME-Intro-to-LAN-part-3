# TRYHACKME-Intro-to-LAN-part-3

# TryHackMe Room: Intro to LAN
### Technologies and designs that power private Networks.

Since the inception of the internet (WWW/World Wide Web), there has been consistent testing, trying and implementation of network designs. In regards to networking when the term topology is used, it used to reference the design and look of the network at hand.

---

## Ring Topology


<img width="205" height="196" alt="Ring_Topology" src="https://github.com/user-attachments/assets/ebfad695-9755-44d8-8cc7-117d72b4ced8" />



Ring topologies are formed using a network of devices like computers that are connected directly to each other, connected through the means of cables, forming a loop.

Ring Topology works by sending data around the loop of connected devices until it gets to the intended device. One interesting detail of ring topologies they often use a mechanism called token passing; a device will only transmit its own data if it currently holds the token. If it receives data meant for another device it will pass it along. If it has no data to send it will pass the token to the next device in the ring topology.

### Advantages
* **Troubleshoot:** because the data only has one way to travel, if data is not reaching a device, we can investigate with ease what device or cabling is at fault. Although this can be a double-edged sword, because it can take time to figure out which device has failed or is at fault in larger ring topology networks.
* **Less prone to Bottleneck:** Less prone to bottlenecks, because data is transferred bit by bit and not managed by one device or cable or travelling across the network all at once, like the Star topology or Bus topology. Yet this can be a double-edged sword.
* **No Central Node:** Unlike the Star topology, it doesn’t rely on a hub or switch to keep devices talking to one another.

### Disadvantages
* **Inefficient data transfer:** Can be time consuming, data has to go through each device to get to the destined device.
* **Contamination of data:** Data can be contaminated affecting the CIA triad pillars of Integrity & Confidentiality of data and access to data; if a device is compromised then data can be stolen or altered.
* **Access of data:** If a cable or device is at fault i.e. cut/damaged cable or broken device or device with non-cyber threats, this can stop the entire network from working, limiting Availability (CIA (Confidentiality, Integrity and Availability) triad) of data and access to data.
