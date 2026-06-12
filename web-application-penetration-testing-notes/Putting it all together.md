# Putting it all together TryHackMe Writeup

This section tied everything together by following the journey of a website request from start to finish.
When a user enters a website address, DNS acts like the internet’s phonebook, finding the correct IP address for the destination.
The browser then communicates with the web server using HTTP to request the webpage's content.
In response, the server sends back resources such as HTML, CSS, JavaScript, and images, which the browser assembles like puzzle pieces to create the fully functional website seen on screen.
Overall, this section highlighted how several technologies work behind the scenes to transform a simple URL into the interactive web experience users encounter every day.

<img width="1350" height="347" alt="image" src="https://github.com/user-attachments/assets/6bcaa2c8-7729-45c5-827d-651e22944565" />

However, there are additional steps and components involved in this process that add extra functionality and help the web operate more efficiently.

----
# Other Components
Modern websites rely on more than just a web server to provide a fast, reliable, and secure experience.

# Load Balancers
Load balancers act like traffic controllers, distributing incoming requests across multiple servers to prevent overload and ensure users can still access the website if a server fails.

# Content Delivery Networks
CDNs (Content Delivery Networks) improve performance by storing copies of static content, such as images, videos, CSS, and JavaScript, on servers located around the world, allowing users to receive content from the nearest location.

# Databases
Databases serve as the website's memory, storing and retrieving important information such as user accounts, settings, and application data.

# Web Application Firewall
Meanwhile, WAFs (Web Application Firewalls) act as security guards, inspecting incoming traffic and blocking malicious requests before they reach the web server.

# Key Findings
Load balancers improve website performance and availability by distributing traffic across multiple servers.

Health checks allow load balancers to detect failed servers and automatically reroute traffic.

<img width="892" height="437" alt="image" src="https://github.com/user-attachments/assets/7252840e-2885-4ed2-97b4-0f4334d8b620" />

CDNs reduce loading times by delivering content from servers closest to the user.

Databases are responsible for storing and managing website data efficiently.

WAFs help protect websites from attacks by filtering and blocking harmful requests.

<img width="857" height="212" alt="image" src="https://github.com/user-attachments/assets/9308fd22-9c59-4ec5-a42f-1699e1621140" />

These technologies work together to make modern websites faster, more scalable, and more secure.

---
# The order of steps taken when requesting a web page in a browser
1. Request the website tryhackme.com in the browser
2. Check the local cache for IP to see if a similar request has been made recently. 
3. If the request is not found locally, the next order of action would be to check the recursive dns server for the IP address.
4. The DNS server will query the root server to find the authoriative DNS server.
5. 
