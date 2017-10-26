# Data Integration

To setup a data integration project in PowerApps follow the instructions below.
For more information see [Microsoft's introduction to Data Integration](https://docs.microsoft.com/en-us/dynamics365/unified-operations/dev-itpro/data-entities/data-integration-cds). You then reference those connections in a Data Integration project.

Before you can work with a Data Integration project, you must provision a connection for each system that you intend to work with in the Microsoft PowerApps portal. You then reference those connections in a Data Integration project.

1. From the PowerApps [website](https://web.powerapps.com) click on settings and select the "Admin center" menu item. ![logo](assets/settings_cog.png "Settings")
2. Then select the Data integration tab.

## Connection Sets
Connection sets are a collection of two more connections, organization mapping information, and integration keys that can be reused among projects.

1. Click "New connection set" and fill in the details. 
  1. Give the Connection set a name.
  2. Select a Connection & Environment for Dynamics 365.
  3. Select a Connection & Environment for Common Data Service.
  4. Organizations:
    1. Enter your Organization for Dynamics 365 for Sales.
    2. Enter your Organization for Common Data Service.
2. Click "Create".

## Projects
Projects enable the flow of data between systems.

1. Click "New project" and fill in the details.
2. Give the project a name.
3. Select the "Accounts (Sale to CDS)" template and click next.
4. Choose Connection sets and click next.
4. Select an Organization and click next.
5. Read the privacy notice and consent and click create.

## Run/Schedule Project
Now everything is setup we can run or schedule the Project.

1. Go back to Projects.
2. Select a Project from the list.
3. Select the Scheduling tab.
  1. Leave as Run manually and click the Run project icon in the top right corner.
  2. Or select Recur every and pick your settings and click the "Save schedule".
  
<b>Note: We recommend scheduling the project to recur every 30 mins.</b>

## Known Issues
1. If your records in Dynamics 365 have an invalid Country/Region you will get an invalidEnums error on the mailingpostaladdress_country source field during the DI sync.