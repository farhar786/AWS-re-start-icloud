#  Cloud Foundations – One

## Questions
1)  **Define what IaaS, PaaS and SaaS is.**

#### Iaas:
Infrastructure as a service', is on-demand access to cloud-hosted physical and virtual servers, storage and networking - the backend IT infrastructure for running applications and workloads in the cloud.

#### PaaS:
platform as a service' is on-demand access to a complete, ready-to-use, cloud-hosted platform for developing, running, maintaining and managing applications. 

#### SaaS:
Software as a service'is on-demand access to ready-to-use, cloud-hosted application software.



2)  **Provide 6 advantages of cloud computing.
**

Cloud Computing saves money by its very nature, the cloud is designed for cost savings. 
Cloud Computing is fast Cloud Computing enables businesses to send, store, and distribute information more quickly and efficiently than before. 
Cloud Computing grants SMEs access to cutting-edge technology 
Cloud Computing offers mobility
Cloud Computing is secure 
Cloud Computing means enhanced data storage

3)  **Define what an  region and an Availability Zone is.**

*  Regions are large and widely dispersed into separate geographic locations. Availability Zones are distinct locations within an  Region that are engineered to be isolated from failures in other Availability Zones.



4)  **List all the  regions.**

The  Cloud spans 99 Availability Zones within 31 geographic regions around the world, with announced plans for 15 more Availability Zones and 5 more  Regions in Canada, Israel, Malaysia, New Zealand, and Thailand.




5)  **What are the categories in which the  services are grouped?** 

 services are grouped into 10 categories: 
Compute, Storage, Database, Networking and Content Delivery, Management and Governance, Security, Identity and Compliance, Analytics, Application Integration, Mobile and IoT, and AR and VR.


6)  **What is the difference between object storage and block storage?
**
The main difference between object storage and block storage is the way they organize and manage data. Object storage is better suited for storing large amounts of unstructured data, while block storage is better suited for structured data that requires fast and low-latency access.

7)  **List two  compute services and explain them.**

 offers the broadest and deepest functionality for compute.

*  EC2
 Amazon Elastic Compute Cloud (EC2) offers granular control for managing your infrastructure with the choice of processors, storage, and networking.

 *  Elastic Beanstalk.
 *  Fargate.
 *  Lambda.



8)  **List two  storage services and explain them.**

* S3 
Amazon S3 is a highly scalable and durable object storage service that allows users to store and retrieve data from anywhere on the web. It is designed to support a wide range of use cases, from simple backup and recovery to complex big data analytics. Some of the key features of Amazon S3 include:
Object storage
Durability and availability
Security and compliance

* Amazon EBS (Elastic Block Store
EBS
Amazon EBS is a high-performance block storage service that provides persistent storage volumes for use with Amazon EC2 instances. It is designed to provide low-latency access to data and is optimized for transactional workloads such as databases. Some of the key features of Amazon EBS include:
Block storage
Durability and availability
Snapshots and backups
Performance options



#  Cloud Foundations – Two

## Questions


**1)  Explain the  Shared responsibility model.**

A shared responsibility model is a cloud security framework that dictates the security obligations of a cloud computing provider and its users to ensure accountability. Both the customers and  have responsibily.   is responsible for what is **on** the cloud and the customers are responsible for what is **in** the cloud

      is responsible for infranstructure, the host operating system, the virtualization layer and the physical security of the cloud servers.

Customers are responsible for managing their data (including encryption options), classifying their assets, and using IAM tools to apply the appropriate permissions.


**2)  Explain an Identity and Access Management (IAM) Role.**

An IAM role is similar to an IAM user, in that it is an  identity with permission policies that determine what the identity can and cannot do in . However, instead of being uniquely associated with one person, a role is intended to be assumable by anyone who needs it. Also, a role does not have standard long-term credentials such as a password or access keys associated with it. Instead, when you assume a role, it provides you with temporary security credentials for your role session.



**3)  Explain an Identity and Access Management (IAM) Policy.**

An  managed policy is a standalone policy that is created and administered by .  managed policies are designed to provide permissions for many common use cases. They make it easier for you to get started with assigning permissions to users, groups, and roles than if you had to write the policies yourself.An  managed policy is a standalone policy that is created and administered by . Standalone policy means that the policy has its own Amazon Resource Name (ARN) that includes the policy name. For example, arn::iam:::policy/IAMReadOnlyAccess is an  managed policy.



