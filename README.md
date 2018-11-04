# Project 7 - WordPress Pentesting

Time spent: **5** hours spent in total

> Objective: Stand up a basic honeypot and demonstrate its effectiveness at detecting and/or collecting data about an attack

## Pentesting Report

    1. I deployed 2 honeypots:
      a. mhn-honeypot-1
      b. mhn-honeypot-2
      
      
    2. Issues I encountered:
      a. Session Timeout: 
        - When I tried to load the external IP in a browser, it gave me a timeout error every time. 
        - Fix: . Find the mhn-admin VM under "Instances" and click on "Edit". Under the "Firewalls" settings check the both the boxes   "Allow HTTP traffic" and "Allow HTTPS traffic". Click on "Save". 
    Any issues you encountered
    A summary of the data collected: number of attacks, number of malware samples, etc.
    Any unresolved questions raised by the data collected
