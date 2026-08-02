# Soldier Health & Fitness Monitoring System

A centralized, web-based platform to digitally record, track, and evaluate the health status, physical fitness, and medical history of soldiers — enhanced with **AI/NLP-driven medical note risk-ranking** and **sentiment-based morale tracking**.

## 📌 Problem Statement

Defence units currently maintain soldiers' medical checkups, injury history, and fitness scores through paper registers or disconnected spreadsheets. This leads to:
- Duplicated or misplaced records
- Slow retrieval of a soldier's health history
- No centralized alert system for follow-up checkups or low fitness scores
- No structured way to gauge soldiers' mental well-being / morale

## 🎯 Objectives

- Centralized digital system for soldiers' health and fitness data
- Role-based access for soldiers, medical officers, commanding officers, and administrators
- NLP-based parsing of medical officers' free-text notes to auto-extract symptoms/risk keywords and rank soldiers by health-risk priority
- NLP sentiment analysis on soldier well-being logs to track morale trends over time
- Automated dashboards, reports, and notifications to support faster, data-driven decisions

## ✨ Key Features / Modules

| Module | Description |
|---|---|
| User Authentication | Secure, role-based login for all user types |
| Soldier Profile Management | Core profile: personal details, service number, rank, unit |
| Health Monitoring | Vital signs, BMI, and general health status tracking |
| Fitness Tracking | Running time, push-ups, sit-ups, endurance score logging |
| Medical History | Chronological record of checkups, treatments, injuries |
| **Intelligent Medical Note Parser (NLP)** | Extracts symptoms/risk keywords from free-text medical notes and ranks soldiers by health-risk priority |
| **Morale Sentiment Tracker (NLP)** | Classifies soldier well-being log entries as positive/neutral/negative and visualizes morale trends over time |
| Dashboard & Reports | Consolidated, role-specific summaries and readiness reports |
| Notifications | Alerts for pending checkups, high-risk flags, and declining morale |

## 🧠 AI/NLP Enhancements

This project extends a traditional CRUD-based health monitoring system with two AI modules:

1. **Medical Note Risk Ranking** — inspired by resume-screening NLP techniques, this module parses free-text medical notes to extract context-aware risk indicators, ranking soldiers so medical officers can prioritize the highest-risk cases first.
2. **Morale Sentiment Tracking** — inspired by social-media sentiment analysis techniques, soldiers submit periodic well-being logs which are classified (positive/neutral/negative) and visualized as trends, triggering alerts on sustained negative sentiment for early psychological intervention.

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | HTML, CSS, Bootstrap, JavaScript |
| Backend | Python (Flask) |
| Database | MySQL |
| NLP / AI | Python (spaCy / NLTK, scikit-learn) |
| Visualization | Chart.js |

## 👥 Users of the System

- **Soldier** – views own health, fitness, and well-being history
- **Medical Officer** – records checkups, reviews risk-ranked notes
- **Commanding Officer** – reviews unit readiness dashboards and reports
- **Administrator** – manages users and system configuration

## 🚀 Getting Started

```bash
# Clone the repository
git clone https://github.com/<your-username>/soldier-health-fitness-monitoring-system.git
cd soldier-health-fitness-monitoring-system

# Create virtual environment
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Configure MySQL database credentials in config.py

# Run the application
python app.py
```

## 📂 Project Structure

```
soldier-health-fitness-monitoring-system/
├── app.py
├── config.py
├── requirements.txt
├── static/
│   ├── css/
│   └── js/
├── templates/
├── models/
├── nlp/
│   ├── medical_note_parser.py
│   └── sentiment_tracker.py
└── database/
    └── schema.sql
```

## 🔮 Future Enhancements

- Integration with wearable fitness devices
- Dedicated mobile application
- Predictive analytics for health risk forecasting
- Integration with external hospital/defence medical networks
- Multi-language support
- Biometric-based authentication

## 📄 License

This project is developed as an academic mini-project for educational purposes.

## 👤 Author

**[Your Name]**  
B.Tech CSE (AI/ML) | [Your University]
