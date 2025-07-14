# SplunkSaviour – Smart Emergency Alert System for Colleges 🚨

SplunkSaviour is a Splunk-powered emergency alert system designed specifically for college campuses. It monitors simulated emergency events such as fires, panic button activations, medical emergencies, and network outages using dummy log files.

The system visualizes these incidents on real-time Splunk dashboards and automatically triggers alert emails to designated authorities (like wardens, IT teams, or medical staff).

No hardware or sensors required — all emergency events are simulated using CSV files, making this solution ideal for academic prototypes and demonstrations.

---

## 🎯 Key Features

- 📊 Real-time emergency monitoring dashboards
- 📁 Dummy log simulation (fire, panic button, medical, network)
- 📧 Automated email alerts to authorities
- 📈 Visual history of incidents and trend analysis
- ⚙️ Fully testable without physical hardware

---

## 🛠️ Technology Stack

- **Splunk Enterprise** or **Splunk Cloud**
- Dummy log files (`emergency_logs.csv`)
- Splunk:
  - Dashboards (XML)
  - Saved Searches (`savedsearches.conf`)
  - Event Types (`eventtypes.conf`)
  - Alert Actions (email notifications)

---

## 📂 Project Structure

```plaintext
SplunkSaviour/
├── README.md
├── default/
│   └── savedsearches.conf
├── data/
│   └── ui/
│       └── views/
│           └── emergency_dashboard.xml
├── sample_data/
│   └── emergency_logs.csv
├── screenshots/
│   └── dashboard_view.png
│   └── sample_alert_email.png