**4)  Describe an Amazon Machine Image (AMI).**

Amazon Machine Image (AMI) is a pre-configured virtual machine image used to create an EC2 instance in the  cloud.



**5)  List the different EC2 instance types with use cases for each type.** 

##### There are four types:
* On-demand, which provides instant access to as much compute, memory and storage as you need. However, on-demand pricing is generally the most expensive.
* Spot instances. ...
* Reserved instances, which give you access to a dedicated but finite amount of resources. ...
* Dedicated hosts.


**6)  Explain Virtual Private Cloud (VPC).**

It is a virtual network infrastructure provided by cloud computing platforms such as Amazon Web Services (), Microsoft Azure, and Google Cloud Platform (GCP). 

A VPC provides a private, secure, and isolated environment for running cloud resources such as virtual machines, databases, and storage, within a defined set of IP addresses. 

Users can create subnets, route tables, and network gateways to control the traffic flow within the VPC and between the VPC and other resources in the cloud.

**7)  Differentiate between a Public and a Private subnet.**

A private subnet sets that route to a NAT gateway/instance. Private subnet instances only need a private ip and internet traffic is routed through the NAT in the public subnet. You could also have no route to 0.0.0.0/0 to make it a truly private subnet with no internet access in or out.A public subnet routes 0.0.0.0/0 through an Internet Gateway (igw). Instances in a public subnet require public IPs to talk to the internet.



# Python fact finding exercise

## Questions

* 1) Define a list and tuple in Python. Provide some examples.

A tuple is similar to a list, but it is immutable, meaning that once it is created, the elements cannot be changed. Tuples are defined using parentheses () and the elements are separated by commas. For example:
my_tuple = (1, 2, 3, 'four', 'five')
Lists are defined using square brackets [] and the elements are separated by commas.
my_list = [1, 2, 3, 'four', 'five']


* 2) What is a namespace in Python?

A namespace in Python is a mapping between names and objects. It is a way to organize and distinguish names in a program.
Python has several namespaces, including the built-in namespace, the global namespace, and the local namespace.

3) What is the difference between a local variable and a global variable?

A local variable is a variable that is defined inside a function and is only accessible within that function. Local variables have a limited scope within the function
Global variable
A global variable is a variable that is defined outside of a function and can be accessed from anywhere in the program. global variables have a wider scope that includes the entire program.


* 4) What is an IDE? Mention some common IDEs that could be used with Python.

An IDE (Integrated Development Environment) is a software application that provides a comprehensive environment for writing, testing, and debugging code.
Some common IDEs used with Python include:
•    PyCharm
•    Spyder
•    Visual Studio Code
•    IDLE (Python's built-in IDE)
•    Jupyter Notebook


* 5) What are modules in Python? Provide some examples.

In Python, a module is a file that contains Python definitions and statements.
Modules can contain functions, classes, variables, and other objects. To use a module, it must be imported into the program using the import statement. For example:
import math
result = math.sqrt(25)
print(result) # output: 5.0

* 6) What is the difference between an array and a list?

A list is used to collect items that usually consist of elements of multiple data types.
List cannot manage arithmetic operations.
When it comes to flexibility, the list is perfect as it allows easy modification of data.
It consumes a larger memory.

Array.
An array is also a vital component that collects several items of the same data type.
Array can manage arithmetic operations.
When it comes to flexibility, the array is not suitable as it does not allow easy modification of data.
It consumes less memory than a list.




* 7) What are operators? Provide some examples.

Operators are symbols that perform operations on one or more operands to produce a result. In Python. 
Arithmetic operators (+, -, *, /, %, //, **)
Comparison operators (==, !=, <, >, <=, >=)
Assignment operators (=, +=, -=, *=, /=, %=, //=, **=)
Logical operators (and, or, not)
Bitwise operators (&, |, ^, ~, <<, >>)






# Database fact finding exercise

## Questions

**1) What is the difference between a relational and a non-relational database?**

A relational database is structured, meaning the data is organized in tables. Many times, the data within these tables have relationships with one another, or dependencies. 
Some of the most common relational databases
* MySQL
* IBM Db2
* Snowflake
* Amazon Aurora
* PostgreSQL
* Microsoft SQL Server


A non relational database is document-oriented, meaning, data in a document-based format, with each document representing a record representing data in  whatever manner is best suited to the type of data being stored. Non-relational databases are designed to contain unstructured data.
Some of the most common relational databases
* MongoDB
* IBM Cloundant
* Amazon DynamoDB
* Apache Cassandra


**2) What are indexes?**

