<h1> AWS-CloudTrail-Log-Analysis</h1>
I try to confirm a breach by analyzing CloudTrail logs, identify any compromised AWS service, and find any data that was exfiltrated.


<h2>Description</h2>

- Scenario: Investigated unusual AWS account activity using CloudTrail logs and AWS CLI.

- Findings: Identified compromised account (Temp-User), privilege escalation into AdminRole, and exfiltration of sensitive data from an S3 bucket.

- Skills practiced: JSON parsing, AWS CLI, CloudTrail log analysis, S3 enumeration, IP threat intel lookups.


<h2>Tool Used</h2>
- AWS CLI

<h2>Environments Used </h2>

- Kali Linux
- VirtualBox

<h2>Walk-Through</h2>

<p align="center">
AWS CLI Setup: <br/>
<img src="https://i.imgur.com/KUAeYBM.png" height="80%" width="80%" alt="Cloud Breach"/>
<br />
<br />
Find Compromised User:  <br/>
<img src="https://i.imgur.com/ogbF05U.png" height="80%" width="80%" alt="Cloud Breach"/>
<br />
<br />
Parse Through Logs:  <br/>
<img src="https://i.imgur.com/zcbHb6D.png" height="80%" width="80%" alt="Cloud Breach"/>
<br />
<br />
Threat Actor Attempt to Access S3 Emergency Bucket:  <br/>
<img src="https://i.imgur.com/80CO2kQ.png" height="80%" width="80%" alt="Cloud Breach"/>
<br />
<br />
Threat Actor Assumes More Privileged Role:  <br/>
<img src="https://i.imgur.com/0z5TKJd.png" height="80%" width="80%" alt="Cloud Breach"/>
<br />
<br />
Threat Actor Extracts Information From S3 Bucket:  <br/>
<img src="https://i.imgur.com/nIKtVWF.png" height="80%" width="80%" alt="Cloud Breach"/>
<br />
<br />





<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
