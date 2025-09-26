https://www.linkedin.com/pulse/what-happens-when-we-type-wwwgooglecom-our-browser-ingrid-mornac-fi8re

## What happens when we type www.google.com in our browser?
It’s something we all do every day, sometimes dozens of times: open a browser, type an address like www.google.com. And presto, the page appears instantly on our phone or computer. 
But behind this seemingly simple action, an incredible technological journey takes place! 
Let’s take a peek behind the scenes.

When we type www.google.com and the Enter key, the computer doesn't understand, it doesn't speak that language. A system called DNS (Domain Name System) acts like a translator. It converts the name into numbers, called an IP address, which tells the computer where to send the request on the Internet.
To actually send our message, we need to make sure it takes the right path to Google: our GPS is called 'IP Protocol'. Our factor, the 'TCP Protocol', ensures that every part of the message arrives intact and in the correct order.
For the delivery to go smoothly, we also need security. That’s where the Firewall comes in the guard at the gate. It allows normal messages to pass, and blocks suspicious ones (like viruses or attacks).
Firewalls exist on our device, at our Internet provider, and on Google’s servers.

Once the request reaches Google, it sometimes needs to be secured against spying. That’s where HTTPS (HyperText Transfer Protocol Secure) comes into play, symbolized by the padlock 🔒.
The browser and Google exchange secret keys through what’s called an SSL (Secure Sockets Layer) certificate.
The more modern and secure version is TLS (Transport Layer Security), though many people still say “SSL.”

Google receives billions of requests per day. If they all landed on a single computer, we can imagine that it would have crashed instantly. That’s why there are many servers. To decide where each request goes and keep everything fast and efficient, there’s a conductor called the Load Balancer, the traffic balancer. 
The Load Balancer directs our request to the right server, where it arrives at a Web Server.
If it’s something simple (like an image or HTML code), the web server returns the response directly.
If more logic is needed, the request goes to Google’s brain—the Application Server.
The Application Server applies the rules and algorithms that make Google work. It decides what response to send back to the browser.

Often, answering properly requires looking up information. The application server queries a massive Database, like a giant library. It contains an index of all the world's websites, user data, popular searches, and more. It can respond in just a split second. 

Finally, the web server packages everything into an http response. The response travels back through the Internet to our computer. Our browser receives the content, assembles all the elements and displays the page on our screen.
It happens in just a few milliseconds! 

To summarize the process: 
1. Find the IP → DNS resolution. 
2. Establish the communication channel →TCP/IP connection. 
3. Security filtering → Firewall verification. 
4. Encryption and authentication → HTTPS/SSL/TLS negotiation. 
5. Choose an available server → Load balancer distribution. 
6. Handle the HTTP request → Processing by the web server. 
7. Apply the business logic → Application server. 
8. Retrieve the information → Database query. 
9. Display the page in our browser → Response and rendering.  

![Web Request Diagram](https://raw.githubusercontent.com/Mornac/holbertonschool-network/blob/main/what_happens_when_your_type_google_com_in_your_browser_and_press_enter/1-what_happen_when_diagram.jpg)
