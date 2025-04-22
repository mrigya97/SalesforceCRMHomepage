# Project 2: Digital Experience and Product Catalog Setup

> **Note:** This is the continuation of **SalesforceCRM Project 1**, which is available in the **SalesforceCRM** repository.

## 1. Enabling Digital Experience

### 1.1 Create a Site and Template
- **Log in**: Access your Salesforce Developer Org.
- **Navigate to Experience Cloud**: Go to `Setup > Experience Cloud > All Sites`.
- **Create a New Site**:
  - Select **Customer Service template**.
  - Name and create the site following the prompts.
- **Access the Site**: Click **View Site** after creation to access and start setup.

### 1.2 Workspace Configuration Under Builder
- **Open Builder**: Navigate to `Setup > Experience Cloud > All Sites`, then click **Builder** for the newly created site.
- **Configure Workspace**: Customize the workspace layout to align with the company’s branding and functional requirements.

### 1.3 Rich Text Editor and Autocomplete Search
- **Rich Text Editor**: Add this component as needed through **Page Components**.
- **Autocomplete Search**: Add this component to enable users to quickly search for products or information.

### 1.4 Theme Configuration
- **Theme Settings**:
  - Go to **Theme Settings** and customize the theme to reflect your company’s branding (colors, fonts, etc.).

### 1.5 Administration Settings
- **Configure Settings**: Navigate to **Administration** under site settings to configure access, permissions, and other administrative settings.

### 1.6 Theme and Font Configuration
- **Return to Theme Settings**: Adjust fonts, colors, and styles according to your company’s branding guidelines.

---

## 2. Products List and Catalog Page Creation

### 2.1 Clone Products List View
- **Go to Salesforce Setup**:
  - Navigate to `Object Manager > Products`.
  - Click on **List Views** and find the default Products list view.
  - Click **Clone** to create a new list view.
- **Add Filters**: Customize filters to match your requirements (e.g., by category, availability).

### 2.2 Drag the List to the Page Using Record List Component
- **Open Experience Builder**: Go back to the Builder in the site.
- **Add Record List Component**:
  - Drag the **Record List** component onto the page where you want the products list to appear.
  - Configure the component to use the newly cloned list view.
  - Adjust the display settings to **Compact mode** for a streamlined look.

### 2.3 Create Product Catalog Page
- **Create a New Page**:
  - In the Builder, select **New Page** and choose **Object Page**.
  - Use the **Rich Content Components** to add details about products.
- **Customize Header Properties** (Optional): Adjust header properties in the Record List settings if needed for better visibility and navigation.

### 2.4 Add Other Components
- **Ask a Question**: Include a component that allows users to submit questions or requests.
- **Customer Contact**: Add a component for customer contact options or forms.

### 2.5 Create and Add Dashboard
- **Create Report**:
  - Go to **Reports & Dashboards > Reports** and create a report to track key product metrics.
- **Create Dashboard**:
  - Go to **Reports & Dashboards > Dashboards** and create a dashboard.
  - Add components to visualize key data (e.g., top products, sales metrics).
- **Drag Dashboard to the Page**:
  - In the Builder, drag the dashboard component to your page.
  - Use the **Roll-Up Summary** options if needed to include data from related records.
  - Adjust pixel size and layout for optimal display.

---

## Final Steps

### 3.1 Review and Test
- Ensure all components are working as expected and the layout aligns with the company’s branding and functional needs.
- Perform testing to verify that the site and product catalog meet all requirements.

### 3.2 Publish
- Once everything is configured and tested, **publish** the site for users to access.

---

## Creating the Product List

### 4.1 Create or Customize the Product List View
- **Log In**: Access your Salesforce Developer Org.
- **Navigate to Object Manager**:
  - Go to `Setup > Object Manager > Product (or Products if using a different name)`.
- **Create or Clone a List View**:
  - Select **List Views**.
  - If you want to create a new list view, click **New**.
  - If you want to clone an existing list view, select the existing view and click **Clone**.
- **Configure the List View**:
  - Name the list view (e.g., "Product List View").
  - Set the filter criteria to include the products you want to display.
  - Choose the fields to display in the list view (e.g., Product Name, Price, Quantity).
  - Save the list view.

### 4.2 Implementing the Product List on the Homepage
- **Access Experience Builder**:
  - Go to `Setup > Experience Cloud > All Sites`.
  - Find your site and click **Builder**.
- **Add the Product List to the Homepage**:
  - Open the **Homepage** in Experience Builder.
  - Drag the **Record List** component onto the desired section of the homepage.
  - Configure the **Record List** component to use the Product object or the list view you created earlier.
- **Customize the Page Layout**:
  - Adjust layout and style using **Page Properties** and **Style** options.
  - Ensure the product list is visually appealing and easy to navigate.
- **Add Additional Components**:
  - Add **Search** or **Filter** components to enhance functionality.
  - Consider adding **Call to Action** or **Promotional Banners** to highlight featured products.

### 4.3 Publish Your Changes
- **Preview the Page**: Use the Preview option to see how the product list looks on the homepage.
- **Publish**: Once satisfied, click **Publish** to make your changes live.

### 4.4 Testing
- **Test Functionality**: Ensure the product list displays correctly and that users can interact with it as expected.
- **Check Responsiveness**: Verify that the product list looks good on different devices (e.g., desktop, tablet, mobile).

---

## Sales Performance Dashboard

### 5.1 Components
1. **Sales Overview**:
   - **Chart Type**: Bar Chart
   - **Data**: Total Revenue by Product.
   - **Objective**: Show how much revenue each product has generated.
   
2. **Top Products**:
   - **Chart Type**: Pie Chart
   - **Data**: Revenue Distribution by Product Category.
   - **Objective**: Highlight which product categories are generating the most revenue.

3. **Sales Pipeline**:
   - **Chart Type**: Funnel Chart
   - **Data**: Opportunities by Stage.
   - **Objective**: Visualize the distribution of opportunities through various stages of the sales process.

### 5.2 Implementation Steps
1. **Create Custom Reports**:
   - **Total Revenue by Product**:
     - Go to `Reports > New Report`.
     - Select **Opportunities** report type.
     - Group by **Product Name** and summarize the **Amount** field for total revenue.
   - **Monthly Sales Trends**:
     - Similar report, but group by **Close Date** (monthly).
   - **Revenue Distribution by Product Category**:
     - Create a report summarizing revenue by **Product Category**.

2. **Build the Dashboard**:
   - Go to `Reports & Dashboards > Dashboards > New Dashboard`.
   - Add components:
     - **Bar Chart**: "Total Revenue by Product" report.
     - **Line Chart**: "Monthly Sales Trends" report.
     - **Pie Chart**: "Revenue Distribution by Product Category" report.
     - **Funnel Chart**: Opportunities by stage.

3. **Test and Refine**:
   - Review the dashboard for accuracy and usability.
   - Ensure data updates and visualizations reflect intended insights.

### 5.3 Steps to Add a Dashboard to a Salesforce Experience Builder Page
1. **Access the Experience Builder**:
   - Go to `Setup > Experience Cloud > All Sites`.
   - Click on **Builder** for your site.
2. **Add a Dashboard Component**:
   - Drag the **Dashboard** component from the **Components** panel onto your page.
3. **Configure the Dashboard Component**:
   - Select the **Sales Performance Dashboard** from the dropdown.
4. **Preview and Publish**:
   - Preview the page and click **Publish** once satisfied.


