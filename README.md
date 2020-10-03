# The NextGen Architectural Paradigm for designing "Hyper Scale Secured Resilient Product system"

<img alt="hyperscaler" src="/images/Large-Building-Animation.gif" width="900" height="450"/>

**The Mission & Vision:**
This repo is one step towards my humble pursuit of Democratizing, simplifying & seamslessly oragnizing *very many dynamic and moving dimensions* of "The Architectural Paradigm, constructs & pattern for designing Next Genrartion Product system". Any Enterprise Grade Product design generally comprises of following essential attributes - 

	- 'Hyper-scale' (Auto Scale @ hyper web scale), 
	- 'Distributed & Orachasterated' (CaaS), 
	- 'Modular, Metered, Monitored & Fine-Grained' (uS Governance & management),
	- 'Secured' (Onion layers like Security for Users/APIs/Data/AI/Infra/..),
	- 'Smart' (AI/ML/Ontology powered),
	- 'Resilient',
	- 'Trusted' (Provenance driven),
	- 'Maintainable'
	- 'Consistent deployment powered by DevSecOps',
	- 'Seamless one-click hosting & deployment in any Cloud / On-Prem / Hybrid Cloud Infra', 

Knowing how to design scalable systems will help one become a better architect, and certainly helps in crsytalizing one's **Business idea** take shape at scale.



**The Offering & The Target Audience**
This repository intends to offers

	- A Real-world vision and recipe of the design, development and operationalization of Enterprise grade N-Tier product systems. i.e., principles of scalable system design.
	- A curated list of tools, constructs, frameworks and open source libraries for to build & opertaionize such a comprehensive, operational & production garde system.


Target Audience:
	- Entereprise Architects / Solution Architects
	- Platform Ops Architects & Engineers
	- Microservice Architects & Engineers
	- AI/ML Architects & Engineers
	- DevSecOps, DataOps, MLOps, AIOps Engineers
	
***
**The Foundation:**
Designing & architecting Hyper Scale Secured Resilient N-Tier Product System may appear as daunting as canvassing an Universe itself. There are very many moving dynamic aspects and nuances. This Repo unambiguously tries to simplify the wonderland of Product design. The repo and the asscoiated artefacts is a crux of my
	- deep industry experience of conceptualizing, budiling and operationizing market renowened credible Products in past
	- continuous learning based on ***Real World Architectures*** and Engineering solutions shared with architect community by some of the very establsihed product companies such as ***Airbnb/ NetFlix / Cloudera / LinkedIn Engineering / Pinterest Engineering / Uber Engineering / Walmart Labs Tech Blog / Amazon AWS / Facebook Engineering / Google Research Blogs/ Intel Software Blogs/ Yahoo Engineering*** et al. 
	- Please click on the [Product Company Engineering blogs & Real World Architectures](README_ProductEngineeringArchitectureBlogs_Reference.md), and take a quick holy dip into the same.


Herein, my sincere endeavour is to pamper your journey with Infographics/ panoramic views of the design, the sweeping architectural constructs, and many more such delightful  elements of Next Gen Enterprise grade Product system.
***

## Sattelite view of HyperScale Distributed Resilient Secured Smart PRODUCT design

Welcome Onboard!

<img alt="hyperscaler" src="/images/sattelite_moving.gif" width="900" height="250"/>


This section offers Sattelite view of various dimensions of system design topics. 
> Each section contains links to more in-depth resources. Please click on to venture deep into the topics. 
> Click and traverse the wonduerful space of System Design. 

- Hold on for a Sec! Before we embark the long, arduous, yet-so-entertaining journey to build the **Enterprise-Grade-Product** with Next generation principles of Ssytem Designing., let us take a quick sojourn at the pitstop called - "Product Design Steps - A quick tip". 

- The PitStop : "Product Design Steps - A quick tip" : is all about knowing how to go about when you decide/asked to venture into the Enterprise-Grade-Product-designing trajectory.

