------------
# Report on the Outage of Holberton website
------------

<img src=./image.png width=50% height=50%>

### Issue Summary
On  April 24th, 2022 the Holberton site was noted to return 500 Internal Server Error's  on all GET request made on the platform routes, when the expected response was an HTML file defining a simple Holberton site. 75% of the users were affected. The root was an outage that occurred on the Master server, (Web-A) running on Nginx server.

### Timeline
The outage was noted by Mr. Emeka through the server’s (Datadog) On-call monitoring system at 03.00 (WAT) on Tuesday 24th April 2022. The debugging and fixing of the WEB-A server lasted for 2 hours. 

### Root cause and resolution
- The master server Web-A stopped functioning due to overloading coming from multiple requests at the same time. It was noted that the capacity of the load-balancer can no longer manage the increased traffic on the site. Actually, the Holberton website stats as at 31st of March noted increase by 8% against the usual 2% increase at the beginning of a new session.
- To remedy the situation, a temporary fix was adopted. The request on the Web-A server was channeled to the Web-B server. The master server was temporarily disconnected for memory clean-up then connected back to the load-balancer and round-robin algorithm was configured so that both the master and client servers can handle equal number of requests

### Corrective and preventative measures must contain:
All the recommended measures is in-view of accommodating the increased traffic on the website and prevent future occurrences.
-	Increase the database memory of the Web-A and Web-B servers.  
-	Add additional monitoring system on Web-B server.
-	Increase the capacity of the Load-balancer.
-	patch Nginx server.

