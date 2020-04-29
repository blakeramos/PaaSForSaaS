# Oracle’s Cloud Platform: Transform and Extend Oracle ERP Cloud

<!-- Comment out table of contents
## Table of Contents
[Introduction](#introduction)
-->

## Introduction

*Complete Cloud Portfolio:*

Oracle Cloud is a Generation 2 enterprise cloud that delivers powerful compute and networking performance and includes a comprehensive portfolio of infrastructure and platform cloud services. Built from the ground up to meet the needs of mission-critical applications, Oracle Cloud supports all legacy workloads while delivering modern cloud development tools, enabling enterprises to bring their past forward as they build their future. Our Generation 2 Cloud is the only one built to run Oracle Autonomous Database, the industry's first and only self-driving database. Oracle Cloud offers a comprehensive cloud computing portfolio, from application development and business analytics to data management, integration, security, artificial intelligence (AI), and blockchain.

The Oracle Cloud platform-as-a-service (PaaS) portfolio is comprehensive and standards-based, and built on Oracle and open-source technologies that integrate with your existing applications, regardless of origin. Machine learning, artificial intelligence, and security are built in, meaning you can self-secure and repair, giving you more time to build and deploy. It is architected to detect and defend against modern threats, so you can innovate more. Combine low cost with high performance to lower your TCO. Oracle's PaaS portfolio can be integrated with Oracle SaaS. For example, it can be integrated with ERP Financials, Procurement, and more, you can increase productivity, lower costs, and improve controls. 

This is the first of several labs that are part of the **Oracle’s PaaS for SaaS** workshop. This workshop will walk you through the process of using: 
- Oracle Analytics for Applications (OAX) and a sub-set of the 50+ out-of-the-box financial KPIs and 25+ benchmark finance dashboards. 
- Oracle Digital Assistant (ODA) prebuilt AI trained skills for ERP Cloud.
- Oracle Integration Cloud (OIC) and Autonomous Datawarehouse (ADW) to process additional orders and store information from ERP cloud in a separate database for long term retention and analytics.
- Oracle Identity Cloud Service (IDCS) and Cloud Access Security Broker (CASB) to centralize an enterprise's user store and enable fraudulent behavior detection. 

You will take on 5 Personas during the workshop. Overall, the majority of the workshop will revolve around the **Finance Manager**. The Finance Manager will be relying on OAX's prebuilt models and visuals to collaborate with the **Business Analyst** on ways to better their account payable ratio. The Finance Manager will then leverage Oracle's Digital Assistant to submit expenses and get updates on his accounts. The company's **New Hire** will then complete a few on-boarding tasks such as procuring a laptop and business cards through ODA. Next, the Finance Manager and a **Customer** needs to be able to process additional orders and store information from ERP cloud in a separate Database for long term retention and analytics. Lastly, the Finance Manager is having difficulty accessing the appropriate documents. The **Application Security Architect** will grant the Finance Manager access to ERP Financials and setup a policy to detect fraudulent behavior. 

During the workshop, you will get exposure to Oracle Analytics for Applications (OAX), Oracle Digital Assistant (ODA), Oracle Autonomous Data Warehouse (ADW), Oracle Integration Cloud (OIC), Oracle Identity Cloud Service (IDCS), and Oracle Cloud Access Security Broker (CASB). 

To get an idea of how these services correlate to one another, here is an example of the PaaSForSaaS Architecture which can be extended with other Oracle SaaS or Oracle PaaS:

![](./images/na.jpg " ")

**Note**: This lab is intended to be a subset of the full PaaSForSaaS showcase. As such, it is assumed a user going through this workshop will be provisioning resources and creating users from scratch. If you decide to use existing infrastructure or resources, be aware and keep note of your namings so resources don't overlap and conflict. 

**Note**: Additionally, as much as possible, do not stray away from the naming conventions used for resources in this workshop. You may run into errors if you do.

### Objectives
- Understand OAX's prebuilt capabilities and KPI(s)
- Understand how to use ODA with ERP Cloud
- Take advantage of custom business logic capabilities of OIC
- Extract and load data from ERP Cloud to ADW.
- Create a centralized user store with IDCS
- Fraudulent behavior detection using CASB


### Required Artifacts
- The following lab requires an Oracle Public Cloud account that will either be supplied by your instructor, or can be obtained through the following steps.
- A cloud tenancy where you have the resources available to provision an ADW instance with 2 OCPUs, an OAC instance with 2 OCPUs, and an ODA instance. To see which services are available in your region, please click on the following link: [Region Services List](https://www.oracle.com/cloud/data-regions.html#northamerica)
- Oracle Cloud Infrastructure supports the following browsers and versions: Google Chrome 69 or later, Safari 12.1 or later, Firefox 62 or later.

## Acquire Oracle Cloud Account and Sign-in

### Step 1: Acquire an Oracle Cloud Trial or Workshop Account
- Bookmark this page for future reference.

- Please click on the URL to create your <a class=“trial-link”  href="https://myservices.us.oraclecloud.com/mycloud/signup?language=en&sourceType=:ex:tb:::RC_NAMK190227P00084:PredictDemandML_ADW_HOL&SC=:ex:tb:::RC_NAMK190227P00084:PredictDemandML_ADW_HOL&pcode=NAMK190227P00084" target="trial">Free Account</a> and complete all the required steps. When you complete the registration process you'll receive a $300 credit that will enable you to complete the lab for free. Additionally, you'll have access to a never-expiring Oracle Cloud account allowing you to explore even more capabilities of the Oracle Cloud.

- Soon after requesting your trial you will receive the following email. You may begin working on this lab once you receive this email.

## Navigate to Lab 100

-   You can always see a list of Lab Guides by clicking on the top right hamburger menu. A sidebar on the right of your browser window will come up. 

-   **You're now ready to continue with Lab 100!**

[Back to top](#introduction)
