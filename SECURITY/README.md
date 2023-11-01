# Security Group AND NACL :

**AWS Security Groups:**

# Step 1: Access Security Groups 
  Definition: AWS Security Groups act as virtual firewalls for your Amazon EC2 instances, controlling inbound and outbound traffic at the instance level.
  
  Instructions:
  
          Go to the AWS Management Console and navigate to the EC2 Dashboard.
          
          In the navigation pane, choose "Security Groups."

# Step 2: Create a Security Group
  Definition: Security Groups allow you to define rules that determine what kind of traffic is allowed to reach your EC2 instances.
  
  Instructions:
  
       Click the "Create Security Group" button.
       
       Give your Security Group a name and description.
       
       Specify inbound and outbound rules for your Security Group.
       
             Inbound: These rules control incoming traffic to your EC2 instances, specifying which protocols and ports are allowed. For example, to allow SSH 
                 access, you create an inbound rule allowing Port 22 from a specific IP address.
                 
             Outbound: These rules control outgoing traffic from your instances, specifying destinations that your instances can access. The default outbound rule 
                 allows all traffic.

# Step 3: Associate with EC2 Instances
  Definition: You need to associate your Security Group with your EC2 instances to control the traffic they receive.
  
  Instructions:
  
        Select the EC2 instances you want to associate with this Security Group.
        
        Choose "Actions" and then "Networking," and click "Change Security Groups."
        
        Add your newly created Security Group.

**AWS Network Access Control Lists (NACLs):**

# Step 1: Access NACLs
   Definition: AWS Network Access Control Lists (NACLs) are stateless, subnet-level firewalls that control inbound and outbound traffic at the subnet level in your 
          Virtual Private Cloud (VPC).
   Instructions:
   
        From the AWS Management Console, go to the VPC Dashboard.
        
        In the navigation pane, choose "Network ACLs."

# Step 2: Create a Network ACL
    Definition: Creating a NACL involves setting up rules for controlling traffic between subnets in your VPC.
    
    Instructions:
    
           Click the "Create Network ACL" button.
           
           Give your NACL a name and associate it with a VPC.

# Step 3: Define Rules
    Definition: NACL rules are used to specify what types of traffic are allowed or denied. They are stateless, so you need both inbound and outbound rules.
    Instructions:
    
           Create inbound and outbound rules as needed.
           
                Inbound: These rules control incoming traffic to the subnet, specifying which protocols and ports are allowed. For example, rule 100 might allow 
                      HTTP traffic (Port 80).
                      
                Outbound: These rules control outgoing traffic from the subnet, specifying destinations that are allowed. The default outbound rule allows all 
                    traffic.

# Step 4: Associate with Subnets
    Definition: After defining rules, you associate your NACL with specific subnets to apply the rules to the network traffic.
    Instructions:
           Go to the "Subnet Associations" tab.
           Associate your NACL with the subnets you want to protect with these rules.
