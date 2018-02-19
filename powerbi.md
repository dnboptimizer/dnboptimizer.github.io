# Power BI

To setup a Power BI reports follow the instructions below.  
For more information see [Power BI](https://powerbi.microsoft.com/en-us/).

## Activate Power BI
Request activation of Power BI in your tenant: [aka.ms/cdspowerbi](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRwWp5miMBjRAhmGSAULZVM5URVBXNE01M1NSUVFDWlpQVUhNNzQ0MUdINi4u)

**Note: This may take several hours or into the next business day.**

## Power BI Desktop Application
1. Download the Power UI Desktop application [here](https://powerbi.microsoft.com/en-us/desktop/).
2. Download the <a href="/assets/dnb_Optimizer_1_1_0_0_powerbi.pbit" download>D&B Template</a>. 
3. Launch the Power UI Desktop application, import the D&B template and sign in.
4. Select Home > Edit Queries > Data source settings, select your Dynamics environment and from the list select the Accounts, BusinessProfile and MatchGrade perspective.
5. The report should now popular with the data from your Dynamics entities.

## Publish Report
1. Select Home > Publish and sign in.
2. Select a destination to publish the report too.

## Power BI Web
1. Sign in to [Power BI](https://powerbi.microsoft.com).
2. Select the workspace you published the report too, select the Reports tab and select the report.
3. Click the pin icon on the top right corner to Pin to dashboard, select a dashboard and click Pin.

**Note: You must put the report in a dashboard to embed it into a dynamics 365 dashboard.**

## Share Power BI Workspace
1. Select the workspace you created the dashboard in.
2. Click the ellipsis in the top right corner.
3. Select "Edit workspace".
4. Add the email addresses of the member you want to share the report with.
5. Click Save.

** Note: See [Dynamics](d365.md) section to view the Power BI report in Dynamics. **