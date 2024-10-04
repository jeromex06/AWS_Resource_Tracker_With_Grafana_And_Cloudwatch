# AWS Resource Tracker with Grafana and CloudWatch

This project is designed to monitor AWS resources using Grafana and CloudWatch. It provides a visual representation of key AWS metrics, helping you track and manage your resources more effectively.

# **Features**

\- Monitors AWS resources such as EC2 instances, IAM users, RDS instances, etc.

\- Visualizes CloudWatch metrics in Grafana.

\- Customizable dashboards and alerts for monitoring.

# **Prerequisites**

\- AWS account with CloudWatch enabled.  
\- AWS CLI installed and configured.  
\- Grafana installed on your Ubuntu system.  
\- AWS IAM role or access key with the necessary permissions to access CloudWatch.

# **Installation**

## **Step 1: Set up AWS CLI**

Make sure the AWS CLI is installed and configured with the necessary permissions. Run the following to configure it:

*aws configure*

Enter your AWS access key, secret key, region, and output format.

## **Step 2: Set up Grafana**

If you haven’t already installed Grafana, follow these instructions:

1\. Download and install Grafana from the official website: https://grafana.com/grafana/download.  
2\. Start the Grafana server:

*sudo systemctl start grafana-server*

3\. Open Grafana in your browser at http://localhost:3000.

## **Step 3: Configure AWS CloudWatch Data Source in Grafana**

1\. Log in to Grafana and go to \*\*Configuration \> Data Sources\*\*.  
2\. Add \*\*CloudWatch\*\* as a data source.  
3\. Enter your AWS credentials (Access Key, Secret Key, Region).

## **Step 4: Import Dashboard**

1\. Export your Grafana dashboard configuration as JSON.  
2\. Save the JSON file locally.  
3\. You can import the grafana\_dashboard.json from this repository into Grafana by:  
\- Navigating to \*\*Create \> Import Dashboard\*\* in Grafana.  
\- Uploading the JSON file.

# **Usage**

\- After setup, navigate to your Grafana dashboard to view AWS resource metrics.  
\- Add additional AWS services or CloudWatch metrics by customizing the dashboard.

