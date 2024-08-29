This is the continuation of SalesforceCRM project 1 which is avaiable in SalesforceCRM  repository.

Project 2: Digital Experience and Product Catalog Setup
1. Enabling Digital Experience
1.	Create a Site and Template
o	Login: Log in to your Salesforce Developer Org.
o	Go to Experience Cloud: Navigate to Setup > Experience Cloud > All Sites.
o	Create a New Site:
	Click New and select Customer Service template.
	Follow the prompts to name and create the site.
o	Access the Site:
	After creation, click View Site to access the site setup.
2.	Workspace Configuration Under Builder
o	Open Builder: Go to Setup > Experience Cloud > All Sites and click Builder next to your newly created site.
o	Configure Workspace: Customize the workspace layout to align with your company’s branding and functional requirements.
3.	Rich Text Editor and Autocomplete Search
o	Rich Text Editor: Ensure that the Rich Text Editor component is included where necessary. You can add this through the Page Components tab in the Builder.
o	Autocomplete Search: Add an Autocomplete Search component to enable users to quickly find products or information.
4.	Theme Configuration
o	Theme Settings:
	Go to Theme in the site’s settings.
	Customize the theme to reflect your company’s branding (colors, fonts, etc.).
5.	Administration Settings
o	Configure Settings: Navigate to Administration under the site settings to configure site access, permissions, and other administrative settings.
6.	Theme and Font Configuration
o	Return to Theme: Go back to the Theme settings to adjust font styles and sizes according to your company’s guidelines.
2. Products List and Catalog Page Creation
1.	Clone Products List View
o	Go to Salesforce Setup:
	Navigate to Object Manager > Products.
	Click on List Views and find the default Products list view.
	Click Clone to create a new list view.
o	Add Filters:
	Customize filters to match your requirements (e.g., by category, availability).
2.	Drag the List to the Page Using Record List Component
o	Open Experience Builder:
	Go back to the Builder in the site.
o	Add Record List Component:
	Drag the Record List component onto the page where you want the products list to appear.
	Configure the component to use the newly cloned list view.
	Adjust the display settings to Compact mode for a streamlined look.
3.	Create Product Catalog Page
o	Create a New Page:
	In the Builder, select New Page and choose Object Page.
	Use the Rich Content Components to add details about products and use the Rich Text Editor for content.
o	Customize Header Properties (Optional):
	Adjust header properties in the Record List settings if needed for better visibility and navigation.
4.	Add Other Components
o	Ask a Question: Include a component that allows users to submit questions or requests.
o	Customer Contact: Add a component for customer contact options or forms.
5.	Create and Add Dashboard
o	Create Report:
	Go to Reports & Dashboards > Reports and create a report to track key product metrics.
o	Create Dashboard:
	Navigate to Reports & Dashboards > Dashboards and create a dashboard.
	Add components to visualize key data (e.g., top products, sales metrics).
o	Drag Dashboard to the Page:
	In the Builder, drag the dashboard component to your page.
	Use the Roll-Up Summary options if needed to include data from related records.
	Adjust pixel size and layout for optimal display.
Final Steps
1.	Review and Test:
o	Ensure all components are working as expected and the layout aligns with the company's branding and functional needs.
o	Perform testing to verify that the site and product catalog meet all requirements.
2.	Publish:
o	Once everything is configured and tested, publish the site for users to access.
This should help you complete Project 2, focusing on creating a product catalog and a comprehensive homepage for your Salesforce site.
Creating the Product List
1.	Create or Customize the Product List View
o	Log In: Access your Salesforce Developer Org.
o	Navigate to Object Manager:
	Go to Setup > Object Manager > Product (or Products if using a different name).
o	Create or Clone a List View:
	Select List Views.
	If you want to create a new list view, click New.
	If you want to clone an existing list view, select the existing view and click Clone.
o	Configure the List View:
	Name the list view (e.g., "Product List View").
	Set the filter criteria to include the products you want to display.
	Choose the fields to display in the list view (e.g., Product Name, Price, Quantity).
	Save the list view.
Implementing the Product List on the Homepage
1.	Access Experience Builder
o	Navigate to Experience Cloud:
	Go to Setup > Experience Cloud > All Sites.
	Find your site and click Builder.
2.	Add the Product List to the Homepage
o	Open the Homepage:
	In Experience Builder, select the Homepage or the page where you want to display the product list.
o	Add a Record List Component:
	From the Components panel, drag the Record List component onto the desired section of the homepage.
o	Configure the Record List:
	Click on the Record List component to configure its settings.
	Choose the Product object or the list view you created earlier from the Record List settings.
	Configure the display options:
	Filters: Apply any necessary filters if you want to show only specific products.
	Display: Choose how you want to display the records (e.g., Compact, Full).
	Columns: Select the columns to display (e.g., Product Name, Price).
3.	Customize the Page Layout
o	Adjust Layout and Style:
	Use the Page Properties and Style options to adjust the layout and style of the product list to fit your design needs.
	Ensure the product list is visually appealing and easy to navigate.
