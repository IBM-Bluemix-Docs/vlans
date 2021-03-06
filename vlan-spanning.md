---

copyright:
  years: 1994, 2020
lastupdated: "2020-07-20"

keywords: VLAN Spanning

subcollection: vlans

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:codeblock: .codeblock}
{:pre: .pre}
{:screen: .screen}
{:term: .term}
{:tip: .tip}
{:note: .note}
{:important: .important}
{:deprecated: .deprecated}
{:external: target="_blank" .external}
{:table: .aria-labeledby="caption"}
{:generic: data-hd-programlang="generic"}
{:download: .download}
{:DomainName: data-hd-keyref="DomainName"}


# VLAN spanning
{: #vlan-spanning}

VLAN spanning enables all devices on an account to communicate with each other by using the private network, regardless of the devices assigned VLAN.
{: #shortdesc}

## Understanding VLAN spanning
{: #understanding-vlan-spanning}

In {{site.data.keyword.cloud}}, VLAN spanning can be used for many different purposes and has an impact on device communication. To learn more about the basics of VLAN spanning before you get started, review the following information.

### How VLAN spanning works
{: #how-vlan-spanning-works}

By enabling VLAN spanning, all of your routed traffic can travel between all private subnets, across all private VLANs on your account. VLAN spanning serves business needs that require the global communication of your routed traffic. For example, enable VLAN spanning if devices that reside on more than one private subnet need to communicate, whether on the same or different VLANs.

When spanning is enabled, it affects the entire account. You cannot exempt any subnets, VLANs, or devices from VLAN Spanning. If you currently rely solely on private subnets to segregate servers into roles or tiers, enabling VLAN spanning removes that segregation.
{:note}

### Default values
{: #vlan-spanning-default-values}

By default, VLAN spanning is disabled. Devices on two different private subnets, whether on the same or different VLANs, can't send IP traffic to one another.

### Services that commonly require VLAN spanning
{: #vlan-spanning-services}

Specific tutorials are available to help you set up VLAN spanning for your situation. See our links to [Other resources](/docs/vlans?topic=vlans-other-resources-vlan-spanning).


## Managing VLAN spanning
{: #manage-vlan-spanning}

You can enable or disable VLAN spanning for your account.

To update your account setting, follow these steps:

  1. From your browser, open the [{{site.data.keyword.cloud_notm}} console](https://{DomainName}/){: external} and log in to your account.
  1. From the dashboard, click the menu icon ![menu icon](../../icons/icon_hamburger.svg) and select **Classic Infrastructure**.
  1. Select **Network > IP Management > VLANs**.
  1. Select the **VLAN Spanning** tab to access the VLAN Spanning section.
  1. Toggle to **Disabled** or **Enable** as needed to enable or disable VLAN spanning.

Toggling VLAN Spanning within a short amount of time might delay application.
{:note}

The update request can take up to 15 minutes to process. A confirmation of the change shows on the screen. You can update your VLAN spanning settings at any time by repeating the previous steps.
