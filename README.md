### Metrix Dashboard Documentation

Introduction
The Metrix Dashboard is a modern and responsive dashboard built using React, Tailwind CSS, and Syncfusion. This documentation provides an overview of the project structure, setup instructions, and a brief explanation of the key components and their functionalities.

### Table of Contents

Project Structure
Installation
Usage
Components
Dashboard
Orders
Customers
Inventory
Conversations
Settings
Styling
Syncfusion Integration
Project Structure

metrix-dashboard/
├── public/
│ ├── index.html
│ └── ...
├── src/
│ ├── components/
│ │ ├── Charts/
│ │ ├── LineChart.jsx
│ │ ├── Pie.jsx
│ │ ├── SparkLine.jsx
│ │ ├── Stacked.jsx
│ │ ├── Dashboard.jsx
│ │ ├── Orders.jsx
│ │ ├── Customers.jsx
│ │ ├── Inventory.jsx
│ │ ├── Conversations.jsx
│ │ ├── Settings.jsx
│ │ ├── Sidebar.jsx
│ │ ├── Navbar.jsx
│ │ └── ...
│ ├── contexts/
│ │ ├── ContextProvider.js
│ ├── data/
│ │ ├── avatar.png/...
│ ├── pages/
│ │ ├── Charts/
│ ├ ├── Calender.jsx/
│ ├ ├── ColorPicker.jsx/
│ ├ ├── Customers.jsx/
│ ├ ├── Ecommerce.jsx/
│ ├ ├── Editor.jsx/
│ ├ ├── Employee.jsx/
│ ├ ├── index.jsx/
│ ├ ├── Orders.jsx/
│ ├──
│ │── App.css
│ ├── App.js
│ ├── index.css
│ ├── index.js
│ └── ...
├── package.json
└── ...

Installation
To get started with the Metrix Dashboard, follow these steps:

1.Clone the repository:
git clone <repository-url>
cd metrix-dashboard

2.Install dependencies:
npm install

3.Start the development server:
npm start

The application will be available at http://localhost:3000.

### Usage

Dashboard
The main dashboard provides an overview of key metrics, including sales, volume, customer statistics, marketing data, product status, and recent orders.

Orders
The Orders component displays a list of recent orders with their status (Pending, Completed).

Customers
The Customers component provides insights into customer data, including the number of active and total customers.

Inventory
The Inventory component shows the status of products, including active and total products.

Conversations
The Conversations component lists customer interactions and support requests.

Settings
The Settings component allows users to configure their preferences and account settings.

Components
Dashboard
Dashboard.jsx - Displays key metrics and statistics for the business.

Orders
Orders.jsx - Shows a list of recent orders and their status.

Customers
Customers.jsx - Provides insights into customer data.

Inventory
Inventory.jsx - Displays product status and inventory details.

Conversations
Conversations.jsx - Lists customer interactions and support requests.

Settings
Settings.jsx - Allows users to configure their preferences and account settings.

Styling
The application uses Tailwind CSS for styling. Custom styles are defined in the src/scss/volt.scss file. Tailwind's utility classes are used throughout the components to ensure a consistent and responsive design.

### Syncfusion Integration

Syncfusion components are used to create interactive and visually appealing charts and graphs.

Installation
Ensure that Syncfusion components are installed:
npm install @syncfusion/ej2-react-charts

Usage
Import and use Syncfusion components in your React components. For example:
import { ChartComponent, SeriesCollectionDirective, SeriesDirective } from '@syncfusion/ej2-react-charts';

const SalesChart = () => (
<ChartComponent>
<SeriesCollectionDirective>
<SeriesDirective dataSource={data} xName='x' yName='y' type='Column' />
</SeriesCollectionDirective>
</ChartComponent>
);

export default SalesChart;
