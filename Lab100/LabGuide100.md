# Lab 100: Oracle Analytics for Application (OAX) with ERP Cloud (INTERNAL ONLY)

## Introduction

This lab will walk you through OAX and we will be analyzing financial data from your Fusion ERP data. The ERP data has already been pre-configured to be in your OAX environment, and will require you to understand how the out-of-the-box visualizations and metrics help the Finance Manager figure out ways to better the company’s accounts payable ratio. *In addition to the workshop*, feel free to watch the walk-through companion video by clicking on the following link:
[Lab 100 Walkthrough Video](<INSERT LINK HERE>)

### Objectives
-   Learn about OAX's prebuilt capabilities, decks, and KPI cards
-   Learn how to build and customize KPI cards
-   Learn how to set conditions on KPI cards
-   Learn how to send out notifications to team members  

### Required Artifacts
-   The following lab requires an Oracle Public Cloud account that will either be supplied by your instructor, or can be obtained through the following steps.
-   An OAX environment from nac-oax-demo-environment
-   The estimated time to complete this lab is 12 minutes

## Part 1. Sign Into OAX Environment

### **STEP 1** : Log in using SSO credentials

-   Once receiving access to your OAX environment, click on **‘Oracle SSO’** to sign in using your SSO credentials. 

-   **Type in SSO**

  ![](./images/OAXEnviron.png " ")

  ![](./images/SSO.png " ")

## Part 2. Navigating Through the OAX Environment

### **STEP 1**: Get to Know the OAX Environment

-   From the default landing page, click on the **hamburger menu** on the top left and **click ‘Decks’** to view the available and pre- built decks.

![](./images/Deck.png " ")

-   Begin familiarizing yourself with the decks by clicking each deck title (Payables, Balance Sheet, etc.).

![](./images/DeckOptions.png " ")

## Part 3. Recognizing Alerts

-   The financial manager wants to dive deeper into their Accounts Payable ratio, which is described in the ‘My Working Capital’ deck.

### ** STEP 1**: Learning About your Decks
-   **Click to ‘My Working Capital’** and familiar yourself with the KPI cards the financial manager has chosen for this deck.

![](./images/Click_to_deck.png " ")

-   Notice the colors above each KPI card; these describe the health of the KPI based on conditions, which we will get into in the following parts.

-   Notice that ‘Days Payable Outstanding’ has a YELLOW condition, which tells us we need to investigate further.

![](./images/MyWorkingCapital.png " ")

## Part 4: Drill Down

### **STEP 1**: Drill into Details

-   To review the ‘Days Payable Outstanding’ KPI in more detail, **click on** its **hamburger menu** and **click ‘Payables Analysis’**.

![](./images/Clickto_Payables_Analysis.png " ")

-   Notice the automated visualizations that come with OAX, to help the financial manager understand variables affecting the ratio.

## Part 5: Adding a KPI Card

-   Adding additional KPIs help describe corresponding KPIs.

### **STEP 1** : Creating Card

-   To add your own card, **click on the addition button** (Note: a deck can hold a max of 8 KPI cards).
![](./images/AddCard.png " ")

### **Step 2**: **Type in** ‘AP Turnover Rate WC’ 

![](./images/APTurnoverRate_WC.png " ")

### **STEP 3**: **Double click** the ratio to pre-populate the Preview section on the right with an automated visualization

![](./images/Populate_Preview.png " ")

### **STEP 4**: Customize 

-   To customize **click ‘Customize Card’** to show the next window: 

![](./images/Customize_Card.png " ")

![](./images/Wo_Show_Change.png " ")
 
-   **Check** the ‘Show Change’ box to obtain the AP Turnover’s comparison metric.

-   Notice the new metric in the visualization (-9.59% QoQ).

![](./images/W_Show_Change.png " ")

### **STEP 5**: **Click ‘Status & Notifications’** on the left to customize alerts.

![](./images/Conditions.png " ")

-   Notice the default settings and what percentile describes each status’ category. 

-   Keep the conditions at its default settings, and **click ‘Add Card’**.

![](./images/Adding_AP.png " ")

-   Notice your new KPI has been added to your deck.

-   Recognize that your new KPI follows the same alert condition as ‘Days Payable Outstanding’ which validates the health of the Accounts Payable metric.

![](./images/Card_Added.png " ")

## Part 6: Send Notifications to Teammates
### **STEP 1**: 
-   Next to the hamburger menu of your KPI card’s hamburger menu, **click** the **‘Maximize’ button** to expand and retrieve a summarized view of your metric.

![](./images/Maximize.png " ")

-   Familiarize yourself with the refined details on the expanded version of your visualization.

![](./images/AP_Turnover_Max.png " ")

-   The financial manager needs to notify his business analyst of the new metric, and the status of Accounts Payable.

### **STEP 2**:

-   To notify, he’ll **click on ‘Enter Message’** on the bottom right and type in 'Charles, please investigate', and *click ‘Add Note’**, which will send a notification to the business analyst to look into this metric. 

![](./images/Adding_Note.png " ")

### **STEP 3**: **Click ‘<’** to jump back to the home page of the KPI card, and see that the note has been successfully added to the card.

![](./images/Show_New_Note.png " ")

## Part 7: Drill Drown into Pre-Built Reports & Visuals

-   The business analyst has selected pre-built visualizations that he wants to attach to the ‘AP Turnover Rate WC’ card.

-   The graphs he chose help describe in detail suppliers, invoices, invoice amount, balances, and more.

### **STEP 1**: Review Attached Reports

-   **Click on** the **hamburger menu** of ‘AP Turnover Rate WC’ and notice the six new reports (beginning after ‘Favorites’).

![](./images/Hamburger_Menu.png " ")
 
### **STEP 2**: **Click on ‘AP Balances Analysis’** to see which pre-built visuals have been chosen by the business analyst to create this report

![](./images/NewReport1.png " ")

![](./images/AP_Bal1.png " ")

### **STEP 3**: **Click ‘<’** at the top left to review additional reports

![](./images/AP_Bal2.png " ")

### **STEP 4**: **Click on ** the hamburger menu on the ‘AP Turnover Rate WC’ card again and **click on ‘AP Invoice Analysis’**

![](./images/Hamburger_Menu.png " ")

![](./images/AP_Invoices.png " ")

-   Familiarize yourself with the pre-built visuals the business analyst has included in his report.

-   Notice the written out report on the bottom right, which has been generated by the ‘Natural Language Generator’, which is describing the ‘Monthly AP Invoices Activity’ visual on the top right.

![](./images/Invoice_Report.png " ")

### **STEP 5**: **Click** through the report by selecting any of the **blue buttons** on the bottom **or the ‘>’** at the bottom right

![](./images/Last_Page.png " ")

## Summary

-   In this lab, we walked through logging into your OAX environment and interacted with the out-of-the-box KPI cards and decks which pull from your Fusion ERP environment. We also learned how to add and customize our own KPI metrics to, while collaborating with colleagues by sending them alert notifications for KPIs that indicated a YELLOW condition
-   **You’re now ready to move onto the next lab!**

