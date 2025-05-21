# Cloud-Based Security Monitoring System Using Microsoft Sentinel

This project is a robust cloud-native SIEM solution using **Microsoft Sentinel**, designed to detect brute-force attacks, automate incident response, and provide real-time threat visualization.

## 🔧 Features
- 🔐 Brute-force attack detection (Azure AD, VMs)
- ⚡ Automated incident response with Logic Apps (Playbooks)
- 📊 Real-time dashboards via Workbooks
- 🌐 Scalable and cloud-native Azure architecture

## 🏗️ Architecture Components

| Component             | Description                                                  |
|----------------------|--------------------------------------------------------------|
| Microsoft Sentinel    | Central SIEM for detection and response                      |
| Azure AD, Office 365, VMs | Data sources for log collection                         |
| Log Analytics Workspace | Central log storage and query layer                        |
| Logic Apps (Playbooks) | Automates incident response (e.g., lock user, alert Teams) |
| Workbooks             | Visual dashboards for monitoring                             |

## 📜 Detection Rules

| Rule Name                     | Description                                             | KQL Logic Used |
|------------------------------|---------------------------------------------------------|----------------|
| Brute-force Login Detection  | Detects >5 failed logins in 5 mins from same IP         | ✅             |
| Unauthorized IP Login        | Detects logins from unknown IPs                         | ✅             |
| Repeated Login Failures      | Detects users with multiple rapid login failures        | ✅             |

## 📂 Files Included

- `Microsoft_Sentinel_Portfolio_Hema_Sundar.docx` – Full documentation
- `detection-rule-brute-force.kql` – KQL rule for brute-force attempts
- `playbook-lock-user.json` – Logic App to lock user
- `playbook-alert-teams.json` – Logic App to alert via Microsoft Teams
- `architecture-diagram.png` – System design diagram (optional)

## 🛣️ Roadmap

- [x] Brute-force attack detection using KQL
- [x] Incident response automation using Logic Apps
- [x] Custom dashboards with Workbooks
- [ ] Integration with External Threat Intelligence
- [ ] ML-based Anomaly Detection
- [ ] AWS/GCP log ingestion support

## 📌 Author

**Challa Hema Sundar Yadav**  
🔗 [GitHub Profile](https://github.com/monkeydsundar/sundar)

---

Licensed under MIT. Inspired by Microsoft documentation and real-world cybersecurity practices.
