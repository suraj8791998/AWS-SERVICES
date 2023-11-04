# HERE I CAN ACCESS THE JENKINS PAGE BY USING ROUTE 53 SERVICE RATHER THAN PUBLIC IP
We can use Route 53 service to access jenkins page.

# Step 1: Sign in to AWS and Open Route 53

Sign in to the AWS Management Console.

Navigate to the Route 53 service by clicking on "Services" in the top left corner, and then selecting "Route 53" under the "Networking & Content Delivery" section.

# Step 2: Create a Hosted Zone

In the Route 53 dashboard, click on "Hosted zones" in the left navigation pane.

Click the "Create hosted zone" button.

Enter your domain name "jenkis.com" in the "Domain Name" field, and ensure "Public hosted zone" is selected.

Click the "Create hosted zone" button.

# Step 3: Configure DNS Records

Inside your hosted zone, you need to create DNS records to direct traffic to your desired resources. Commonly, you'll create an "A" record for the root domain or subdomains.

Click the "Create record set" button.

For the root domain (jenkis.com), leave the "Name" field empty.

In the "Type" field, select "A - IPv4 address."

In the "Value" field, enter the IP address of the resource you want to point to. If you're pointing to an EC2 instance, this will be the instance's public IP address.

Optionally, set a TTL (Time to Live) for the DNS record.

Click "Create" to save the record.

You can also create other DNS records like CNAME, MX, or TXT records as needed.

# Step 4: Update Domain Registrar

If your domain "jenkis.com" is registered with a domain registrar other than AWS (e.g., GoDaddy, Namecheap), you need to update the DNS settings at your registrar to point to the Route 53 name servers. Here's a general overview of the steps:

Log in to your domain registrar's website.

Find the DNS settings or name server configuration section.

Replace the existing name servers with the ones provided by AWS in your Route 53 hosted zone. You can find these name server values in the "NS" (Name Server) records of your hosted zone.

Save the changes.

# Step 5: Verify and Wait for DNS Propagation

After updating your domain registrar's name servers, it may take some time for DNS changes to propagate across the internet. This process can take from a few minutes to several hours or more. During this period, your domain "jenkis.com" will become fully functional with Route 53.

That's it! You've now configured Route 53 for your domain, and you can use Route 53's DNS service to manage your DNS records for "jenkis.com." Users can access resources associated with your domain through the DNS records you've configured in Route 53.




