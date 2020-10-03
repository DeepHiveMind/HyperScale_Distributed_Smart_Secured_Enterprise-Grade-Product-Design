# Sub-topic of The NextGen Architectural Paradigm for designing "Hyper Scale Secured Resilient Product system"

**Reverse proxy web server**
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
    * [Load balancer vs reverse proxy](#load-balancer-vs-reverse-proxy)
```

<img alt="hyperscaler" src="/images/sattelite_moving.gif" width="900" height="250"/>


## Reverse proxy (web server)

<p align="center">
  <img src="images/n41Azff.png">
  <br/>
  <i><a href=https://upload.wikimedia.org/wikipedia/commons/6/67/Reverse_proxy_h2g2bob.svg>Source: Wikipedia</a></i>
  <br/>
</p>

A reverse proxy is a web server that centralizes internal services and provides unified interfaces to the public.  Requests from clients are forwarded to a server that can fulfill it before the reverse proxy returns the server's response to the client.

### Additional benefits of Reverse proxy web server :

* **Increased security** - Hide information about backend servers, blacklist IPs, limit number of connections per client
* **Increased scalability and flexibility** - Clients only see the reverse proxy's IP, allowing you to scale servers or change their configuration
* **SSL termination** - Decrypt incoming requests and encrypt server responses so backend servers do not have to perform these potentially expensive operations
    * Removes the need to install [X.509 certificates](https://en.wikipedia.org/wiki/X.509) on each server
* **Compression** - Compress server responses
* **Caching** - Return the response for cached requests
* **Static content** - Serve static content directly
    * HTML/CSS/JS
    * Photos
    * Videos
    * Etc

### Load balancer vs reverse proxy

* Deploying a load balancer is useful when you have multiple servers.  Often, load balancers  route traffic to a set of servers serving the same function.
* Reverse proxies can be useful even with just one web server or application server, opening up the benefits described in the previous section.
* Solutions such as NGINX and HAProxy can support both layer 7 reverse proxying and load balancing.

### Disadvantage(s): reverse proxy

* Introducing a reverse proxy results in increased complexity.
* A single reverse proxy is a single point of failure, configuring multiple reverse proxies (ie a [failover](https://en.wikipedia.org/wiki/Failover)) further increases complexity.

### Source(s) and further reading

* [Reverse proxy vs load balancer](https://www.nginx.com/resources/glossary/reverse-proxy-vs-load-balancer/)
* [NGINX architecture](https://www.nginx.com/blog/inside-nginx-how-we-designed-for-performance-scale/)
* [HAProxy architecture guide](http://www.haproxy.org/download/1.2/doc/architecture.txt)
* [Wikipedia](https://en.wikipedia.org/wiki/Reverse_proxy)



## Contact info

Feel free to contact me to discuss any issues, questions, or comments.

My contact info can be found on my [GitHub page](https://github.com/DeepHiveMind).

## License

I, *The DeepHiveMind*, am providing code and resources in this repository to you under custom Copyright & license (Copyright 2020 DeepHiveMind & Creative Commons Legal Code CC0 1.0 Universal). Please Refer to the [Copyright 2020 DeepHiveMind License](https://github.com/DeepHiveMind/HyperScale_Distributed_Smart_Secured_Enterprise-Grade-Product-Design/blob/main/LICENSE) for further details as to this. Thanks!
