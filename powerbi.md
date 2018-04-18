# Power BI

To setup a Power BI reports follow the instructions below.  
For more information see [Power BI](https://powerbi.microsoft.com/en-us/).

## Power BI Desktop Application
1. Download the Power UI Desktop application [here](https://powerbi.microsoft.com/en-us/desktop/).
2. Download the <a href="/assets/dnb_Optimizer_1_1_0_0_powerbi.pbit" download>D&B Template</a>. 
3. Launch the Power UI Desktop application, import the D&B template.
4. This import will fail as it tries to connect to a default environment.
5. Select Cancel and/or Close until you are returned to the reports view.
6. Select Home > Edit Queries > Data source settings > Change Source and enter your Dynamics environment details:<code> https&#58;&#47;&#47;&lt;Your Dynamics 365 (online) service URL&gt;/api/data/v&lt;8.0 or 8.1 or 8.2&gt; </code>
7. Select Apply Changes > Organizational Account > Sign In
8. After successfully signing in, select Connect
9. The report should now populate with the data from your Dynamics entities.

## Publish Report
1. Select Home > Publish and sign in.
2. Select a destination to publish the report too.

## Power BI Web
1. Sign in to [Power BI](https://powerbi.microsoft.com).
2. Select the workspace you published the report to, select the Reports tab and select the report.
3. Click the pin icon on the top right corner to Pin to dashboard, select a dashboard and click Pin.
4. Select the workspace you published the report to, select the Datasets tab and click the "Schedule Refresh" icon for the dataset associated with the report.
5. Expand the section titled "Scheduled Refresh" then wait a few seconds until the section becomes active.
6. Toggle the slider for "Keep your data up to date" to the "on" position, choose a time and frequency for the refresh, and Apply changes.

**Note: A refresh schedule must be provided for the dataset otherwise the associated dashboard will never update.**
**Note: You must put the report in a dashboard to embed it into a dynamics 365 dashboard.**

## Share Power BI Workspace
1. Select the workspace you created the dashboard in.
2. Click the ellipsis in the top right corner.
3. Select "Edit workspace".
4. Add the email addresses of the member you want to share the report with.
5. Click Save.

** Note: See [Dynamics](d365.md) section to view the Power BI report in Dynamics. **