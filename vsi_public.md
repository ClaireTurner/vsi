---

copyright:
  years: 2017, 2019
lastupdated: "2019-09-16"

keywords: public virtual servers, network traffic, virtual server deployment

subcollection: virtual-servers

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Public virtual servers
{: #about-public-virtual-servers}

The public {{site.data.keyword.BluVirtServers}} offerings are IBM-managed, multi-tenant virtual server deployments. They give you rapid scalability and higher-cost effectiveness with pre-defined sizes that meet all business requirements to get you up and running quickly.
{:shortdesc}

Public virtual servers have many advantages, including the following:

* **Global availability** 

    The public virtual server offering is available in data centers across the globe.

* **Configuration choices, rapid deployment, and scalability** 

    The public virtual server offering gives you small or large virtual server options to meet various workload requirements.

Network traffic for public virtual servers, which encompasses virtual server instance SAN and other network-attached storage, has no guarantee. If network traffic of a virtual server instance begins to have a significant, negative impact on other virtual servers, that instance might be restarted on a new host, or in extreme cases, completely disabled. This negative impact is often observed as traffic levels approach 20,000 to 30,000 packets per second (PPS).  For guaranteed networking, use of the Dedicated Virtual Server offering is recommended. For more information, see the single-tenant environment, [Dedicated virtual server](/docs/vsi?topic=virtual-servers-about-dedicated-virtual-servers#about-dedicated-virtual-servers) offering.

The following families of public instances are available for this offering. 

| Families  | Description                                                                                              |
| ----------------------- | -------------------------------------------------------------------------------------------------------- | 
| [Balanced](/docs/vsi?topic=virtual-servers-balanced#balanced) | Best for common cloud workloads that require a balance of performance and scalability. Uses network-attached storage. |
| [Balanced local storage](/docs/vsi?topic=virtual-servers-balanced-local-storage#balanced-local-storage) | Best for large database workloads that require high I/O performance with very low latency. |
| [Variable compute](/docs/vsi?topic=virtual-servers-about-virtual-server-profiles#variable-compute)  | Best for workloads that don’t require steady, high-CPU performance. | 
| [Compute](/docs/vsi?topic=virtual-servers-compute#compute) | Best for moderate to high web traffic workloads.|
| [Memory](/docs/vsi?topic=virtual-servers-memory#memory)  | Best for memory caching and real-time analytics workloads. |
| [GPU](/docs/vsi?topic=virtual-servers-gpu#gpu)  | Best for high-performance workloads.
{: caption="Table 1. Public virtual server family selections" caption-side="top"}

Network speeds greater than 10 Gbps are achievable through additional configuration. For more information about network performance, see [Configuring virtual server settings for improved network performance](/docs/vsi?topic=virtual-servers-configuring-network-performance).

Some of these families are also available for {{site.data.keyword.vsi_is_full}}. For more information, see [{{site.data.keyword.vsi_is_short}}](/docs/vpc-on-classic-vsi?topic=vpc-on-classic-vsi-getting-started#gettingstartedvsigen).
{:tip}

## Next steps
{: #next-steps-public-virtual-servers}

After you review and decide upon your virtual server profile, it's time to provision your public virtual server. To get started, see [Provisioning public instances](/docs/vsi?topic=virtual-servers-ordering-vs-public#ordering-vs-public).
