
# 🛡️ GigShield India
### *Protecting the Working Hour, Not Just the Worker*

> **Parametric Income Protection Insurance for India's 15 Million Gig Workers**

[![Java](https://img.shields.io/badge/Java-Spring%20Boot-orange?style=for-the-badge&logo=java)](https://spring.io/projects/spring-boot)
[![React](https://img.shields.io/badge/Frontend-React%20PWA-blue?style=for-the-badge&logo=react)](https://reactjs.org/)
[![AWS](https://img.shields.io/badge/Cloud-AWS-yellow?style=for-the-badge&logo=amazonaws)](https://aws.amazon.com/)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

---

## 🚨 The Problem

In India's gig economy, a delivery partner's **income is tied to being on the road.**

When a Zomato server crashes at peak hour, or a Blinkit zone is blocked by a local rally — the worker loses **30% of their daily wage** with zero recourse.

Existing insurance covers:
- ✅ Accidents
- ✅ Health emergencies
- ✅ Vehicle damage

But **nothing** protects the **"empty pocket"** caused by external, uncontrollable disruptions.

> GigShield was built to protect the **working hour** — not just the person or the vehicle.

---

## 💡 What is GigShield?

**GigShield** is a **parametric insurance platform** that triggers automatic income-loss payouts when external, verifiable events disrupt a gig worker's ability to earn.

No paperwork. No waiting. **Data triggers the payment.**

---

## ⚙️ Core Features

### 🔐 Verification-First Login
Workers log in via **OAuth** using their existing delivery partner credentials (Zomato / Swiggy / Amazon) to verify their active partner status. No fake accounts.

### 📜 The Smart Contract Disclaimer
Upon every login, users accept a legally-binding Smart Contract:
> *"This platform covers ONLY income loss from external disruptions. It strictly excludes medical bills, life insurance, accident coverage, and vehicle repairs."*

### 💳 Weekly Subscription Tiers

| Tier | Weekly Cost | Coverage Level |
|------|------------|----------------|
| 🌱 Eco | ₹49 / week | Basic coverage |
| ⭐ Standard | ₹99 / week | Enhanced coverage |
| 👑 Elite | ₹199 / week | Maximum coverage |

*Protection that costs less than a few cups of chai per week.*

### ⚡ Automatic Parametric Triggers

The system auto-activates payouts when:

| Event | Trigger Condition |
|-------|------------------|
| 🌡️ Extreme Heat | Temperature > 42°C sustained |
| 🌧️ Heavy Rain | IMD red/orange alert active in zone |
| 📱 App Server Crash | Delivery platform down for community |
| 🚧 Rally / Strike | Verified by R.A.V.E. Engine |
| 🌉 Rare Events | Human-verified Special Request Portal |

### ⏱️ The 1-Hour Promise
Verified funds hit the worker's **UPI / IMPS account in under 60 minutes.**

---

## 🧠 How It Works

```
Worker Active in Zone
        ↓
External Event Detected (Weather API / App Heartbeat / R.A.V.E.)
        ↓
Zone-Level Validation (affects GROUP, not just individual)
        ↓
GPS Cross-Reference → Fraud Check (no ghosting)
        ↓
Parametric Payout Calculated (based on disruption duration)
        ↓
UPI Transfer Initiated ⚡ < 60 Minutes
```

---

## 🔧 Technology Stack

### Backend
- **Java (Spring Boot)** — Core microservices & REST APIs
- **Apache Kafka** — Real-time event streaming
- **PostgreSQL** — Transactional data storage
- **Redis** — Caching & session management
- **Apache Flink** — Stream processing for fraud detection

### Frontend
- **React.js (PWA)** — Mobile-first Progressive Web App
- **Tailwind CSS** — Styling
- **Firebase Cloud Messaging** — Push notifications & risk alerts
- **Workbox** — Offline service worker support

### AI / ML & Verification
- **TensorFlow Lite** — On-device zone prediction
- **Deeplearning4j** — Java-native ML models
- **R.A.V.E. Engine** — Rally & Anomaly Verification Engine (Google News API + Twitter/X API)

### External APIs
- **OpenWeatherMap API + IMD API** — Real-time hyper-local weather
- **Google Maps Platform API** — GPS zone mapping & geofencing
- **Twitter/X API v2** — Local trend scanning for strikes/protests

### Payments
- **Razorpay UPI API** — Sub-60-minute payouts
- **IMPS Integration** — Instant bank transfers

### Security & Smart Contracts
- **OAuth 2.0 + JWT** — Delivery partner authentication
- **Solidity + Web3j** — Immutable smart contract disclaimer on Ethereum
- **IPFS** — Decentralized disclaimer hash storage

### Infrastructure
- **AWS (EC2, S3, RDS, Lambda)** — Cloud hosting
- **Docker + Kubernetes** — Container orchestration
- **Jenkins** — CI/CD pipeline
- **Terraform** — Infrastructure as Code

### Monitoring
- **ELK Stack** — Centralized logging
- **Prometheus + Grafana** — Performance dashboards
- **Sentry** — Error tracking

---

## 🛡️ R.A.V.E. — Rally & Anomaly Verification Engine

Our proprietary verification system for non-weather disruptions:

1. Worker submits disruption claim from affected zone
2. AI scans **Google News API** for local event keywords
3. Cross-references **Twitter/X local trends** in real-time
4. Applies **Consensus Model** — multiple API sources must agree
5. **Zone-level validation** — must affect a group, not an individual
6. GPS cross-reference checks worker is actually in the disrupted zone
7. ✅ Payout triggered or ❌ Claim flagged for human review

---

## 🚫 Fraud Prevention: Anti-Ghosting System

**"Ghosting"** = A rider claims a loss in Zone A but drives to Zone B to work.

GigShield prevents this by:
- Real-time **GPS tracking** cross-referenced with delivery platform's **Active Service status**
- **Geofencing** via Google Maps — payout only if worker stays in disrupted zone
- Apache Flink **stream processing** detects anomalous movement patterns instantly

---

## 📱 Screenshots

> *Coming soon — UI in active development*

---

## 🚀 Getting Started

### Prerequisites
```bash
Java 17+
Node.js 18+
Docker & Docker Compose
PostgreSQL 15+
Redis 7+
```

### Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/gigshield-india.git
cd gigshield-india
```

### Backend Setup
```bash
cd backend
./mvnw clean install
docker-compose up -d   # starts PostgreSQL + Redis + Kafka
./mvnw spring-boot:run
```

### Frontend Setup
```bash
cd frontend
npm install
npm run dev
```

### Environment Variables
Create a `.env` file in `/backend/src/main/resources/`:
```env
OPENWEATHER_API_KEY=your_key
GOOGLE_MAPS_API_KEY=your_key
TWITTER_BEARER_TOKEN=your_key
RAZORPAY_KEY_ID=your_key
RAZORPAY_KEY_SECRET=your_secret
```

---

## 📊 What's Next

- [ ] 🔔 **Predictive Risk Alerts** — AI warns workers: *"Severe heatwave tomorrow; your shield is active"*
- [ ] 🏢 **B2B Pilot** — Built-in "Income Safety" toggle inside Zomato/Swiggy partner apps
- [ ] 📍 **Zone-Based Dynamic Pricing** — Premiums adjust based on historical zone volatility
- [ ] 🌍 **Multi-City Expansion** — Mumbai, Delhi, Bengaluru, Chennai, Hyderabad

---

## 🏆 Key Achievements

- **Trigger-Not-Claim Logic** — Data triggers payment, not paperwork
- **Sub-60-Minute Liquidity** — Fastest income payout in Indian insurtech
- **₹49/week Affordability** — Protection cheaper than a cup of chai
- **Zone-Level Validation** — Industry-first group-event verification system

---

## 🤝 Team

Built with ❤️ for India's gig workers at **[Hackathon Name]**

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

## ⚠️ Important Disclaimer

> GigShield is **strictly** an Income Loss Protection platform. It does **NOT** cover medical bills, life insurance, accident coverage, or vehicle repairs. All users must accept the Smart Contract terms upon registration.

---

*"We didn't build insurance. We built a safety net for the working hour."* 🛵⚡