o	Add Additional Components:
	You can add other components around the product list, such as Search or Filter components, to enhance functionality.
	You might also include components like Call to Action or Promotional Banners to highlight featured products.
4.	Publish Your Changes
o	Preview the Page:
	Use the Preview option in Experience Builder to see how the product list looks on the homepage.
	Make any necessary adjustments.
o	Publish:
	Once you’re satisfied with the layout and functionality, click Publish to make your changes live.
5.	Testing
o	Test Functionality:
	Ensure the product list displays correctly and that users can interact with it as expected.
o	Check Responsiveness:
	Verify that the product list looks good on different devices (e.g., desktop, tablet, mobile).
By following these steps, you'll have a functional product list integrated into the homepage of your Salesforce site, ready for users to interact with and explore.
If you need to showcase a single, impactful report or dashboard to demonstrate your Salesforce skills to employers, consider creating a Sales Performance Dashboard. This dashboard provides a comprehensive view of sales activities and product performance, and it's often highly relevant to employers seeking to understand how you can leverage Salesforce for business insights.
Sales Performance Dashboard
Components
1.	Sales Overview
o	Chart Type: Bar Chart
o	Data: Total Revenue by Product.
o	Objective: Show how much revenue each product has generated.
2.	Top Products
o	Chart Type: Pie Chart
o	Data: Revenue Distribution by Product Category.
o	Objective: Highlight which product categories are generating the most revenue.
3.	Sales Pipeline
o	Chart Type: Funnel Chart
o	Data: Opportunities by Stage.
o	Objective: Visualize the distribution of opportunities through various stages of the sales process.
Implementation Steps
1.	Create Custom Reports:
o	Total Revenue by Product:
	Go to Reports > New Report.
	Select the Opportunities report type.
	Group by Product Name.
	Summarize the Amount field to get the total revenue.
o	Monthly Sales Trends:
	Create a similar report but group by Close Date (monthly).
o	Revenue Distribution by Product Category:
	Create a report summarizing revenue by Product Category.
2.	Build the Dashboard:
o	Go to Reports & Dashboards > Dashboards > New Dashboard.
o	Add Components:
	Bar Chart: Add the "Total Revenue by Product" report.
	Line Chart: Add the "Monthly Sales Trends" report.
	Pie Chart: Add the "Revenue Distribution by Product Category" report.
	Funnel Chart: Create a report for opportunities by stage and use it for the funnel chart.
o	Customize Layout:
	Arrange components for clarity and impact.
	Use meaningful titles and labels.
3.	Test and Refine:
o	Review the dashboard for accuracy and usability.
o	Ensure that data updates correctly and visualizations reflect the intended insights.
Key Skills Demonstrated
•	Data Aggregation: Ability to aggregate and summarize sales data.
•	Visualization: Skill in creating effective visual representations of data.
•	Insights: Capability to derive actionable business insights from Salesforce data.
This dashboard will highlight your ability to analyze sales data, track performance, and present information in a visually appealing and informative manner.
To drag the Sales Performance Dashboard to a Salesforce Experience Builder page, follow these steps:
Steps to Add a Dashboard to a Salesforce Experience Builder Page
1.	Access the Experience Builder:
o	Go to Setup (gear icon in the top-right corner).
o	Search for Digital Experiences or Experience Cloud in the Quick Find box.
o	Select All Sites and then click on Builder next to the site you want to edit.
2.	Navigate to the Page:
o	In the Experience Builder, find the page where you want to add the dashboard.
o	You can select an existing page or create a new page if needed.
3.	Add a Dashboard Component:
o	On the left-hand side, you’ll see the Components panel.
o	Scroll through or search for the Dashboard component. If it’s not visible, you might need to look under Custom Components or use the search bar.
4.	Drag and Drop the Dashboard Component:
o	Drag the Dashboard component from the Components panel onto your page layout where you want it to appear.
o	Release the component to place it on the page.
5.	Configure the Dashboard Component:
o	After placing the component, you’ll need to configure it to display your Sales Performance Dashboard.
o	Click on the component you just added to open its properties panel on the right side.
o	Under Dashboard, select the Sales Performance Dashboard you created from the dropdown list.
o	Adjust the size and layout of the component as needed to fit the page design.
6.	Adjust Component Settings:
o	You can customize settings such as width, height, and visibility.
o	If needed, use the Rich Text Editor to add text or descriptions around the dashboard component.
7.	Preview and Publish:
o	Use the Preview button to see how the dashboard looks on the page.
o	Make any final adjustments if necessary.
o	Once satisfied, click Publish to make the changes live.
8.	Verify the Dashboard:
o	After publishing, check the live site to ensure that the dashboard is displaying correctly and that all data is accurate.
Key Tips
•	Responsive Design: Ensure the dashboard displays well on various devices and screen sizes.
•	User Permissions: Make sure users accessing the site have the necessary permissions to view the dashboard data.
•	Performance: Monitor the page’s performance to ensure the dashboard does not cause any loading issues.
This process will help you integrate your dashboard into the Salesforce Experience Builder, showcasing your skills in both dashboard creation and page design.


