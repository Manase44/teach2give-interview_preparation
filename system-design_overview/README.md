- [SYSTEM DESIGN](#system-design)
- [Understanding System Design](#understanding-system-design)
  - [Importance of System Design](#importance-of-system-design)
  - [Essential Design Methods in System Design](#essential-design-methods-in-system-design)
  - [Fundamental Concepts of System Design](#fundamental-concepts-of-system-design)
  - [Advanced Concepts of System Design](#advanced-concepts-of-system-design)
  - [Components of System Design](#components-of-system-design)
  - [Steps For Preparing System Design](#steps-for-preparing-system-design)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# SYSTEM DESIGN
# Understanding System Design
___
System design is the process of defining the architecture, models, and components of a system in order to meet specific user requirements while considering factors like scalability, aintainability, and perfomance.  
## Importance of System Design
- Gives a clear understanding of the user functional and non-functional requirements and how exactly to achieve them.  

- Provide a platform for making fundamental decisions for the project, such as deciding whether to go with SQL or NoSQL database.  

- System design enhances the quality of a system by ensuring it is scalable and can accomodate traffic increase.  

- It provides the structural layout of how the system's components will be designed, for example, how many servers will be installed and where. 

- It enhances the efficiency of the system by ensuring that the architecture and models of the system are optmized.


## Essential Design Methods in System Design
There are various method and techniques used to design the system architecture, and they include:  

1. **Architectural design** - This method describes the structure, model, components, and interaction of the entire system.
2. **ERD diagrams** - Entity relationship diagrams are used to design the applications database structure; define schemas, system entities, attributes, and the relationship betwen entities. 

3. **UML diagrams** - Unified modeling language is a collection of various system modeling techniques used to represent various aspects of the system.

4. **Class diagrams** - It describes the system's data and functionality by representing the classes, class attributes, class methods, and the relationship between multiple classes.  

5. **Sequence diagrams** - This method models the beahvior of the system by representing the interactions between various components in the system.

## Fundamental Concepts of System Design 

1. ### Performance and scalability
      
      __Performance__ is the speed and efficiency at which a system can execute a task. Caching is one of the many mechanisms to ensure high performance of a system.  

      __Scalability__ is the ability of a system to accormodate changes and growth in traffic. Distributing loads among several servers is one method of guaranteeing scalability of a system.


2. ### Latency and throughput
  
      __Latency__ is the time taken for data to be transmitted from one point to another in a system.  It is measured in miliseconds. It is affected by network structure, geographics distance, and the transport protocol.

      __Throughput__ is the number of operations a system can handle in a given time. It is emasured in megabytes per second. Scaling up the server can increase the system's throughput.
3. ### Consistency patterns and availability patterns
    
    __Consistency pattern__  is a property that ensure syncronization within a system by enabling all nodes within the system to see the same data at the time. There are various consistency patterns including:  
    - _Strong consistency_  which ensures that each request gets freshly updated data. This way it peioritizes consistency over availability of the data.  

    - _weak consistency_ which focuses on fast access to data. The data may be fresh or cached.
    - _Eventual balancing_ which prioritize availability of the data and not consistency. After update, data may not be immediately available.
    
    __Availability pattern__ is the proportion of time that the system or  particular service is accessible and operational. There are various availability patterns n system design, they include:
    - _Load balancing_  which involves distributin incoming requests across multiple servers to ensure optimal utilization and availability.  

    - _Retry and timeout strategies_ which ensure availability of resources by retrying making of the request after a specifid interval of time.

## Advanced Concepts of System Design
1. ### Content Delivery Netwwork 
      This is a distributed server network that is used to deliver resources faster, decrease latency, and improves the performance of the system. Resources fro the original server are cached and accessed fro there in the subsequent requests.
2. ### Domain Name System
      Is a distributed naming system for computers resources such as websites. It maps the domain name with a unique IP addres, such that, request ma ethrough that domain name, returns the resource of the respective IP address.
3. ### Caching
      This is a mechanism to store copies of resources in a temporary storage, so that they can be access from their more quickly.
4. ### Proxies
      This is an application that acts as intermediary between the client and the actual server and used for caching resources. Request to the server by the client are made through the proxy.


## Components of System Design
1. ### Microservices and Service Discovery
      Microservices is an architecture style that structures applications as a collection of independent, deployable, and losely coupled services. Each service is identified by a unique ID and name. The ___Service discovery___ provides a platform for the various services to communicate and allow scalability. 
2. ### Database Systems: RDBMS and NoSQL
      A database system is an electronic storage of organized collection of data or informatiion. There are two main categories of databases, they include:
      - **Relational database management system** - which uses _SQL(Structured Query Language)_. They are used to store structured data. They store data in a table format which can only be scaled vertically.  
      
      - **NoSQL** - which stores data in key value pairs and can be scaled horizonatlly. It is used to store unstructured data.
3. ### Communicatioon Protocols

      These are rules that guide the exchange of messages between two system. There are various communication protocols including but not limited to:  
      - HTTP/HTTPS
      - TCP/IP
      - UDP
      - WebSockets

## Steps For Preparing System Design
1. **Requirements Clarification**: The first step for preparing system design for a software is getting to understande the syste requirements. There are two types of requirements:
      - **Function requirements** - These are the features and functions that the system should have. For example, _"User authentication"_,  in a system is a function requirement.
      - **Non-Function requirements** - These are set of specification that describe the system's capabilities and constraints. For exapmle, _"scalability"_ , is a non-function requirement.
2. **Estimation of Resources**: After defining the requirements of the system, the next step is to decide what kind of resources will be used to build the system. For example, considering the amount of requests, you may decide on the number of servers, or even the type of database the system is going to use.

3. **Defining the system interface; describing the API endpoints and what to expect form each API**
4. **Defining the data model and choosing the type of database to be used by the system.**
5. **Analyze the system design to ensure that t meets both the functional and no functional requirements.**
7. **Identify the bottlenecks in the system and discuss the optimal solutions to resolve them**


