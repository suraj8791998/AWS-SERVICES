# AWS ROUTE 53

# Step 1: Access Route 53
    Definition: Amazon Route 53 is a scalable and highly available Domain Name System (DNS) web service provided by AWS. It helps route web traffic to your resources.
    Instructions:
         Go to the AWS Management Console.
         In the navigation pane, choose "Route 53."

# Step 2: Create a Hosted Zone
    Definition: A hosted zone is a container for DNS records for a specific domain. It allows you to control how your domain's DNS information is managed.
    Instructions:
         Click the "Create Hosted Zone" button.
         Enter your domain name (e.g., example.com) and choose a type (public or private).
         Route 53 automatically generates a unique Hosted Zone ID.

# Step 3: Create DNS Records
    Definition: DNS records are used to map human-friendly domain names to IP addresses or other resources.
    Instructions:
       Within your hosted zone, you can create various types of DNS records like A, CNAME, MX, etc.
       For example, create an A record to map your domain to the IP address of a web server.

# Step 4: Update Name Servers
    Definition: After creating DNS records, you need to update your domain's name servers with your domain registrar to use Route 53 for DNS management.
    Instructions:
       Route 53 provides you with a set of name server records. 
       Update these records with your domain registrar (where you purchased the domain).

# Step 5: Health Checks and Routing Policies
    Definition: Route 53 allows you to configure health checks and routing policies for your resources to enhance availability and reliability.
    Instructions:
        Create health checks to monitor the health of your resources.
        Configure routing policies such as simple, weighted, latency-based, geolocation, or failover routing based on your needs.

# Step 6: Monitor and Troubleshoot
    Definition: Use Route 53 monitoring and logging to keep track of your DNS requests and resolve any issues.
    Instructions:
          Monitor the health of your resources and DNS queries through Route 53's dashboard.
          Use CloudWatch Logs for detailed log data
