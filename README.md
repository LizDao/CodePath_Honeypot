
# Project 7 - WordPress Pentesting

Time spent: **5** hours spent in total

> Objective: Stand up a basic honeypot and demonstrate its effectiveness at detecting and/or collecting data about an attack
  1. I deployed 2 honeypots:
      a. mhn-honeypot-1
      b. mhn-honeypot-2
      
      
   2. Issues I encountered:
      1. Session Timeout: 
          - When I tried to load the external IP in a browser, it gave me a timeout error every time. 
          - Fix: Find the mhn-admin VM under "Instances" and click on "Edit". Under the "Firewalls" settings 
                 check the both the boxes "Allow HTTP traffic" and "Allow HTTPS traffic". Click on "Save". 
      2. Cannot see event in MHN: 
         - After deployed and attack the honeypot, I can see the number of attack increased in the View Sensors page but nothing
         showed on the the Attack page. And when I tried to export json report, it showed 0 record exported.
       
         - Fix: 
            + [MHN Troubleshooting Guide](https://github.com/threatstream/mhn/wiki/MHN-Troubleshooting-Guide)
            + Section: "I have an internally deployed honeypot and even when I scan it, I see not events in MHN."
       
    
   3. Summary of data:   
        1. Number of attacks:
            - Honeypot 1: 3616 attacks (within 3 days)
            - Honeypot 2: 89 attacks (within 3 hours)
        2. Top Source IP:
        
                 Source_IP   Freq          
                 35.239.84.63  992  
               185.244.25.164  298 
               209.141.35.236  141 
                68.183.123.55  116 
                209.141.56.95  112 
                  185.8.50.73  103 
              
              
         3. Top Source Port:
         
                  Port   Freq
                 44828   43
                 13714   29
                 51422   19
                 45629   17
                 
         4. Top Destination Port:
         
                Port  Freq
                8088 1552
                  23  209
                8080  127
                  80   96
                 445   68
    
   4. There were no malware captured
        ![pay load screen shot](https://github.com/LizDao/CodePath_Honeypot/blob/master/Screenshot_2018-11-04%20Payloads.png)
   5. Session Data Report    
      [json file](https://github.com/LizDao/CodePath_Honeypot/blob/master/session.json)
      
      [csv file](https://github.com/LizDao/CodePath_Honeypot/blob/master/session2.csv)
