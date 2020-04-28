# Oracle’s Cloud Platform: Transform and extend Oracle ERP Cloud

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
- Oracle Integration Cloud (OIC) and Autnomous Datawarehouse (ADW) to process additional orders and store information from ERP cloud in a separate database for long term retention and analytics.
- Oracle Identity Cloud Service (IDCS) and Cloud Access Security Broker (CASB) to centralize an enterprise's user store and enable fraudulent behavior detection. 

You will take on 2 Personas during the workshop. The **Data Scientist Persona** will prepare the data for training and validating the machine learning models and apply those models in order to predict the future demand. The **Business Analyst Persona** will also build and apply Machine Learning models using Oracle Analytics Cloud service without writing a single line of code. During the workshop, you will get exposure to Oracle Autonomous Data Warehouse (ADW), Oracle Machine Learning tool (OML), Oracle Analytics Cloud Service (OAC), Oracle Application Express (APEX), Oracle Rest Data Service (ORDS), and the Oracle Digital Assistant (ODA) chatbot.

The **Finance Manager** will
The **Business Analyst** will
The **New Hire** will
The **Customer** will
The **Application Security Architect** will 

To get an idea of how these services correlate to one another, here is an example of that Cloud Data Platform Architecture which can be extended with further Oracle services such as user federation through Identity Cloud Service (IDCS) and Oracle Integration Cloud (OIC):

![](./images/cloud-data-construction-arch.jpg " ")

**Note**: This lab is intended to be a comprehensive full cloud showcase. As such, it is assumed a user going through this workshop will be provisioning resources and creating users from scratch. If you decide to use existing infrastructure or resources, be aware and keep note of your namings so resources don't overlap and conflict. 

**Note**: Additionally, as much as possible, do not stray away from the naming conventions used for resources in this workshop. You may run into errors if you do.

*In addition to the workshop*, feel free to watch the walkthrough companion videos by clicking on the following links below and signing in with your Oracle SSO:

1. [Lab 100 Walkthrough Video](https://otube.oracle.com/media/Lab100A+ADW+and+APEX+Essentials/0_dluujk0s)
2. [Lab 200 Walkthrough Video](https://otube.oracle.com/media/Lab200A+Machine+Learning+with+ADW/0_xa5dg572)
3. [Lab 300 Walkthrough Video](https://otube.oracle.com/media/Lab300A+ORDS+and+APEX/0_s9mbgdfx)
4. [Lab 400 Walkthrough Video](https://otube.oracle.com/media/Lab+400A+Getting+Started+with+OAC/0_kmhc3x9v)
5. [Lab 500 Walkthrough Video](https://otube.oracle.com/media/Lab+500A+Analytics+in+OAC/0_ekr3yppl)
6. [Lab 600 Walkthrough Video](https://otube.oracle.com/media/Lab+600A+Implementing+APIs+into+ODA/0_f8nheacr)

**_To log issues_**, click here to go to the [github oracle](https://github.com/oracle/learning-library/issues/new) repository issue submission form.

### Objectives
- Provision an Autonomous Data Warehouse (ADW) Instance
- Build an Oracle Application Express (APEX) App
- Create Machine Learning Models within the Autonomous Data Warehouse (ADW) Instance by using the Oracle Machine Learning Tool (OML)
- Visualize Data and Prediction Models in Oracle Analytics Cloud (OAC)
- Bonus: Integrate a 3rd Party Web App and Oracle Digital Assistant (ODA) Chatbot


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
