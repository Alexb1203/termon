# termon
Raspberry Pi Hardware Monitor Application. See CPU &amp; GPU Performance of your Desktop/Laptop from a raspberry pi.
This is a client application, please download the server application from https://openhardwaremonitor.org/downloads/

The server application makes your hardware vitals accessible; serving a json webpage with all the information needed.

This client application is designed to neatly print that JSON data using Java in Terminal or Command Prompt.

I would recommend editing /etc/rc.local on the raspberry pi and inserting a statement below.

Run with "Java -jar termon.jar [Refresh in Miliseconds] [Instert Desktop IP Here]"

ex: Java -jar termon.jar 1000 192.168.1.245:8080

Right now it is setup to look for keywords using NVIDIA & INTEL.
I do not have AMD products so I have not made it look for AMD products.
You may download the source and re-appropiate it for your needs. It should be extremely simple changes to support AMD
or any other products.
