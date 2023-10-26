# Homework 7
1/c Jake Carpenter,
CNS,
25OCT23


## Part 2

The vulnerable service that I researched was on Google Chrome through HTTP on port 8000 (alternate HTTP port). This exploit requires Chrome to have the Sandbox feature disabled. Sandboxing in Chrome is a feature that keeps websites limited to their webpage, and prevents them from other activities (i.e. opening pop-ups). When starting the exploit, the host must have Google Chrome open so Metasploit can detect an instance. When configuring the exploit, Metasploit will host a server from the listeners IP and on port 8000. Once this instance is created, Metasploit will wait for hosts to connect. If any hosts types that URL of the Metasploit server, Metasploit will notify the attacker of the connection, dump the payload, and set up a meterpreter shell. Accessing the session inside Metasploit gives full control of the user to the listener while they are connected. Although this exploit seems very specific, if deployed in the right circumstances, it would be very significant. Many organizations would have Sandboxing disabled for all their external firewalls and restrictions. If an attacker were to get an internal connection, getting full access to another host through their web browser would be detrimental.



## Part 3

The CVE for the Google Chrome exploit is CVE-2020-6418: Access of Resource Using Incompatible Type ('Type Confusion'). This issue was only present on version 80.0.3987.122, so you must delete the auto-updater inside the Google Chrome files if you were to recreate this. The reason why this vulnerability was such a big deal, despite requiring Sandboxing to be disabled, is because many organizations disable Sandboxing on purpose becuase they run custom software and have different functions for their internal webistes. 
