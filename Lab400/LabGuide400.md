# Lab 400: Securing Oracle ERP with Identity Cloud Service & Cloud Access Security Broker (INTERNAL ONLY)

<!-- Comment out table of contents
## Table of Contents
[Introduction](#introduction)
-->

## Introduction

This lab walks you through registering a Fusion apps demo environment. From there you will be able to start integrating the demo with Identity Cloud Service (IDCS) and Cloud Access Security Broker (CASB). 
*In addition to the workshop*, feel free to watch the walk-through companion video by clicking on the following link:
[Lab 400 Walkthrough Video](<INSERT LINK HERE>)



### Objectives
-   Learn how to request a demo instance of ERP Cloud
-   Understand the capabilities of Oracle's Identity Cloud Service and Cloud Access Security Broker and how they provide an extra layer of security for ERP Cloud.

### Required Artifacts
-   ERP Cloud Instance from [demo.oracle](https://demo.oracle.com/)
-   IDCS Instance
-   CASB Instance
-   The estimated time to complete this lab is 60 minutes.

### Extra Resources
-   To learn more about Identity Cloud Service (IDCS), feel free to explore the capabilities by clicking on this link: [IDCS Documentation](https://docs.oracle.com/en/cloud/paas/identity-cloud/)
-   To learn more about Cloud Access Security Broker (CASB), feel free to explore the capabilities by clicking on this link: [CASB Documentation](https://docs.oracle.com/en/cloud/paas/casb-cloud/)
-   To learn more about , Oracle ERP Cloud feel free to explore the capabilities by clicking on this link: [ERP Cloud](https://go.oracle.com/LP=85331?elqCampaignId=48423&src1=ad:pas:go:dg:erp&src2=wwmk160606p00030c0001&SC=sckw=WWMK160606P00030C0001&mkwid=%7cpmt%7ce%7cpdv%7cc%7c&GOOGLE&oracle+erp+cloud&Cj0KCQjw7qn1BRDqARIsAKMbHDaSJX4r2woRQrLHIFTCk3imWrf6ORbhp3f1czxUvvxVTsz8Votd7TQaAhggEALw_wcB&gclid=Cj0KCQjw7qn1BRDqARIsAKMbHDaSJX4r2woRQrLHIFTCk3imWrf6ORbhp3f1czxUvvxVTsz8Votd7TQaAhggEALw_wcB&gclsrc=aw.ds)


## Part 1. Requesting an ERP Cloud Instance

### **STEP 1**: Login to Demo Central and Request an Environment

-   Once at the [homepage](https://demo.oracle.com/apex/f?p=DEMOWEB:HOME::::::), navigate to the "Demos" section. 

![](../Lab200/images/demo-home.jpg " ")

-   Click the **Register a Demo**.

![](../Lab200/images/register.jpg " ")

-   Search or select the Demo Title called **FUSION GSI - ERP, SCM, HCM & Engagement Cloud**.

![](../Lab200/images/demo-title.jpg " ")

-   Fill in the details, demo resource details, activity dates, and any additional information. 

-   The select **Next** in the bottom right corner.

![](../Lab200/images/details.jpg " ")

-   In the additional information section select the Horizontal or Industry-Specific category that is most applicable. 

-   The next field will ask if you want to add other to this Demo, if applicable please enter the Oracle email of the person you want to add to the demo.

-   Next, select the product you plan to include in your demo. This should be **Products -> Cloud Apps -> Fusion Apps -> ERP Cloud**.

-   Click **Next**.

-   Confirm your details and click **Submit**.

![](../Lab200/images/submit.jpg " ")

### **STEP 2**: Access ERP Cloud Environment

-   Once the environment has been approved you will receive an email from **demo-central-noreplies_ww@oracle.com**, this will have a **link** where you can access your registration details and environment information. 

-   Make sure to save the access details and copy the password as we will be using it in the next part. Please **Note** that the environment password will change weekly. 

-   Then click on **Launch Demo**

![](../Lab200/images/env-details.jpg " ")

-   Click on **ERP and SCM Cloud Login** and you will be taken to the **Sign In** page for your ERP instance.

![](../Lab200/images/erp1.jpg " ")

-   Here you can sign-in with a few different users using the same password, but in this workshop we will be exploring two different personas. 

## Part 2. Provision a user from IDCS to ERP Cloud

### **STEP 1**: Access the IDCS console

-   Navigate to the **IDCS console** sign-in page provided by your lab facilitator. Enter the provided administrator username and password. **If you do not have the URL or the credentials, please contact your lab facilitator.**

![](./images/idcs-login.png " ")

-   Once logged in, you will see the IDCS console page displaying all of the relevant information (users, groups, passwords, etc.) that an identity domain administrator would be interested in.  

-   In the **Users** module, click on the profile icon silhouette to navigate to the list of users in IDCS.

![](./images/idcs-console.png " ")

### **STEP 2**: Create a new user in IDCS

-   We are now seeing the list of users in the current IDCS instance.

-   Click on the **Add** button to add a new user to IDCS.
    
![](./images/idcs-users.png " ")

-   A window will pop up prompting us to enter the new user's information. Go ahead and fill out the required fields then click **Next**.

![](./images/idcs-newuser.png " ")

-   We're now prompted to assign this user to a group. For the purpose of this lab, the facilitators have already created the group for us. Assign the user to **ERP_FA_Users** then click **Finish**.

![](./images/idcs-newusergroup.png " ")

-   The new user is created and we can see the user's current information, groups and application access. If you explore the groups and access tabs, we can see that the user belongs to **ERP_FA_Users** group and has access to **two** applications. These applications allow us to provision the user from IDCS to ERP Cloud using a pre-built connector. 

![](./images/idcs-newuserprofile.png " ")

![](./images/idcs-access.png " ")



### **STEP 3**: Verify new user creation in ERP Cloud
-   Sign in to the demo ERP Cloud instance as **DEMOFAADMIN** and use the password copied previously from the clipboard. This user, Harry Hooper, is the security administrator for the ERP Cloud instance.

![](./images/erp-login.png " ")

-   Navigate to the **home page** of the ERP Cloud instance.

-   On the home page, scroll the dashboard until we find **Tools**. Click on it.

-   Click on **Security Console**.

![](./images/erp-security.png " ")

-   Here we see the security configuration settings available to the administrator. 

-   Click on **Users**.

-   Now, we want to verify that the user we created in IDCS also exists in the ERP Cloud system.

-   In the **Search bar**, type the username of the user created in IDCS.

-   If the provisioning was successful, we will see the new user under **Search Results** as shown.

![](./images/erp-users.png " ")

## Part 3. Monitor risky user behavior in ERP Cloud with CASB.

### **STEP 1**: Access the CASB console.

-   Navigate to the **CASB console** sign-in page provided by your lab facilitator. Enter the provided administrator username and password. **If you do not have the URL or the credentials, please contact your lab facilitator.**

![](./images/casb-login.png " ")

-   Once logged in, we're greeted with the CASB dashboard. Here the security administrator can get quick insights into what applications are experiencing risky behaviors. These risks can also be filtered by geographical location, risk type, and associated users.

![](./images/casb-dashboard.png " ")

### **STEP 2**: Create a new risk policy.

-   Now we're going to create a new risk policy to track abnormal user behavior.

-   Click on the upper left menu.

-   Expand the **Configuration** sub-menu.

-   Click on **Policy Management**. 

![](./images/casb-console.png " ")

-   Here we can see a list of all the policies our CASB is leveraging to monitor all the applications associated with it for risky behavior. These policies are used to determine how we define risky behavior. 

![](./images/casb-policy.png " ")

-   Click on **New Policy**. 

    -   Enter a **Name**, **Description**, and select a **Risk Priority** for the new policy. You may choose to include this in a user's risk score as well. Click **Next**.
    
    ![](./images/casb-newpolicy1.png " ")

    -   Select **ERPCloud** for **Application type**, **Any** for **Application instance**, **Job Role** for **Resource**, **Text** for **Resource name**, contains **Business Development Manager**, **Role membership added** for **Action on this resource**. Click **Next**.
    
    ![](./images/casb-newpolicy2.png " ")
    
    -   Leave blank and click **Next**.
    
    ![](./images/casb-newpolicy3.png " ")
    
    -   Leave as is and click **Next**.
    
    ![](./images/casb-newpolicy4.png " ")
    
    -   You provide a custom alert message or add your email for the alert to be sent to you directly. Click **Next**.
    
    ![](./images/casb-newpolicy5.png " ")
    
    -   Review and click **Submit**.
    
    ![](./images/casb-newpolicy6.png " ")

### **STEP 3**: Assign a faulty job role to the new user created in Part 2. 

-   Navigate back to the ERP Cloud security console. 

-   Search for the newly created user and click on the user's display name.

![](./images/erp-users.png " ")

-   Click **Edit** on the upper menu bar.

![](./images/erp-userinfo.png " ")

-   Click **Add Role** next to the Roles header.

![](./images/erp-edituser.png " ")

-   Search for **Business Development Manager** and select **GSE Business Development Manager**.

-   Click **Add Role Membership** then click **Done**.

![](./images/erp-addrole.png " ")

-   The new user is now assigned the faulty job role.

-   It will take a few minutes for CASB to detect the anomaly. Hang tight!

### **STEP 4**: Verify that an abnormal role assignment was detected by CASB.

-   Navigate back to the CASB console.

![](./images/casb-dashboard.png " ")

-   Click on the upper left menu.

-   Click on **Applications**.

-   Select **FA_CASB** and click **View details**.

![](./images/casb-applications.png " ")

-   Once CASB detects the anomaly, the risk event will be shown similarly to below.

![](./images/casb-applicationdetails.png " ")

-   To gain more insight, click on the risk event row. Here we can see which user initiated the role assignment, what role was assigned, and to whom the role was assigned. 

![](./images/casb-riskevent.png " ")

## Summary

-   In this lab, you requested a demo ERP Cloud instance and further secured it with IDCS and CASB to detect fraudulent user behavior as well as leverage auto user provisioning from a single identity store to a target application.


-   **You are finished with all of the labs!**

[Back to top](#introduction)


