---
title: "Enable Microsoft 365 usage analytics"
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: 
- M365-subscription-management 
- Adm_O365
- Adm_TOC
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 9db96e9f-a622-4d5d-b134-09dcace55b6a
description: "Learn how to start collecting data for your tenant by using the Microsoft 365 Usage Analytics template app in Power BI."
---

# Enable Microsoft 365 usage analytics

Microsoft 365 usage analytics is also available for Microsoft 365 US Government Community.
  
## Steps to enable Microsoft 365 usage analytics

To get started with Microsoft 365 usage analytics you must first make the data available in the Microsoft 365 admin center, then initiate the template app in Power BI.
  
### Get Power BI

If you don't already have Power BI, you can [sign up for the free Power BI service](https://go.microsoft.com/fwlink/p/?linkid=845347). Select **Get started free** to get the free version. 
  
![Select Get started free to get Power Bi](../media/7916b7ac-c1c8-40c0-b076-9a96ef5e0eb7.png)
  
You can also expand **Products** to buy a version of Power BI. 

>[!NOTE]
>You need a Power BI Pro license to install, customize, and distribute a template app. Please see more at [Prerequisites](https://docs.microsoft.com/en-us/power-bi/service-template-apps-install-distribute?source=docs#prerequisites)

>You need a Power BI Pro license to share your content, and the people you share it with do too, or the content needs to be in a workspace in a [Premium capacity](https://docs.microsoft.com/en-us/power-bi/service-premium-what-is).
  
### Enable the template app

To enable the template app, you have to be either a **global administrator**, **report reader**, **Exchange administrator**, **Skype for Business administrator**, or **SharePoint administrator**. 
  
See [About admin roles](../add-users/about-admin-roles.md) for more information. 
  
1. In the admin center, go to the **Reports** \> <a href="https://go.microsoft.com/fwlink/p/?linkid=2074756" target="_blank">Usage</a> page. 
    
2. On the **Usage** page, locate the **Microsoft 365 usage analytics** card, and select **Get started**.
    
3. On the Reports panel that opens, set **Make data available to Microsoft 365 usage analytics for Power BI** to **On** \> **Save**. 
  
This initiates the data collection process and will complete in 2 to 48 hours depending on the size of your tenant. The **Go to Power BI** button will be enabled (no longer gray) when data collection is complete. 
    
### Initiate the template app

To initiate the template app, you have to be either a **global administrator**, **report reader**, **Exchange administrator**, **Skype for Business administrator**, or **SharePoint administrator**. 
  
1. Copy the tenant Id and select **Go to Power BI**.
    
2.	When you get to Power BI, sign in. Select Apps->Get apps from the navigation menu.    
  
3. In the **Apps** tab, type Microsoft 365 in the search box and then select **Microsoft 365 usage analytics** \> **Get it now**.

    [![Select Get it now](../media/78102250-9874-4a32-8365-436f13560b52.png)](https://app.powerbi.com/groups/me/getapps/services/cia_microsoft365.microsoft-365-usage-analytics)
    
4.	Once the app is installed. Click on the tile to open it.

5.	Click **Explore app** to view the app with sample data. Click **Connect** to connect the app to your organization’s data.

6.	After clicking **Connect**, on the **Connect to Microsoft 365 usage analytics** screen, type in the tenant Id you copied in step (1) \> **Next**.
    
7. On the next screen, select **oAuth2** as the **Authentication method** \> **Sign in**. If you choose any other authentication method, the connection to the template app will fail.
    
    ![Choose oAuth2 as authentication method](../media/ac85a360-c278-4c60-8aa3-68f4828f1d96.png)
  
8. Once the template app is instantiated the Microsoft 365 usage analytics dashboard will be available in Power BI on the web. The initial loading of the dashboard will take between 2 to 30 minutes.
  
Tenant level aggregates will be available in all reports. **User-level details will only become available after the 1st or 15th day of the calendar month after opting in**. This will impact all reports under User Activity (See [Navigate and utilize the reports in Microsoft 365 usage analytics](navigate-and-utilize-reports.md) for tips on how to view and use these reports).
    
## Make the collected data anonymous

To make the data that is collected for all reports anonymous, you have to be a global administrator. This will hide identifiable information such as user, group and site names in reports and in the template app .
  
1. In the admin center, go to the **Settings** \> **Settings**, and under **Services** tab, choose **Reports**.
    
2. Select **Reports**, and then choose to **Display anonymous identifiers**. This setting gets applied both to the usage reports as well as to the template app.
  
3. Select **Save changes**.S
