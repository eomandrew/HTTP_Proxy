# HTTP_Proxy
This is a Java web proxy server that intercepts each and every HTTP request and forwards it on to the web server. This proxy controls the response that is sent to the client from the web server. The modifications made on the response affects all text, hyperlinks, and images.
## Installation/Execution
1.) Download all files locally  
2.) Compile the java files (This proxy is currently using a deprecated method of DataInputStream)  
```bash
javac *.java
javac Proxy.java -Xlint:deprecation Proxy.java HttpRequest.java HttpResponse.java
```
3.) “Proxy.java” is my main class and should be executed with 1 argument, which is the port number.  
The port number is what the proxy will connect to for incoming connections from clients. To use the proxy server with browser and proxy on separate computers, you will need the IP address on which your proxy server is running. In this case, while running the proxy, you will have to replace the “localhost” with the IP address of the computer where the proxy server is running. Also note the port number used to configure your proxy settings on the machine.

## How to Use
1.) Go to your browser (I used firefox), and change the proxy settings to manual, passing in
"localhost" and whatever port number you would like (make sure it is between 0 –
65535) to use for the HTTP proxy.  
To use the proxy server with browser and proxy on separate computers, you will need the IP address on which your proxy server is running. Instead of passing in "localhost" to the proxy, you will need to pass in the IP address of the system using the proxy. 
2.) Execute the Proxy class using the same port number as its argument  
3.) The changes made by the proxy will be most noticeable on the website http://pages.cpsc.ucalgary.ca/~sina.keshvadi1/441/web/index.html  
4.) if everything is working, you should see changes to:
2019 to 2219 • NBA to TBA 1 • World to Titan • Drummond to Kobe-B24 

### Contact
Andrew Eom  
eomandrew@gmail.com
