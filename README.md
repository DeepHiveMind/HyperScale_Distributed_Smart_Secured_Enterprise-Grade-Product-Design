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



**The Offering & The Target Audience:**

This repository intends to offers

	- A Real-world vision and recipe of the design, development and operationalization of Enterprise grade N-Tier product systems. i.e., principles of scalable system design.
	- A curated list of tools, constructs, frameworks and open source libraries for to build & opertaionize such a comprehensive, operational & production garde system.

Essence of the Offering: 
- [The Wonderful Journey : Principles of scalable Product Design](#index-of-product-design-topics)
- [The PitStop : "Product Design Steps - A quick tip"](#pitstop)

Target Audience:: 
	
	- Entereprise Architects, Principal Solution Architects | 
	- Platform Ops Architects & Engineers | 
	- Microservice Architects & Engineers | 
	- AI/ML Architects & Engineers | 
	- DevSecOps, DataOps, MLOps, AIOps Engineers | 
	

**The Foundation:**

Designing & architecting Hyper Scale Secured Resilient N-Tier Product System may appear as daunting as canvassing an Universe itself. There are very many moving dynamic aspects and nuances.
This Repo unambiguously tries to simplify the wonderland of Product design. The repo and the asscoiated artefacts is based on the crux of my

- deep industry experience of conceptualizing, budiling and operationizing market renowened credible Products in past.
- continuous learning and surfing of ***Real World Architectures*** and Engineering solutions shared with architect community by some of the very establsihed product companies such as ***Airbnb/ NetFlix / Cloudera / LinkedIn Engineering / Pinterest Engineering / Uber Engineering / Walmart Labs Tech Blog / Amazon AWS / Facebook Engineering / Google Research Blogs/ Intel Software Blogs/ Yahoo Engineering*** et al. 
- Please click on the [Product Company Engineering blogs & Real World Architectures](README_ProductEngineeringArchitectureBlogs_Reference.md), and take a quick holy dip into the same.
<br/>
Herein, my sincere endeavour is to pamper your journey with Infographics/ panoramic views of the design, the sweeping architectural constructs, and many more such delightful  elements of Next Gen Enterprise grade Product system.

<br/>
<br/>

## Sattelite view of HyperScale Distributed Resilient Secured Smart PRODUCT design

Welcome Onboard!

<img alt="hyperscaler" src="/images/sattelite_moving.gif" width="900" height="250"/>


This section offers Sattelite view of various dimensions of system design topics. 
> Each section contains links to more in-depth resources. Please click on to venture deep into the topics. 
> Click and traverse the wonduerful space of System Design. 

- Hold on for a Sec! Before we embark the long, arduous, yet-so-entertaining-&-wonderful journey to build the **Enterprise-Grade-Product** with Next generation principles of Ssytem Designing, let us take a quick sojourn at the pitstop called - "Product Design Steps - A quick tip". 

- The PitStop : "Product Design Steps - A quick tip" : is all about knowing how to go about when you decide/asked to venture into the Enterprise-Grade-Product-designing trajectory.

<br/>

[[⬆]](#toc) <a name='pitstop'>**PITSTOP: Product Design Steps - A quick tip**</a> 
<br/>

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

For each component, design to write the specific APIs for each component. One may need to finish
the detailed OOD design for a particular function. You may also need to design the database schema for the database.

```
For example, if you were asked to *"Design a url shortening service"* discuss:
* Generating and storing a hash of the full url
    * [MD5] and [Base62]
    * Hash collisions
    * SQL or NoSQL
    * Database schema
* Translating a hashed url to the full url
    * Database lookup
* API and object-oriented design
```




**Step 4: Scale the design**

Identify and address bottlenecks, given the constraints.  For example, do you need the following to address scalability issues?

* Load balancer
* Horizontal scaling
* Caching
* Database sharding

*Discuss potential solutions and trade-offs.  Everything is a trade-off.  Address bottlenecks using [The Wonderful Journey : Principles of scalable Product Design](#index-of-product-design-topics).*

<br/>

[[⬆]](#toc) <a name='index-of-product-design-topics'>**The Wonderful Journey : Principles of scalable Product Design**</a>  

* [Product design topics: KickOff](https://github.com/DeepHiveMind/HyperScale_Distributed_Smart_Secured_Enterprise-Grade-Product-Design/blob/main/README_Product_System_design_KickOff.md)
```
    * Load balancing
    * Asynchronism
    * Caching
	* Cloning (Server/Pod/Container replication)
	* Vertical scaling
    * Horizontal scaling
    * Database replication
    * Database partitioning
	* Performance vs scalability]
	* Latency vs throughput
	* Availability vs consistency
		* CAP theorem
			* CP - consistency and partition tolerance
			* AP - availability and partition tolerance
	* Consistency patterns
		* Weak consistency
		* Eventual consistency
		* Strong consistency
	* Availability patterns
		* Fail-over
			* Active-active
			* Active-passive
		* Replication
			* Master-slave replication
			* Master-master replication
		* Availability in numbers
			* 99.9% availability - three 9s
			* 99.99% availability - four 9s
			* Availability in parallel vs in sequence
```
* [Domain name system](https://github.com/DeepHiveMind/HyperScale_Distributed_Smart_Secured_Enterprise-Grade-Product-Design/blob/main/README_Product_System_design_CDN.md)
```
	* DNS Servers Attribute
		* Name server
		* Mail exchange
		* Address
		* Canonical
	* Managed DNS Service
		* CloudFare 
		* AWS Route 53
		* Azure DNS
		* GCP Cloud DNS
	* DNS- Traffic routing methods
		* Weighted round robin
			* Prevent traffic from going to servers under maintenance
			* Balance between varying cluster sizes
			* A/B testing
		* Latency-based (routing-policy-latency)
		* Geolocation-based (routing-policy-geo)
```
* [Content delivery network](https://github.com/DeepHiveMind/HyperScale_Distributed_Smart_Secured_Enterprise-Grade-Product-Design/blob/main/README_Product_System_design_CDN.md)
```
    * Push CDNs
    * Pull CDNs
	* Good fit use case for Pull CDN
	* Good fit use case for Push CDN
```
* [Load balancer](https://github.com/DeepHiveMind/HyperScale_Distributed_Smart_Secured_Enterprise-Grade-Product-Design/blob/main/README_Product_System_design_Load-balancer.md)
```
	* Additional benefits of LB
		* SSL termination (Removes the need to install X.509 certificates)
		* Session persistence
	* Load Balancer - Route Traffic Method
		* Random
		* Least loaded
		* Session/cookies
		* Round robin or weighted round robin
		* Layer 4 load-balancing
		* Layer 7 load-balancing
	* Load Balancing Layers
		* Layer 4 load balancing(Transport Layer)
		* Layer 7 load balancing(Application Layer)
```
* [Reverse proxy (web server)](https://github.com/DeepHiveMind/HyperScale_Distributed_Smart_Secured_Enterprise-Grade-Product-Design/blob/main/README_Product_System_design_Reverse-proxy-web-server.md)

```
	* Additional benefits of Reverse proxy web server 
		* Increased security
		* Increased scalability and flexibility
		* SSL termination (Removes the need to install X.509 certificates on each server)
		* Compression
		* Caching
		* Direct serving of Static content
			* HTML/CSS/JS
			* Photos
			* Videos
			* Etc
    * Load balancer vs reverse proxy
```
* [Application layer Microservices](https://github.com/DeepHiveMind/HyperScale_Distributed_Smart_Secured_Enterprise-Grade-Product-Design/blob/main/README_Product_System_design_ApplicationMicroservice.md)
```
	* Microservices Overview
		* Service Discovery
		* Service Discovery Health Check
		*  Service Discovery common Tooling
			* Etcd / Consul / Zookeeper
			* Health check
		* Service Communication Protocols
			* Hypertext transfer protocol (HTTP protocol) 
				* Common HTTP verbs
			* Transmission control protocol (TCP protocol)
			* User datagram protocol (UDP protocol)
			* Use TCP over UDP when
			* Use UDP over TCP when
			* Remote procedure call protocol (RPC protocol)
				* Popular RPC frameworks 
					* Protobuf
					* Thrift
					* Avro
				* RPC Protocols elements
					* Client program
					* Client stub procedure
					* Client communication module
					* Server communication module
					*Server stub procedure 
				* Sample RPC calls
				* Disadvantage(s): RPC
			* REST architectural style Protocol (REST Protocol)	
				* Qualities of RESTful interface
				* Sample REST calls
				* Disadvantage(s): REST
			* RPC and REST protocols calls comparison
		* Service Communication Types - Synchronous &  Asynchronism
			* Asynchronism
			* Asynchronism Technique - Message queues Technique
				* Message queues Tooling
					* Redis
					* RabbitMQ
					* KubeMQ
					* Amazon SQS
			* Asynchronism Technique - Task queues Technique
				* Task queues Tooling
					* Celery
			* Asynchronism Technique - RPC / gRPC Technique
			* Asynchronism Technique - Callback Technique
			* Asynchronism Technique - asyncio (async & await) Technique
			* Asynchronism - Back pressure
			* Disadvantage(s): asynchronism
		* Disadvantage(s): application layer Microservice
```
* [Cache](https://github.com/DeepHiveMind/HyperScale_Distributed_Smart_Secured_Enterprise-Grade-Product-Design/blob/main/README_Product_System_design_Caching.md)
```
	* Cache Overview
	* Caching location
		* Client caching
		* CDN caching
		* Web server caching
		* Database caching
		* Application caching
    * Caching level
		* Caching at the database query level
		* Caching at the object level
	* Suggestions of what to cache
    * When to update the cache
	* Cache update strategy
        * Cache strategy: Cache-aside
			* Disadvantage(s): cache-aside
        * Cache strategy: Write-through
			* Disadvantage(s): write through
        * Cache strategy: Write-behind (write-back)
			* Disadvantage(s): Write-behind
        * Cache strategy: Refresh-ahead
			* Disadvantage(s): refresh-ahead
	* Disadvantage(s): Cache
```
* [Database](https://github.com/DeepHiveMind/HyperScale_Distributed_Smart_Secured_Enterprise-Grade-Product-Design/blob/main/README_Product_System_design_Database.md)
```
	* Database Overview
    * NoSQL DB Overview
	* NoSQL DB Propoerties
		* BASE 
			* Basically available
			* Soft state
			* Eventual consistency
		* BASE vis-a-vis CAP
	* NoSQL DB Types
        * Key-value store
			* Key-value store: Best Fit use case
        * Document store
			* Document store: Best Fit use case
        * Wide-column store
			* Wide-column store: Best Fit use case
        * Graph Database
			* Graph store: Best Fit use case
	*  SQL or NoSQL
		* Reasons for **SQL**
		* Reasons for **NoSQL**
		* Sample data well-suited for NoSQL
			* clickstream and log data
			* requently accessed ('hot') data
			* Temporary data
			* Leaderboard or scoring data
			* Metadata/lookup tables data
	* Relational database management system (RDBMS Overview)
	* RDBMS DB Properties
		* ACID
	* RDBMS DB Scaling Techniques
        * Master-slave replication
        * Master-master replication
        * Federation
        * Sharding
        * Denormalization
        * SQL tuning]
		* Tighten up the schema
		* Use good indices
		* Avoid expensive joins
		* Partition tables
		* Tune the query cache
```
* [Security](https://github.com/DeepHiveMind/HyperScale_Distributed_Smart_Secured_Enterprise-Grade-Product-Design/blob/main/README_Product_System_design_Security.md)
* [FAQ on System Design](https://github.com/DeepHiveMind/HyperScale_Distributed_Smart_Secured_Enterprise-Grade-Product-Design/blob/main/README_ProductEngineeringArchitectureBlogs_Reference.md)
* [Contact info](#contact-info)
* [License](#license)

## Real world N Tier Product Architectural Panoramic view
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
Please refer to the above Section [The Wonderful Journey : Principles of scalable Product Design](#index-of-product-design-topics).


## Contact info

Feel free to contact me to discuss any issues, questions, or comments.

My contact info can be found on my [GitHub page](https://github.com/DeepHiveMind).

## License

I, *The DeepHiveMind*, am providing code and resources in this repository to you under custom Copyright & license (Copyright 2020 DeepHiveMind & Creative Commons Legal Code CC0 1.0 Universal). Please Refer to the [Copyright 2020 DeepHiveMind License](https://github.com/DeepHiveMind/HyperScale_Distributed_Smart_Secured_Enterprise-Grade-Product-Design/blob/main/LICENSE) for further details as to this. Thanks!
