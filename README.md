# General-NOtes

AKS Cluster
Docker Image
WAF
Azure Service Bus
Big Data Source (Whether Databricks, Data Lake, Azure Data Factory), introduce into docker image
how will you send that source for processing
You need to deploy LB as a service in AKS, Load Balancer - AKS will create a service for load balancing which will take care of my public ip
Gateway
Apache Spark - is the framework which deals with computing elements and doesnt deal with storage


Network and Solution Architecture 



Big Data - Structured Data (SQL, Row and Collum Data), Semi Structured Data (JSON, XML, CSV), Unstructured Data (Image, Video and File related data) - 


- First we will create the docker file for the required services
- create an image out of that docker file
- Push that image to an existing or new container registry after tagging it
- Second create an AKS cluster (here we will be taking 2 node cluster) and attaching the Azure container registry which we
created in the orevious step
- GET the AKS credentials

Taking an example of ticket booking application
User >> WEB App for Hotel, Flight >> Booking Engine Vendor API <<>> Payment 
                                                         <<Service Bus>> Order Processing >> Seat Allocation, Price Match AI EMAIL  
														 
Azure Service Bus has 2 components (1. Queues - Works on FIFO) (2. Topics and Subscription - Here you can apply filter whether it is a 													transaction yes or transaction no)


1. One container of apache spark
2. one container of application
3. Service Bus Instance




Questions - how to club azure servuce bus with AKS


https://github.com/anildwarepo/spark-on-aks with Datalake


1. Design the Network and Solution architecture for containerized Microservice application components in Azure
2. The Application UI is accessible from Internal and external customers and It need to handle the txn Volume 5000 msgs per second.
3. The application components communicates through service bus for resiliency.
4. Application also has backend components to kick off Spark based data processing workloads.
Think through problems and demonstrate creativity how you have resolve them.


Azure CNI

