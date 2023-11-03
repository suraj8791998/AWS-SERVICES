AWS Elastic Load Balancers (ELB):

# LOAD BALANCERS

# Step 1: Access Elastic Load Balancers
    Definition: AWS Elastic Load Balancers distribute incoming application or network traffic across multiple targets, 
          such as Amazon EC2 instances or containers.

    Instructions:

            Go to the AWS Management Console.

            In the navigation pane, choose "EC2" and then select "Load Balancers."

# Step 2: Create a Load Balancer
    Definition: Create a load balancer by specifying its type (Application, Network, or Gateway), and configure its settings.

    Instructions:

            Click the "Create Load Balancer" button.

            Choose the type of load balancer that suits your application (e.g., Application Load Balancer).

            Configure the basic settings, including the name, scheme, and IP address type.

# Step 3: Configure Listeners
    Definition: Listeners define how the load balancer routes traffic to target instances or services.

    Instructions:

            Configure listeners by specifying a protocol and port, and associate them with target groups or services.

            For example, create an HTTP listener on port 80 and forward traffic to a target group.

# Step 4: Create Target Groups
     Definition: Target groups define the targets (instances or services) that the load balancer routes traffic to.

     Instructions:

            Create a target group and specify its name, protocol, port, and health check settings.

            Register targets (e.g., EC2 instances) with the target group.

# Step 5: Set Up Routing
      Definition: Configure routing rules to determine how traffic is distributed among targets within target groups.

      Instructions:

            Set routing rules to route traffic to different target groups based on factors 
               like path patterns, host headers, or URL paths.

# Step 6: Configure Security Settings
      Definition: Configure security settings like security groups and certificates (for HTTPS listeners) to secure traffic.

      Instructions:

            Specify security groups to control incoming traffic.

            Configure SSL/TLS certificates for HTTPS listeners for secure communication.

# Step 7: Register Instances (Optional)
      Definition: If you're using EC2 instances as targets, register them with the target group to enable routing.

      Instructions:

            Select the target group and register EC2 instances by specifying their instance IDs.

# Step 8: Monitor and Auto-Scaling (Optional)
      Definition: Use CloudWatch and Auto Scaling to monitor and automatically adjust the number of 
         instances in your target groups based on metrics.

      Instructions:

            Set up CloudWatch alarms to trigger Auto Scaling actions.

            Configure Auto Scaling policies and scaling groups for target groups.

# Step 9: High Availability (Optional)
       Definition: Use features like cross-zone load balancing and failover to enhance high availability.

       Instructions:

            Enable cross-zone load balancing to distribute traffic evenly across multiple Availability Zones.

            Configure failover routing to redirect traffic to a standby load balancer in case of a failure.

