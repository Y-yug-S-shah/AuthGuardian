# AuthGuardian
## Splunk-Powered Authentication Log Analysis & Security Monitoring

### Introduction
Welcome to **AuthGuardian**, my hands-on project for blue team security operations practice using Splunk.
This project is meant to assist me (and anyone else who cares) in building real world skills at analyzing authentication logs,
determining threats, and automating incident response workflows. I created it to close the gap between theory
and practice, and to demonstrate my skills at using industry-standard tools.

## What did I learn and do?
- Processed 1,000+ Daily Authentication Events.
- Identified 5 Brute Force attempts within a day, the count is referred based on the rate of suspicious activity within my test environment. It shows my ability to identify and react to threats even at scale.
- Cut False Positive Alerts by 40% (approximate), by sharpening detection rules and using whitelists, I greatly reduced down on pointless alerts. This improves the security team's efficiency and relevance to actual issues.
- Created 2 Dashboards, creating multiple dashboards indicates my experience with data visualization and my dedication to making security data actionable and visible.
- Automated 2 Security Alerts, automating important alerts translates into quicker response times and reduced manual labor, which are in high demand in a high-pressure security environment.

## What It Consists Of!
### 1. Log Analysis and Visualization
At the core of **AuthGuardian** is **Splunk**, which I leverage to ingest, search, and visualize
authentication logs. I have configured custom dashboards that show login trends, user
activity, and failed attempts. This allows me to easily see patterns or anomalies, such as
unusual spikes in attempts to log in, that could signal a security problem.

### 2. Threat Detection and Alerting
- **AuthGuardian** contains a set of Splunk queries aimed at monitoring for suspicious behavior, like multiple failed login attempts from one IP or user. They are designed to automatically trigger alerts upon the identification of a possible brute force attack.
- Iʼve optimized the detection logic tailored to the data available to minimize false positives through an emphasis on actual
indicators of compromise. This renders the alerts more actionable and saves security teams from unnecessary distractions.
### 3. Automation and Incident Response
- To automate incident response, I have developed automated playbooks in Splunk.
These automated playbooks initiate tasks such as blocking malicious IPs, alerting security personnel,
and producing incident reports—all without human intervention.
- I thoroughly document every incident along with the steps to investigate and close
it. This is done to maintain compliance and share knowledge among the team.

## How to Use
### To deploy and modify AuthGuardian in your environment, do the following:
- Upload Authentication Logs to Splunk
  - Go to the Splunk Web interface.
  - Click the "Add Data" or "Upload" button in the Splunk Home page.
  - Choose your authentication log file (samLogs.log) from your local machine. Splunk will index and process the data for analysis.
- After uploading, make sure the data source is properly named and indexed for maximum performance. 

- Run Splunk Queries
  - Open the Splunk Search & Reporting application.
  - Paste and copy the applicable queries from the queries/ directory into the search field.
  - Run each query to inspect authentication activity, identify failed logins, and produce actionable information.

- Investigate Dashboards and Alerts
  - Run the queries and inspect the results in Splunk's dashboard view.
  - Save and customize dashboards to watch for important security metrics in real-time.
  - Set up alerts if necessary to alert you to suspicious activity or possible threats.

- Check Incident Reports and Playbooks
  - Take a look at the incident response documentation and playbook templates under the docs/ directory.

## Thank you for visiting AuthGuardian. Should you have any questions or suggestions, feel free to reach out or contribute to the project.
