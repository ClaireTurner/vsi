---

copyright:
  years: 2017, 2019
lastupdated: "2019-09-16"

keywords: transient virtual servers, transient instances, transient offering, cost savings

subcollection: virtual-servers

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:tip: .tip}
{:table: .aria-labeledby="caption"}

# Transient virtual servers
{: #about-vs-transient}
The {{site.data.keyword.BluVirtServers}} transient offering is a good option if you have flexible workloads and want cost savings. You will save money by running your workload on a transient virtual server. Transient instances are provisioned when there is unused capacity available. Therefore, when data center resources are needed for full, on-demand accounts, you can also lose those resources. Transient instances are de-provisioned on a first-on, first-off basis when those resources need to be reclaimed.   

Transient virtual servers offer the following flexibility:

* **Global availability**

    The transient virtual server offering is available in data centers across the globe.

* **Cost savings**

    Transient virtual servers are ideal for non-production workloads. For example, you might use a transient instance to test and develop applications, or test scalability in environments that don't require constant uptime.

Transient instances are public instances that use SAN-backed storage. The following families of public instances are available for this offering.

| Families  | Description                                                                                              |
| ----------------------- | -------------------------------------------------------------------------------------------------------- | 
| [Balanced](/docs/vsi?topic=virtual-servers-about-virtual-server-profiles#balanced) | Best for common cloud workloads that require a balance of performance and scalability. Uses network-attached storage.|
| [Compute](/docs/vsi?topic=virtual-servers-about-virtual-server-profiles#compute) | Best for moderate to high web traffic workloads.|
| [Memory](/docs/vsi?topic=virtual-servers-about-virtual-server-profiles#memory)  | Best for memory caching and real-time analytics workloads. |
{: caption="Table 1. Public virtual server family selections" caption-side="top"}

Network speeds greater than 10 Gbps are achievable through additional configuration. For more information about network performance, see [Configuring virtual server settings for improved network performance](/docs/vsi?topic=virtual-servers-configuring-network-performance).

## Notifications
{: #notifications-transient-virtual-servers}

You can use the {{site.data.keyword.slapi_short}} to receive notifications when resources are available for a transient instance. You can also use the API to programmatically provision a transient virtual server when resources become available. Likewise, you can use the API to programmatically stop provisioning instances when resources become unavailable. For more information, see [Configuring automated reclaim notifications](/docs/vsi?topic=virtual-servers-configuring-notifications-for-reclaims-of-transient-virtual-servers#configuring-notifications-for-reclaims-of-transient-virtual-servers).  

## Limitations
{: #limitations-transient-virtual-servers}

Consider the following limitations before provisioning a transient virtual server.

* The number of supported, concurrent instances are part of your account-wide device quota. For more information about concurrent instance limits, see [FAQ: Virtual servers](/docs/vsi?topic=virtual-servers-faqs-virtual-servers#faqs-virtual-servers).
* Transient instances cannot be upgraded or downgraded.
* Resources can be reclaimed at any time, without notification.
* Transient instances cannot use local storage.
* Transient instances cannot use GPU-based or variable compute profiles.


## Next steps
{: #next-steps-transient-virtual-servers}

After you review and select your virtual server profile, it's time to provision your transient virtual server. To get started, see [Provisioning transient instances](/docs/vsi?topic=virtual-servers-ordering-vs-transient#ordering-vs-transient).

