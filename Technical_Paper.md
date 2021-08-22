## **SCALING**

Scaling is a process of a system to enhance it's capacity to match the client's demand.

## **Load Balancing**

__*Load balancing*__ can be defined as it is a process of distributing application or network traffic across multiple servers to minimize the server response time.

## **Load Balancer**

A load balancer can be:

* A physical device(hardware)
* Application(software) delivery controller(ADC)
* An algorithm

![Load Balancing](https://www.nginx.com/wp-content/uploads/2014/07/what-is-load-balancing-diagram-NGINX-1024x518.png)

A load balancer distributes traffic to different web servers in the resourse pool so that no single servers gets overloaded and become unreliable. Load balancers minimize server response time.

It actually takes the requests from clients and allocates servers according to the load which is already there on servers. Like, if a server is idle, then it immediately assigns the traffic to that server so that the user gets the response without waiting much. And also it checks for the availability and reliability of the servers.

Some load balancing algorithms:

1. Round Robin
1. Least Connection Method
1. Least Response Time Method
1. Least Bandwidth Method
1. Hashing Methods
1. Custom Load Method

## **Scalability**
The scalability of a system or an application can be measured by the number of requests it can effectively support simultaneously. The state at where it can no longer handle additional requests effectively is the limit of its scalability, and it's due to when the hardware resources runs out, requiring more machines.

We may scale this resources in any combination of adjustments to CPU and physical memory(more machines), hard disk etc.

For this, we have two types of scaling,

1. Vertical Scaling(scaling up)

1. Horizontal Scaling(scaling out)

![scaling](https://www.section.io/assets/images/blog/featured-images/horizontal-vs-vertical-scaling-diagram.png)

### **differences between Horizontal and Vertical Scaling**

>  | Horizontal Scaling | Vertical Scaling
 --- | --- | ---
**Databases** | It is based on the partitioning of data(each node only contains part of the data).| In this, the data lives on a single node and scaling is done through multi-core, like, spreading the load between CPU and RAM resources of the machine.
**Concurrency**| Done with Master/Worker, Tuple Spaces, Blackboard, MapReduce.|Performed via multi-threading and in-process message passing.
**Message passing** | The data sharing is more complex and updating is more costly.|The data sharing and message passing can be done by passing a reference.
**Examples** | [Cassandra](https://cassandra.apache.org/_/index.html), [MongoDB](https://www.mongodb.com/), [Google Cloud Spanner](https://cloud.google.com/spanner)| [MySQL](https://www.mysql.com/),[Amazon RDS](https://aws.amazon.com/rds/)

#### **The decision to scale up or scale out depend on the following factors**
* Perfomance
* Flexibility
* Regularity of Upgrades
* Redundancy
* Geographical Distribution
* Cost




#### References:
* [nginx](https://www.nginx.com/resources/glossary/load-balancing/)
* [citrix](https://www.citrix.com/en-in/solutions/application-delivery-controller/load-balancing/what-is-load-balancing.html)
* [section.io](https://www.section.io/blog/scaling-horizontally-vs-vertically/)










