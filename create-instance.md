Launching an instance
to launch a linux instance go to AWS management console.
>open the amazon EC2 console at [https://console.aws.amazon.com/ec2/](https://console.aws.amazon.com/ec2/)

>from console dashboard choose launch instance.
>The Choose an Amazon Machine Image (AMI) page displays a list of basic configurations, called Amazon Machine Images (AMIs), that serve as templates for your instance. Select an HVM version of Amazon Linux 2. Notice that these AMIs are marked "Free tier eligible."

>On the Choose an Instance Type page, you can select the hardware configuration of your instance. Select the t2.micro type, which is selected by default. Notice that this instance type is eligible for the free tier.

>Choose Review and Launch to let the wizard complete the other configuration settings for you.

>On the Review Instance Launch page, under Security Groups, you'll see that the wizard created and selected a security group for you. You can use this security group, or alternatively you can select the security group that you created when getting set up using the following steps:

**Choose Edit security groups.**

>On the Configure Security Group page, ensure that Select an existing security group is selected.

>Select your security group from the list of existing security groups, and then choose Review and Launch.

>On the Review Instance Launch page, choose Launch.

>When prompted for a key pair, select Choose an existing key pair, then select the key pair that you created when getting set up.



Warning

**Don't select the Proceed without a key pair option. If you launch your instance without a key pair, then you can't connect to it.**

>When you are ready, select the acknowledgement check box, and then choose Launch Instances.

>A confirmation page lets you know that your instance is launching. Choose View Instances to close the confirmation page and return to the console.

>On the Instances screen, you can view the status of the launch. It takes a short time for an instance to launch. When you launch an instance, its initial state is pending. After the instance starts, its state changes to running and it receives a public DNS name. (If the Public DNS (IPv4) column is hidden, choose Show/Hide Columns (the gear-shaped icon) in the top right corner of the page and then select Public DNS (IPv4).)

>It can take a few minutes for the instance to be ready so that you can connect to it. Check that your instance has passed its status checks; you can view this information in the Status Checks column.