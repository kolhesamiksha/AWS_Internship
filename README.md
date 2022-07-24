# AWS_Training and Internship

In this Task Attached Frontend(Wordpress) to Backend(RDS database) using Loan Balancer.

1. Launched aws-linux instance over aws and downloaded httpd, php7.3, and wordpress latest.tar.sh file.
2. move the latest.tar.gz file to cd /var/www/html.
3. created RDS instance.
4. After running the private Ip address wordpress configuration page get displayed by feeding database name, admin, password, RDS endpoint information. a configuration details page arises.
whatever information was there into that page should be made changes in the /var/www/html/wp-config-sample.php and after running the configuration. wordpress got successfully launched over our instance.
same procedure is followed for another EC-2 instance and lastly Application Load Balancer created and attatched to both instances.
Hence wordpress succesfully get able to accessed using load balancer.


### EC-2

An EC2 instance is nothing but a virtual server in Amazon Web services terminology. It stands for Elastic Compute Cloud. It is a web service where an AWS subscriber can request and provision a compute server in AWS cloud.

An on-demand EC2 instance is an offering from AWS where the subscriber/user can rent the virtual server per hour and use it to deploy his/her own applications.

The instance will be charged per hour with different rates based on the type of the instance chosen. AWS provides multiple instance types for the respective business needs of the user.

Thus, you can rent an instance based on your own CPU and memory requirements and use it as long as you want. You can terminate the instance when it’s no more used and save on costs.


### RDS

Amazon Relational Database Service (Amazon RDS) is a web service that makes it easier to set up, operate, and scale a relational database in the AWS Cloud. It provides cost-efficient, resizable capacity for an industry-standard relational database and manages common database administration tasks. 
You can use the database products you are already familiar with: MySQL, MariaDB, PostgreSQL, Oracle, Microsoft SQL Server.

Amazon RDS manages backups, software patching, automatic failure detection, and recovery.

You can turn on automated backups, or manually create your own backup snapshots. You can use these backups to restore a database. The Amazon RDS restore process works reliably and efficiently.

You can get high availability with a primary instance and a synchronous secondary instance that you can fail over to when problems occur. You can also use read replicas to increase read scaling.

In addition to the security in your database package, you can help control who can access your RDS databases by using AWS Identity and Access Management (IAM) to define users and permissions. You can also help protect your databases by putting them in a virtual private cloud (VPC).

### Load Balancer

A load balancer serves as the single point of contact for clients. Clients send requests to the load balancer, and the load balancer sends them to targets, such as EC2 instances. To configure your load balancer, you create target groups, and then register targets with your target groups. You also create listeners to check for connection requests from clients, and listener rules to route requests from clients to the targets in one or more target groups.
It's helful to distribute the workload across different services/platforms.
