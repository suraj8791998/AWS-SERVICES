# S3 BUCKETS 

# Step 1: Access S3
    Definition: Amazon S3 is an object storage service that offers scalable and durable storage for various data types, including files,     images, and backups.
    Instructions:
       Go to the AWS Management Console.
       In the navigation pane, choose "S3."

# Step 2: Create a Bucket
    Definition: A bucket is a container for storing objects (files) in S3. Buckets have a globally unique name.
    Instructions:
        Click the "Create bucket" button.
        Choose a unique name for your bucket (e.g., my-example-bucket).
        Select the AWS region where you want to create the bucket.

# Step 3: Configure Bucket Properties
    Definition: Configure settings for your S3 bucket, including versioning, logging, and object tags.
    Instructions:
         Set up properties like versioning to keep multiple versions of objects.
         Enable server access logging for tracking access to your objects.
         Add object tags for better management.

# Step 4: Set Permissions
     Definition: Define who can access your S3 bucket and objects. This involves configuring bucket policies, access control lists (ACLs),   and CORS (Cross-Origin Resource Sharing).
     Instructions:
         Configure permissions based on your use case:Bucket policies for fine-grained access control.
         ACLs for granting specific permissions to individual objects.
         CORS for controlling web browser access.

# Step 5: Create Folders and Upload Objects
    Definition: Create folders (commonly referred to as "prefixes") within your bucket and upload objects to store data.
    Instructions:
         Within your bucket, you can create folders or "prefixes" to organize objects.
         To upload an object, select "Upload" and choose the file from your local machine.

# Step 6: Enable Static Website Hosting
    Definition: You can use S3 to host static websites, making content accessible to the public via a custom domain.
    Instructions:
         Go to the bucket's properties and enable static website hosting.
         Specify an index document and an error document.

# Step 7: Monitor and Manage Your Bucket
    Definition: Monitor usage, access, and management of your S3 bucket using features like access logs, CloudWatch metrics, and events.
    Instructions:
        Configure access logs to track requests made to your bucket.
        Set up CloudWatch alarms for monitoring bucket metrics.
        AWS S3 is a versatile storage service with numerous use cases. 
