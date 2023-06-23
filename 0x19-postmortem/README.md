


Issue Summary:
Duration: May 10th, 2023, 9:00 AM EST - May 10th, 2023, 12:00 PM EST
Impact: The company's e-commerce website was down, resulting in 100% of users being unable to access the site. Users attempting to access the website received a "502 Bad Gateway" error message.
Root Cause: The root cause of the outage was an issue with the load balancer configuration. A recent change to the load balancer's settings resulted in misconfigured health checks, causing it to mark all backend servers as down and blocking traffic to the website.
Timeline:
9:00 AM EST: The issue was detected when a customer support representative received a complaint from a user unable to access the website.
9:05 AM EST: The incident was escalated to the engineering team, who began investigating the issue.
9:10 AM EST: The team discovered that the load balancer was blocking traffic to all backend servers.
9:15 AM EST: Assumptions were made that the issue was related to server configuration and the team began investigating the servers.
9:30 AM EST: The team discovered that all backend servers were operational and correctly configured.
9:45 AM EST: It was discovered that the load balancer was misconfigured, causing it to mark all backend servers as down.
10:00 AM EST: The team attempted to resolve the issue by restarting the load balancer, but this did not fix the issue.
11:30 AM EST: The team identified the root cause as a misconfigured health check and made the necessary changes to the load balancer's configuration.
12:00 PM EST: The website was fully operational and accessible to all users.
Root Cause and Resolution:
The root cause of the outage was a misconfigured health check on the load balancer, causing it to mark all backend servers as down. This blocked all traffic to the website and resulted in the "502 Bad Gateway" error message for users attempting to access the site.
The issue was fixed by correcting the load balancer's configuration. The team adjusted the health check settings to properly detect the status of the backend servers. Once this change was made, the load balancer began forwarding traffic to the backend servers, and the website became fully operational.


Corrective and Preventative Measures:
To prevent similar issues in the future, the engineering team will implement several corrective and preventative measures. These include:
Adding additional monitoring to the load balancer to ensure the proper functioning of health checks.
Conducting regular load testing to identify and address any potential issues before they become outages.
Implementing a disaster recovery plan to ensure the timely recovery of the website in the event of an outage.
Tasks to address the issue include:
Conducting a thorough review of load balancer configurations to ensure they are properly set up.
Implementing additional monitoring and alerts to quickly identify and address any potential issues.
Developing and testing a disaster recovery plan to ensure timely recovery in the event of an outage.
Overall, the engineering team has taken steps to prevent similar issues from occurring in the future and has implemented changes to ensure the timely recovery of the website in the event of an outage.