[[⬆]](#toc) **PITSTOP: Product Design Steps - A quick tip** 

**Step 1: Clarify the User Personal, constraints and identify the user cases** 

To Deliberate and agreeing on the scope of the system. Gather requirements and scope the problem.  Ask questions to clarify use cases and constraints.  Discuss assumptions.

  
- User Persona Identification::
		* Who is going to use it?
		* How are they going to use it?
		* How many users are there?

- main functions of the system::
		* What does the system do?
		* What are the inputs and outputs of the system?

- and constraints list the scale of the system such as :: 
		* How much data do we expect to handle?
		* How many requests per second do we expect?
		* What is the expected read to write ratio?	
		- requests per second, 
		- requests types, 
		- data written per second, 
		- data read per second, et al.

**Step 2: Outline a High-level architecture design**

Sketch the important components and the connections between them, but don't go into a lot of details. 
Usually, a scalable system includes webserver (load balancer), service (service partition), database (primary/secondary database cluster plug cache).

* Sketch the main components and connections
 
**Step 3: Design Component design**

Dive into details for each core component.  


For example, if you were asked to *"Design a url shortening service"* discuss:

* Generating and storing a hash of the full url
    * [MD5](solutions/system_design/pastebin/README.md) and [Base62](solutions/system_design/pastebin/README.md)
    * Hash collisions
    * SQL or NoSQL
    * Database schema
* Translating a hashed url to the full url
    * Database lookup
* API and object-oriented design

For each component, you need to write the specific APIs for each component. You may need to finish
the detailed OOD design for a particular function. You may also need to design the database schema for the database.


** Step 4: Scale the design

Identify and address bottlenecks, given the constraints.  For example, do you need the following to address scalability issues?

* Load balancer
* Horizontal scaling
* Caching
* Database sharding

***Discuss potential solutions and trade-offs.  Everything is a trade-off.  Address bottlenecks using [The Wonderful Journey : Principles of scalable Product Design](#index-of-product-design-topics).***


[[⬆]](#toc) <a name='index-of-product-design-topics'>**The Wonderful Journey : Principles of scalable Product Design**</a>  

* [System design topics: start here](#system-design-topics-start-here)
    * [Step 1: Review the scalability video lecture](#step-1-review-the-scalability-video-lecture)
    * [Step 2: Review the scalability article](#step-2-review-the-scalability-article)
    * [Next steps](#next-steps)
* [Performance vs scalability](#performance-vs-scalability)
* [Latency vs throughput](#latency-vs-throughput)
* [Availability vs consistency](#availability-vs-consistency)
    * [CAP theorem](#cap-theorem)
        * [CP - consistency and partition tolerance](#cp---consistency-and-partition-tolerance)
        * [AP - availability and partition tolerance](#ap---availability-and-partition-tolerance)
* [Consistency patterns](#consistency-patterns)
    * [Weak consistency](#weak-consistency)
    * [Eventual consistency](#eventual-consistency)
    * [Strong consistency](#strong-consistency)
* [Availability patterns](#availability-patterns)
    * [Fail-over](#fail-over)
    * [Replication](#replication)
    * [Availability in numbers](#availability-in-numbers)
* [Domain name system](#domain-name-system)
* [Content delivery network](#content-delivery-network)
    * [Push CDNs](#push-cdns)
    * [Pull CDNs](#pull-cdns)
* [Load balancer](#load-balancer)
    * [Active-passive](#active-passive)
    * [Active-active](#active-active)
    * [Layer 4 load balancing](#layer-4-load-balancing)
    * [Layer 7 load balancing](#layer-7-load-balancing)
    * [Horizontal scaling](#horizontal-scaling)
* [Reverse proxy (web server)](#reverse-proxy-web-server)
    * [Load balancer vs reverse proxy](#load-balancer-vs-reverse-proxy)
* [Application layer](#application-layer)
    * [Microservices](#microservices)
    * [Service discovery](#service-discovery)
* [Database](#database)
    * [Relational database management system (RDBMS)](#relational-database-management-system-rdbms)
        * [Master-slave replication](#master-slave-replication)
        * [Master-master replication](#master-master-replication)
        * [Federation](#federation)
        * [Sharding](#sharding)
        * [Denormalization](#denormalization)
        * [SQL tuning](#sql-tuning)
    * [NoSQL](#nosql)
        * [Key-value store](#key-value-store)
        * [Document store](#document-store)
        * [Wide column store](#wide-column-store)
        * [Graph Database](#graph-database)
    * [SQL or NoSQL](#sql-or-nosql)
* [Cache](#cache)
    * [Client caching](#client-caching)
    * [CDN caching](#cdn-caching)
    * [Web server caching](#web-server-caching)
    * [Database caching](#database-caching)
    * [Application caching](#application-caching)
    * [Caching at the database query level](#caching-at-the-database-query-level)
    * [Caching at the object level](#caching-at-the-object-level)
    * [When to update the cache](#when-to-update-the-cache)
        * [Cache-aside](#cache-aside)
        * [Write-through](#write-through)
        * [Write-behind (write-back)](#write-behind-write-back)
        * [Refresh-ahead](#refresh-ahead)
* [Asynchronism](#asynchronism)
    * [Message queues](#message-queues)
    * [Task queues](#task-queues)
    * [Back pressure](#back-pressure)
* [Communication](#communication)
    * [Transmission control protocol (TCP)](#transmission-control-protocol-tcp)
    * [User datagram protocol (UDP)](#user-datagram-protocol-udp)
    * [Remote procedure call (RPC)](#remote-procedure-call-rpc)
    * [Representational state transfer (REST)](#representational-state-transfer-rest)
* [Security](#security)
* [FAQ on System Design](#README_ProductEngineeringArchitectureBlogs_Reference.md)
* [Credits](#credits)
* [Contact info](#contact-info)
* [License](#license)

## Real world N-Tier Product Architectural Panoramic view
<br/>

***Real world N-Tier Product Architectural - High level Architectural constructs***
<br/>
<br/>
<p align="center">
  <img src="images/jj3A5N8.png">
  <br/>
</p>

<br/>

***Real world N-Tier Product Architectural - Mid level Architectural constructs***
<br/>
<br/>

<p align="center">
  <img src="images/jrUBAF7.png">
  <br/>
</p>


<br/>

***Real world N-Tier Product Architectural - Low level Architectural constructs:***
<br/>
<br/>
Please refer to the above Section [Detailed Stop : Principles of scalable Product Design](#index-of-product-design-topics).


## Contact info

Feel free to contact me to discuss any issues, questions, or comments.

My contact info can be found on my [GitHub page](https://github.com/DeepHiveMind).

## License

*I, The DeepHiveMind, am providing code and resources in this repository to you under custom Copyright & license (Copyright 2020 DeepHiveMind & Creative Commons Legal Code CC0 1.0 Universal). Please Refer to the License for further details as to this. Thanks!
