# PowerApps

For more information see [PowerApps](https://powerapps.microsoft.com/en-us/).

## Environment
To create an Environment see [PowerApps Environment](https://powerapps.microsoft.com/en-us/guided-learning/learning-manage-environments/).

## Connector
The D&B Optimizer for Microsoft connector provides a way for users to connect to the D&B global business database and return cleaned, firmographic intelligence data. Select the template to add it to your environment. The connector supports 3-legged OAuth2 so you will need to acquire a ClientId and SecretKey from Dun & Bradstreet before you can use the connector. Connect with your D&B account manager or sign up for a [free demo](http://www.dnb.com/marketing/media/dnb-optimizer-for-microsoft-cds-demo.html) to learn how to obtain access.

## Trigger
The D&B Optimizer for Microsoft trigger is based on a scheduler. By default, the flow will recur every 5 minutes.  
For more information see [Run flows on a schedule](https://flow.microsoft.com/en-us/documentation/run-tasks-on-a-schedule/).

## Flow Templates
The D&B Optimizer for Microsoft comes with two templates, one to match and insert firmographic intelligence into your records and one to keep that data up to date. We recommend you use both in your environment to get the maximum benefit from the solution.

**<u>Dynamics for Sales Integration with D&B</u>**  
This flow template will run every five minutes, search for new or updated records and insert firmographic intelligence into your records within your Microsoft application environment.

When you try to save the template you will see errors on four of the steps in the flow. These errors are because the flow doesn't know which Dynamics 365 environment to point to. To fix the errors go to the steps (listed below) and from the drop-down select your Dynamics 365 environment. Then click "Save flow" at the bottom of the page or "Update flow" at the top of the page.

* Check Running Status
* Delete Optimizer Status
* Create Optimizer Status
* Get Last Matched Account Timestamp
* List Records
* Find Oldest Account
* Create Watermark from Now
* Create Watermark from Oldest Account
* Update Dynamics Business Profile
* Create Dynamics Business Profile
* Link Account to Business Profile
* Update Match Grade
* Create Dynamics Match Grade
* Link Match Grade to Account
* Move Matched Watermark
* Refresh Optimizer Status
* Delete A Record

**<u>Dynamics for Sales Integration with D&B - Refresh</u>**  
This flow template will run every hour, search for Business Profile records older than fourteen days and update the records with the latest D&B firmographic data.

When you try to save the template you will see errors on four of the steps in the flow. These errors are because the flow doesn't know which Dynamics 365 environment to point to. To fix the errors go to the steps (listed below) and from the drop-down select your Dynamics 365 environment. Then click "Save flow" at the bottom of the page or "Update flow" at the top of the page.

* List Records
* Update Dynamics Business Profile