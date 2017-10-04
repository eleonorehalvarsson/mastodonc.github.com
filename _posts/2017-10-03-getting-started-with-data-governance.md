---
layout: post
title: Getting Started With Data Governance
date: 2017-10-03
author: bruce
comments: true
categories: [Witan]
---

Data governance is about giving your people and partners timely but compliant access to data. Whether it’s driving collaboration across departments or engaging external suppliers, an effective approach to data governance gives you control over data access and usage, whilst making sure you stay on the right side of policy, regulations and the law. All whilst being able to prove that you’re doing it right. With new regulations like [GDPR](https://en.wikipedia.org/wiki/General_Data_Protection_Regulation) making jail sentences possible penalties for data owners, that’s more important than ever.

<!--more-->

This article looks at ways that organisations can make data governance easier by using techniques that get data to the people that need it, in a safe, secure and "provably" legal way.

But it’s not just about keeping everything above board. Adopting these approaches will help you build an effective data infrastructure that gets data out of silos, and gets colleagues and partners working collaboratively to solve problems, build new products and generate new insights.

<!--HubSpot Call-to-Action Code --><span class="hs-cta-wrapper" id="hs-cta-wrapper-2d5848d9-00d4-4807-8040-ee03471d6f27"><span class="hs-cta-node hs-cta-2d5848d9-00d4-4807-8040-ee03471d6f27" id="hs-cta-2d5848d9-00d4-4807-8040-ee03471d6f27"><!--[if lte IE 8]><div id="hs-cta-ie-element"></div><![endif]--><a href="https://cta-redirect.hubspot.com/cta/redirect/3461032/2d5848d9-00d4-4807-8040-ee03471d6f27"  target="_blank" ><img class="hs-cta-img" id="hs-cta-img-2d5848d9-00d4-4807-8040-ee03471d6f27" style="border-width:0px;" src="https://no-cache.hubspot.com/cta/default/3461032/2d5848d9-00d4-4807-8040-ee03471d6f27.png"  alt="Download a free checklist: Getting a Data Project Started"/></a><!-- end HubSpot Call-to-Action Code -->

## The two sides of "provable" data governance

There are two organisational roles your data governance approach needs to consider:

* **Data Users** - people who need to access, use and share data.

* **Data Auditors & Stewards** - the person or people who oversee both how data is used and who ensure and demonstrate compliance with organisational policies, external regulations and the law.

Data governance needs to address critical questions for each of these roles:

* For the **Data User**

    * are they getting the correct data?

    * are they allowed to use it now for this purpose?

* For the **Data Auditor** or **Data Steward**

    * is the correct data being used for specific purposes

    * can they show that the data was being used correctly.

    * can they show that data usage conforms to legal and policy requirements

    * When things go wrong can they provide a clear audit of data access, usage and permissions?

Whilst some of these questions aren’t new [The Data Governance Institute](https://href.li/?http://www.datagovernance.com/) talks about a "Post-Compliance Paradigm Shift,"

"A change in expectations that says that it’s no longer acceptable to simply 'do' work. Instead, for work that exists in an environment with compliance requirements, the work is not complete until you 1. Do it, 2. Control it, 3. Document it, and 4. Prove compliance.”

The implications of this paradigm shift are clear for any organisation using data - to prove compliance you need both control and documentation of data. This requires a practical and systematic approach to data governance that considers the different perspectives of **Data Users** and **Data Auditors**/**Data Stewards**.

## How should your Data Governance Approach Manage Data Users?

The primary goal of the data user or data consumer is to get access to the correct data to allow them to accomplish their goals. Your data governance system should help with this in a number of ways:

* **Using metadata on data files.** This gives users ways to find data for the correct geography, time and spatial and temporal resolutions.

* **Creating descriptions on files** to help them to understand the rich context in which the data has been created and whether or not there are any issues (methodological, regulatory or others) with using the data.

* **Identifying who the owners and maintainers are** and when the data was uploaded or helps them to understand who the data is from and allows them to contact the maintainers or creators of the data in case of questions or if they need access.

* **Offering "datapacks" to allow users to get a package of data that has been put together by another user, often an expert, to accomplish a particular task.** This curation means that a human has said “this grouping of data is appropriate for a particular projection or piece of analysis”. The description and other metadata on the Datapack can help to determine this.

* **Demonstrating the extent of immutability of data in the system - in particular that data found at a particular location will *never change*.** This means that a user can always go back to a particular file and re-do an analysis or develop a product without worrying that the data has changed underneath them in an unexpected way.

* **Enabling repeatability by being able to add scripts or other analysis and the output of analysis to Datapacks.** This allows inputs, code, and outputs to live together as a repeatable bundle.

## How should Your Data Governance Approach Support Data Audits and Data Stewardship?

The primary goal of the data steward is to make sure that data is being provably used in an appropriate and legal way. This requires flexible and robust access controls and an audit trail of what was done with a particular resource.  A data governance system should therefore include

* **Access controls that allow users to share data with individuals or with particular groups appropriately.** For example the adult social care department of a local authority might want to share data internally and with external partners in order to [create plans or commission services](http://www.mastodonc.com/data%20science/send/asc/witan/2017/09/05/demand-projection-send-asc.html).  In this example access controls will need to be fine grained enough to allow users to see the data they need - for example external partners may only need to see metadata, internal partners will need see both the file and metadata, and specific team members will need to be see the file, edit the metadata and manage sharing. In this way your data governance system will allow users to appropriately delegate authority to other users.

* **When a user gets access to data, all access (edits, uploads, changes to metadata and sharing) are stored should form an audit trail.** Seeing that data was shared with a particular user for a short period of time, the file was accessed and downloaded, and then the sharing was changed is possible to see as a complete event log of all actions is stored in the system for this analysis.

* **Data can curated into Datapacks**.  Again when there descriptions on each file and on the Datapack itself that describe how data can be appropriately used, users won’t attempt to use data in ways that would be misleading, inappropriate or illegal.

## **Taking the next steps with data governance tools**

To make data both a useful asset for your organisation, whilst sticking to the rules, your data governance system and processes need to be able to support the key principles of data governance - using metadata, creating data packs, ensuring the immutability of data, and preserving the immutability of events for all things.

For smaller organisations this could potentially be a manual process, but for larger ones the task will need systems and tools. The question then becomes how do I ensure that my systems and tools are up to the job?  This is where you may want consider technology that has been specifically designed to do data governance effectively - tools like [Witan Datastore](http://www.mastodonc.com/products/witan/) and systems from SAS and Hortonworks have been been designed to make data governance fast and effective.

If you adopt the data governance principles we’ve described, and oversee everything with an efficient system, you’ll be a long way towards making sure data is used effectively and securely in your organisation.

Your data users will be able find the data they need and be confident that they are allowed to use it in their circumstances, and that it won’t change without their knowledge. Data stewards and producers can be confident that their data is only being shared with whom they intend to and that if they need to they can show a trail of how the data they have in the system was used. And you’ll have the foundations for turning data into a resource that offers you exciting opportunities.