An index is a database structure that you can use to improve the performance of database activity. A database table can have one or more indexes associated with it. An index is defined by a field expression that you specify when you create the index. 
a single field name, like EMP_ID.


**3) What are primary keys and secondary keys?**

##### Primary Key
The attribute that uniquely identifies a row or record in a relation is known as primary key -like page number of a book

##### Secondary Key
A field or combination of fields that is basis for retrieval is known as secondary key (mainly used for finding details from large data)
like an index page of a book

**4) What are inner joins and outer joins?**

##### Inner Join
An Inner Join returns only the rows that have matching values in both the tables (we are considering here the join is done between the two tables).

##### Outer Join
The Outer Join includes the matching rows as well as some of the non-matching rows between the two tables. An Outer join basically differs from the Inner join in how it handles the false match condition.
There are 3 types of Outer Join:
Left Outer Join
Right Outer Join
Full Outer Join


**5) What is the difference between DROP TABLE and TRUNCATE TABLE?**

##### TRUNCATE TABLE
Removes all rows from a table without logging the individual row deletions. TRUNCATE TABLE is similar to the DELETE statement with no WHERE clause; however, TRUNCATE TABLE is faster and uses fewer system and transaction log resources.

##### DROP TABLE
Removes one or more table definitions and all data, indexes, triggers, constraints, and permission specifications for those tables.


**6) What are the different data types in SQL?**

In SQL, there are several data types that can be used to represent different types of data. 

##### Some common data types include:

* Integer: Used to store whole numbers without decimal places.
* Float/Real: Used to store decimal numbers.
* Char/Character: Used to store fixed-length character strings.
* Varchar/Varchar2: Used to store variable-length character strings.
* Date/Time: Used to store dates and times.
* Boolean: Used to store true/false values.
* Blob/Binary Large Object: Used to store large binary objects such as images, audio, or video files.
* Decimal/Numeric: Used to store decimal numbers with fixed precision and scale.
* Text: Used to store large amounts of text data.
* XML: Used to store XML documents.

These data types can be used in SQL to define the structure of tables, columns, and variables, and to ensure that the data stored in the database is consistent and accurate.

**7) Explain the WHERE and HAVING clauses.**

##### WHERE Clause
The WHERE clause is used to fetch the data which specify the given condition. It is used to filter records and select only necessary records. It is used with SELECT, UPDATE, DELETE, etc. query. The SQL also implements and, or, and not in the WHERE clause which is known as the boolean condition.
Example:
SELECT COUNT(*)
FROM employee;
Result:
COUNT(*)200 

##### HAVING Clause

The HAVING clause is generally used along with the GROUP BY clause. This clause is used in the column operation and is applied to aggregate rows or groups according to given conditions.
Example: Let’s say you wanted to find the SUM of salaries per department.
SELECT department_id,
SUM(salary) AS total_sal
FROM employee
GROUP BY department_id
ORDER BY department_id; The difference between WHERE and HAVING clauses are:
The WHERE clause is used to filter rows before the grouping is performed.
The HAVING clause is used to filter rows after the grouping is performed. It often includes the result of aggregate functions and is used with GROUP BY




#  Well-Architected Framework fact finding 

## Questions

**1)  What are the five pillars of the Well Architected Framework (WAF)?**

The five pillars of  Well-Architected Framework are as follows:
* Operational Excellence
* Security
* Reliability
* Performance Efficiency
* Cost Optimization


**2)  What are the 3 areas of operational excellence in the cloud?**

The Operational Excellence pillar includes the ability to support development and run workloads effectively, gain insight into their operations, and to continuously improve supporting processes and procedures to deliver business value.

**3)  What are the design principles that strengthen system security?**

* Implement a strong identity foundation.
* Enable traceability.
* Apply security at all layers.
* Automate security best practices.
* Protect data in transit and at rest.
* Keep people away from data.
* Prepare for security events.


