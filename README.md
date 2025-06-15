# AuthGuardian 
## Splunk-Powered Authentication Log Analysis & Security Monitoring

### Introduction
Welcome to **AuthGuardian**, my hands-on project for practicing blue team security operations
using Splunk. This project is designed to help me (and anyone else interested) develop real
world skills in analyzing authentication logs, detecting threats, and automating incident response
workflows. I built it to bridge the gap between theory
and practice, and to showcase my ability to work with industry-standard tools.

## What did I learn and do?
- Analyzed 1,000+ Daily Authentication Events.
- Detected and Investigated 5 Brute Force attempts in a day, this figure is based on the frequency of suspicious activity in my test
environment. It demonstrates my capability to identify and respond to threats, even at scale.
- Reduced False Positive Alerts by 40% (approxiamate), by refining detection rules and implementing whitelists, I significantly cut
down on unnecessary alerts. This makes the security team more efficient and focused on real issues.
- Developed 2 Dashboards, building multiple dashboards shows my proficiency in data visualization and my commitment to making security data accessible and actionable.
- Automated 2 Security Alerts, automating key alerts means faster response times and less manualwork, which are crucial in a fast-paced security environment.

## What It Consists Of!
### 1. Log Analysis and Visualization
At the heart of **AuthGuardian** is **Splunk**, which I use to ingest, search, and visualize
authentication logs. Iʼve set up custom dashboards that display login trends, user
activity, and failed attempts. This helps me quickly spot patterns or anomalies—like
unexpected spikes in login attempts—that might indicate a security issue. 

### 2. Threat Detection and Alerting
- **AuthGuardian** includes a suite of Splunk queries designed to detect suspicious activity, such as repeated failed logins from a single IP or user. These queries automatically generate alerts when a potential brute force attack is detected.
- Iʼve refined the detection logic customized to the available data, reducing false positives by focusing on real
indicators of compromise. This makes the alerts more actionable and reduces unnecessary distractions for security teams.
 
### 3. Automation and Incident Response
- To streamline incident response, Iʼve created automated playbooks within Splunk.
These playbooks trigger actions like blocking suspicious IPs, notifying security staff,
and generating incident reports—all without manual intervention.
- I document each incident in detail, including the steps taken to investigate and resolve
it. This ensures compliance and knowledge sharing within the team.

## How to Use
### To implement and adapt AuthGuardian for your environment, follow these steps:
- Upload Authentication Logs to Splunk
  - Navigate to the Splunk Web interface.
  - Click the "Add Data" or "Upload" button on the Splunk Home page.
  - Select your authentication log file (samLogs.log) from your local system. Splunk will process and index the data for analysis.
  - Once uploaded, ensure the data source is correctly identified and indexed for optimal performance.

- Execute Splunk Queries
  - Access the Splunk Search & Reporting app.
  - Copy and paste the relevant queries from the queries/ directory into the search bar.
  - Run each query to analyze authentication events, detect failed login attempts, and generate actionable insights.

- Explore Dashboards and Alerts
  - After running the queries, review the results in Splunk’s dashboard interface.
  - Customize and save dashboards to monitor key security metrics in real time.
  - Configure alerts as needed to notify you of suspicious activity or potential threats.

- Review Incident Reports and Playbooks
  - Examine the incident response documentation and playbook templates in the docs/ folder.

## Thanks for checking out AuthGuardian! If you have questions or feedback, feel free to reach out or contribute to the project.
