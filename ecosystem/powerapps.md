# PowerApps

For more information see [PowerApps](https://powerapps.microsoft.com/en-us/).

## Connector
The D&B Optimizer for Microsoft connector provides a way for users to connect to the D&B global business database and return cleaned, firmographic intelligence data. Select the template to add it to your environment. The connector supports 3-legged OAuth2 so you will need to acquire a ClientId and SecretKey from Dun & Bradstreet before you can use the connector. Connect with your D&B account manager or sign up for a [free demo](http://www.dnb.com/marketing/media/dnb-optimizer-for-microsoft-cds-demo.html) to learn how to obtain access.

## Trigger
The D&B Optimizer for Microsoft trigger is based on a scheduler. By default the flow will recur every 5 minutes.  
For more information see [Run flows on a schedule](https://flow.microsoft.com/en-us/documentation/run-tasks-on-a-schedule/).

## Flow Templates
The D&B Optimizer for Microsoft comes with two templates, one to match and insert firmographic intelligence into your records and one to keep that data up to date. We recommend you use both in your environment to get the maximum benefit from the solution.

**<u>Dynamics for Sales Integration with D&B and CDS</u>**  
After you have setup and run the [data integration](ecosystem/di.md), save this template. This flow template will run every five minutes, search for new or updated records and insert firmographic intelligence into your records within your Microsoft application environment.

**<u>Dynamics for Sales Integration with D&B and CDS - Refresh</u>**  
This flow template will run every hour, search for Business Profile records older that fourteen days and update the records with the latest D&B firmographic data.

**Note: You must run or schedule the Data Integration project to run at least once before you create a template. See [Data Integration](ecosystem/di.md).**