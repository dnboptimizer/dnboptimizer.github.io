# The Common Data Service

The Common Data Service (a.k.a. CDS).  
For more information see [The Common Data Service](https://powerapps.microsoft.com/en-us/guided-learning/learning-common-data-service/).

## Environment
To create an Environment see [PowerApps Environment](https://powerapps.microsoft.com/en-us/guided-learning/learning-manage-environments/).

## Database/Entities
To create a Common Data Service database in an environment and understand entities see [The Common Data Service](https://powerapps.microsoft.com/en-us/guided-learning/learning-common-data-service/).

The Business Profile entity will be used to store the firmographic information retrieved from Dun & Bradstreet. The Business Profile entities should **not** be edited to avoid any unforeseen side effects.

**Note: Once the Data Integration project is setup the Accounts entity will be read only. If there is data in the Accounts entity we recommend you delete it first. See [Manage data in Excel](https://docs.microsoft.com/en-us/powerapps/data-platform-interactive-excel)**

**Note: Do not delete the records in the Organizations entity as the flows use them. Deleting them will cause the flows to stop working.**

## Perspectives
A perspective offers a "view into data" from a reporting point of view.  
For more information see [Create Power BI reports and dashboards with PowerApps Common Data Service](https://powerapps.microsoft.com/en-us/blog/cdsconnectortopowerbi/).