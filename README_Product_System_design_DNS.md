# Sub-topic of The NextGen Architectural Paradigm for designing "Hyper Scale Secured Resilient Product system"

**Domain name system**
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

<img alt="hyperscaler" src="/images/Large-Building-Animation.gif" width="900" height="450"/>



## Domain name system

<p align="center">
  <img src="images/IOyLj4i.jpg">
  <br/>
  <i><a href=http://www.slideshare.net/srikrupa5/dns-security-presentation-issa>Source: DNS security presentation</a></i>
</p>

A Domain Name System (DNS) translates a domain name such as www.example.com to an IP address.

DNS is hierarchical, with a few authoritative servers at the top level.  Your router or ISP provides information about which DNS server(s) to contact when doing a lookup.  Lower level DNS servers cache mappings, which could become stale due to DNS propagation delays.  DNS results can also be cached by your browser or OS for a certain period of time, determined by the [time to live (TTL)](https://en.wikipedia.org/wiki/Time_to_live).

#### DNS Servers Attribute
* **NS record (name server)** - Specifies the DNS servers for your domain/subdomain.
* **MX record (mail exchange)** - Specifies the mail servers for accepting messages.
* **A record (address)** - Points a name to an IP address.
* **CNAME (canonical)** - Points a name to another name or `CNAME` (example.com to www.example.com) or to an `A` record.

#### Managed DNS Service
Services such as 
- [CloudFlare](https://www.cloudflare.com/dns/) and 
- [Route 53](https://aws.amazon.com/route53/) provide managed DNS services.  

#### DNS- traffic routing methods
Some DNS services can route traffic through various methods:

* [Weighted round robin](https://www.g33kinfo.com/info/round-robin-vs-weighted-round-robin-lb)
    * Prevent traffic from going to servers under maintenance
    * Balance between varying cluster sizes
    * A/B testing
* [Latency-based](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy.html#routing-policy-latency)
* [Geolocation-based](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy.html#routing-policy-geo)

### Disadvantage(s): DNS

* Accessing a DNS server introduces a slight delay, although mitigated by caching described above.
* DNS server management could be complex and is generally managed by [governments, ISPs, and large companies](http://superuser.com/questions/472695/who-controls-the-dns-servers/472729).
* DNS services have recently come under [DDoS attack](http://dyn.com/blog/dyn-analysis-summary-of-friday-october-21-attack/), preventing users from accessing websites such as Twitter without knowing Twitter's IP address(es).

### Source(s) and further reading

* [DNS architecture](https://technet.microsoft.com/en-us/library/dd197427(v=ws.10).aspx)
* [Wikipedia](https://en.wikipedia.org/wiki/Domain_Name_System)
* [DNS articles](https://support.dnsimple.com/categories/dns/)




## Contact info

Feel free to contact me to discuss any issues, questions, or comments.

My contact info can be found on my [GitHub page](https://github.com/DeepHiveMind).

## License

I, *The DeepHiveMind*, am providing code and resources in this repository to you under custom Copyright & license (Copyright 2020 DeepHiveMind & Creative Commons Legal Code CC0 1.0 Universal). Please Refer to the [Copyright 2020 DeepHiveMind License](https://github.com/DeepHiveMind/HyperScale_Distributed_Smart_Secured_Enterprise-Grade-Product-Design/blob/main/LICENSE) for further details as to this. Thanks!