**4)  What are the design principles that increase reliability?**

The design principles that increase the reliability in the  Framework are:

* To automatically recover from failure
* Test recovery procedures
* Scaling horizontally to increase aggregating workload availability.
* Stop guessing capacity.Managing change in automation.
* The reliability pillar provides an overview of design principles, best practices, and questions.


**5)  What are the areas to focus on to achieve performance efficiency in the cloud?**

There are four best practice areas that help achieve performance efficiency in the cloud and these are as follows:

* Selection- Using a data-driven approach to select the patterns and implementation for your architecture and achieve a cost effective solution.
* Review- Cloud technologies are rapidly evolving and you must ensure that workload components are using the latest technologies and approaches to continually improve performance.
* Monitoring- After you implement your workload, you must monitor its performance so that you can remediate any issues before they impact your customers. 
* Monitoring metrics should be used to raise alarms when thresholds are breached.Tradeoffs- When you architect solutions, think about tradeoffs to ensure an optimal approach. 
* Depending on your situation, you could trade consistency, durability, and space for time or latency, to deliver higher performance.


**6)  What are the different approaches to using  resources in a cost-effective manner?**

Different approaches to use  resources in an effective way are by modifying the demand, using a throttle, buffer, or queue to smooth the demand and serve it with less resources resulting in a lower cost, or process it later with a batch service. 

In , you can automatically provision resources to match the workload demand.


#  Billing

## Questions

** 1) List the different types of  support plans.**

There are four different types of  support plans:
* Basic Support: This plan is included with every  account and provides access to  Trusted Advisor,  Personal Health Dashboard, and customer service through email, phone, and chat.

* Developer Support: This plan is designed for developers and provides technical support for  infrastructure services. It includes all the benefits of Basic Support plus 24/7 access to  technical support, unlimited cases, and personalized support.

* Business Support: This plan is designed for businesses that are running production workloads on . It includes all the benefits of Developer Support plus  Trusted Advisor checks for cost optimization, performance improvement, security, and fault tolerance.

* Enterprise Support: This plan is designed for large enterprises that are running mission-critical workloads on . It includes all the benefits of Business Support plus a Technical Account Manager (TAM) who provides personalized support and guidance, and proactive monitoring and planning services to optimize your  infrastructure.


**2) Explain the  Simple Monthly Calculator.**

The  Simple Monthly Calculator is a tool that allows you to estimate your monthly  usage costs based on your expected usage of various  services. It is a free web-based tool that can help you to plan and budget your  infrastructure costs before you start using  services.

The  Simple Monthly Calculator allows you to estimate the costs of different  services based on various usage scenarios.

You can enter details such as the number of instances, the type of instances, the storage required, data transfer requirements, and other factors that affect the cost of using  services.

The  Simple Monthly Calculator provides an estimated cost for each service that you use, as well as a breakdown of the costs for each component of the service. 
You can use this information to optimize your usage of  services and reduce your infrastructure costs.


**3) List and explain the different EC2 pricing models.**

There are four different EC2 pricing models, each with its own characteristics and cost structure. 
They are as follows:

* On-Demand Instances: 

This pricing model allows you to pay for your EC2 instances on an hourly basis, with no long-term commitments or upfront costs. You only pay for the hours that you use the instances. This pricing model is suitable for short-term, unpredictable workloads, or for applications that require the flexibility to scale up and down quickly.

* Reserved Instances: 

This pricing model allows you to reserve capacity on the EC2 platform for a specified period of time, up to 3 years. By committing to use the capacity for a longer period, you can get a discount on the hourly rate compared to On-Demand Instances. Reserved Instances are suitable for applications with predictable workloads, or for those that require capacity for a longer period.

* Spot Instances: 

This pricing model allows you to bid on unused EC2 capacity, and if your bid is accepted, you can use the capacity at a much lower hourly rate than On-Demand Instances. However, the capacity is not guaranteed, and if the spot price goes above your bid, your instances will be terminated. Spot Instances are suitable for applications with flexible start and end times, or for workloads that can be interrupted or stopped without any negative impact.

* Dedicated Hosts: 

A Dedicated Host is a physical EC2 server dedicated for your use. Dedicated Hosts can help you reduce costs by allowing you to use your existing server-bound software licenses like Windows server, SQL server etc.