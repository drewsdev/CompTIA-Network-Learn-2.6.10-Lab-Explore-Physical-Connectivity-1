# CompTIA-Network-Learn-2.6.10-Lab-Explore-Physical-Connectivity-1
## CompTIA CertMaster Learn v9.1

Complete this lab as follows:

1. View the current state of the first six ports on the Cisco switch and its accompany patch panel.  
  a. Under Networking Closet, select Hardware.  
  b. Zoom in on the Cisco switch in the rack to view the power and network activity lights.  
  c. From the top right, select Questions.  
  d. Answer Questions 1-3.  
  e. Minimize the Lab Questions window.  
2. Determine which computers are plugged into ports 1 and 3.  
  a.From the Cisco switch, select the wires plugged into ports 1 and 3.  
  b.Look at the patch panel and find the cables accompanying port.  
  c. From the top right, select Questions.  
  d. Answer Question 4.  
  e. Minimize the Lab Questions window.  
3. From the ITAdmin workstation, ping each of the following computers using the IP addresses shown below:

| Computer Name                         | IP Address   |
|---------------------------------------|--------------|
| Office1                               | 192.168.0.30 |
| Exec                                  | 192.168.0.34 |
| CorpServer                            | 192.168.0.10 |
| Building A router                     | 198.28.56.1  |
| CorpNet Router's Internal Interface   | 198.28.56.1  |
| CorpNet's Router's External Interface | 198.28.56.17 |
| ISP                                   | 163.128.1.1  |  
  a. From the top left, select Floor 1 Overview.  
  b. Under IT Administration, select ITAdmin.  
  c. Right-click Start and then select Terminal (Admin).  
  d. Type ping ip_address and then press Enter.  
  Make a note as to whether the ping was successful or not.  
  e. Repeat step 3d for each remaining IP address.  
  f. Answer Questions 5-6.  
  g. Minimize the Lab Questions window.  
4. From ITAdmin, check for network connectivity.  
  a. From the taskbar, right-click the Network icon and select Network and Internet settings.  
  From the diagram at the top, you are informed that you have an ethernet connection.  
  b. Below the diagram, select Ethernet icon.  
  You are now shown details about your network connection.  
  c. Close the Settings app.  
5. From the hardware view of ITAdmin, check for network connectivity and activity by viewing the network card's link lights.  
  a. From the top left, select IT Administration to view the hardware of the computers in this office.  
  b. Above the ITAdmin workstation (not the monitor), select Back. Notice that:  
    * The link light for the network card is illuminated, indicating a physical connection (link) between this workstation and the next device (the network switch).  
    * The network activity light is blinking, indicating that network traffic is being transmitted on this connection.  
    * These two lights match what you saw when viewing the cables connecting ITAdmin to the Cisco switch and the patch panel.  
6. From the Exec operating system, check for network connectivity.  
  a. From the top left, select Floor 1 Overview.  
  b. Under Executive Office, select Exec.  
  c. Right-click Start and then select Settings.  
  d. Select Network & internet.  
  Under the Network & internet heading, you see that this computer is not connected to any networks.  
  e. Close the Settings app.  
7. From the hardware view of Exec, check for network connectivity and activity by viewing the network card's link lights.  
  a. From the top left, select Executive Office to view the hardware for the computers in this office.  
  b. Above the Exec workstation (not the laptop), select Back.  
  c. Zoom in on the Ethernet cable and examine its link lights.  
  d. The link and network activity lights for the Ethernet port with a cable plugged in are not illuminated. This indicates there is no connection to the switch.  
  Possible causes for no connectivity include:  
      * A faulty or disconnected cable  
      * A bad network card (NIC)  
      * A faulty or disabled switch port  
8. From Exec, test the possibility of a bad NIC by dragging the network cable from the existing network card to the onboard port.  
  a. Drag the Ethernet cable from its existing location to the Ethernet onboard port.  
  b. Answer Question 7.  
9. From the Exec operating system, check for network connectivity.  
  a. On the Exec monitor, select Click to view Windows 11.  
  b. Use the ping command to try to access the following computers:  
      * Right-click Start and then select Terminal (Admin).  
      * Type ping 192.168.0.10 (the CorpServer) and press Enter.  
      * Type ping 163.128.1.1 (the ISP) and press Enter.  
      Both pings are successful.  /n
  c. Right-click Start and then select Settings.  
  d. Select Network & internet.  
  e. Under the Network & internet heading, you see that this computer is now connected to the internet.  
  f. Close the Settings app.  
10. In the Networking Closet, check the link light status for Exec.  
  a. From the top left, select Floor 1 Overview.  
  b. Under Networking Closet, select Hardware.  
  c. Zoom in on the Cisco switch.  
  The network activity lights on the switch (port 1) are blinking, indicating that the Exec computer has a connection and network activity.  
11. From the Hardware view of Office1, check for network connectivity.  
  a. From the top left, select Floor 1 Overview.  
  b. Under Office 1, select Hardware.  
  c. Above the workstation, select Back.  
  The link and network activity lights are not illuminated, indicating that there is no connection to the switch.  
  Possible causes for no connectivity include:  
      * A faulty or disconnected cable  
      * A bad network card (NIC)  
      * A faulty or disabled switch port  
12. Test the network cable for Office1.  
  a. Unplug the existing Ethernet cable from the wall plate and the back of the computer.  
  b. From the Shelf, expand Cables.  
  c. Select the Cat6a Cable (a known good cable).  
  d. From the Selected Component pane:  
      * Drag one RJ45 Connector to the Ethernet port (red) in the wall plate.  
      * Drag the other RJ45 Connector to the Ethernet port in the computer.  
      The link and network activity lights on the NIC still don't show an active connection. Therefore, the cable in the office wasn't the problem.  
13. From the wiring closet, test the network patch cable for Office1.  
  a. From the top left, select Floor 1 Overview.  
  b. Under Networking Closet, select Hardware.  
  c. Remove the existing patch cable from Off 1 (Office 1) and from port 3.  
  d. From the Shelf, select the Cat6a Cable. RJ45.  
  e. From the Selected Component pane:  
      * Drag one RJ45 Connector to the Off 1 port on the patch panel.  
      * Drag the other RJ45 Connector to the port 3 on the Cisco switch.  
      The link and network activity lights for port 3 indicate an active connection. The patch cable in the Network Closet was the problem.  
14. From Office1, test the network connection to the following devices.  
  a. From the top left, select Floor 1 Overview.  
  b. Under Office 1, select Office1.  
  c. Right-click Start and then select Terminal (Admin).  
  d. Ping the following devices:  
      * Office1: 192.168.0.30  
      * Exec: 192.168.0.34  
      * ISP: 163.128.1.1  
      You are now able to ping all devices verifying local and internet connectivity.  
  e. (Optional)  
      * Look at the Network icon in the notification area.  
      * The icon indicates a normal network connection.  
      * Right-click Start and then select Settings.  
      * Select Network & internet.  
      * Under Status, you see that this computer is now connected to the internet.  
      * Close the Settings app.  
15. Score the lab.  
  a. From the top right, select Questions.  
  b. Select Score Lab.
