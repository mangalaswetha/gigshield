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

**GigShield covers one thing and one thing only:**
> ✅ **Income lost because an external, uncontrollable event stopped you from working.**

**GigShield does NOT cover — ever, under any circumstance:**
> ❌ Accidents or injuries
> ❌ Medical bills or hospitalisation
> ❌ Vehicle damage or repair
> ❌ Life insurance or death benefits
> ❌ Personal disputes or individual mechanical failures
> ❌ Anything caused by the worker's own actions

> *If the disruption is yours alone — it is not our trigger. If the disruption shut down your entire zone — that is exactly what we exist for.*

---

## 💡 What is GigShield?

**GigShield** is a **parametric income insurance platform** that pays out automatically when a verified, external, zone-level event — heavy rain, app server crash, rally, extreme heat — stops an entire community of workers from earning.

No paperwork. No waiting. **The external event triggers the payment.**

---

## ⚙️ Core Features

### 🔐 Verification-First Login
Workers log in via **OAuth** using their existing delivery partner credentials (Zomato / Swiggy / Amazon) to verify their active partner status. No fake accounts.

### 📜 The Non-Negotiable Smart Contract
Upon registration, users sign an **immutable on-chain smart contract** (Solidity + IPFS):

> *"GigShield pays ONLY when a verified external event — weather, platform outage, or civic disruption — prevents zone-level work. It will never pay for accidents, health, vehicle, or any personal incident. This cannot be changed after signing."*

This is signed once. Stored on Ethereum. No exceptions, no amendments.

### 💳 Weekly Subscription Tiers

| Tier | Weekly Cost | Coverage Level |
|------|------------|----------------|
| 🌱 Eco | ₹49 / week | Basic |
| ⭐ Standard | ₹99 / week | Enhanced |
| 👑 Elite | ₹199 / week | Maximum |

*Less than a few cups of chai. Matched to weekly payout cycles.*

### ⚡ What Triggers a Payout

| External Event | Trigger Condition |
|----------------|------------------|
| 🌡️ Extreme Heat | Temperature > 42°C sustained in zone |
| 🌧️ Heavy Rain | IMD red/orange alert active in zone |
| 📱 App Server Crash | Delivery platform down — community-wide |
| 🚧 Rally / Strike / Bandh | Verified by R.A.V.E. Engine |
| 🌉 Rare Civic Events | Human-verified Special Request Portal |

### ⏱️ The 1-Hour Promise
Verified funds hit the worker's **UPI / IMPS account in under 60 minutes.**

---

## 🧠 How It Works

```
Worker Active in Zone
        ↓
External Event Detected (Weather API / App Heartbeat / R.A.V.E.)
        ↓
Zone-Level Validation → must affect the GROUP, not one individual
        ↓
Behavioral Integrity Score → Fraud & Spoofing Check
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
- **Solidity + Web3j** — Immutable smart contract on Ethereum
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

Our proprietary verification system for non-weather external disruptions:

1. Worker reports disruption from affected zone
2. AI scans **Google News API** for zone-specific event keywords
3. Cross-references **Twitter/X local trends** in real-time
4. Applies **Consensus Model** — multiple sources must agree
5. **Zone-level validation** — must affect a group, not an individual
6. GPS cross-reference confirms worker is inside the disrupted zone
7. ✅ Payout triggered or ❌ Claim sent to human review

---

## 🚫 Fraud Prevention: Anti-Ghosting System

**"Ghosting"** = Claiming a zone disruption while secretly working in another zone.

GigShield prevents this by:
- Real-time **GPS tracking** cross-referenced with the platform's **Active Service status**
- **Geofencing** via Google Maps — payout only valid inside the disrupted zone
- Apache Flink **stream processing** detects anomalous movement patterns instantly

---

## 🔐 Adversarial Defense & Anti-Spoofing Strategy

> **Threat:** A coordinated syndicate of 500 delivery workers used GPS-spoofing apps — organized via Telegram — to fake zone presence during red-alert weather, draining a competitor's liquidity pool within hours.
>
> **Our answer: We never trusted GPS alone.**

### 1. Differentiating a Genuine Stranded Worker from a Bad Actor

Our **Behavioral Integrity Score (BIS)** compares 6 passive device signals in real-time:

| Signal | Genuine Worker | GPS Spoofer |
|--------|---------------|-------------|
| **Accelerometer / Gyroscope** | Vibration of a stationary bike in rain | Perfectly flat — phone resting at home |
| **Battery Drain Rate** | High — GPS active, poor signal in storm | Normal — device idle |
| **Network Cell Tower ID** | Matches claimed zone's towers | Mismatches — home tower reported |
| **Platform Active Status** | "Online, 0 orders" — zone lockdown | "Offline" — never logged into app |
| **Historical Zone Pattern** | Delivered in this zone 3+ times this week | First appearance in this zone ever |
| **Claim Timing vs. Alert Timing** | Claim arrives 8–15 min after IMD alert | Claim arrives within 60 seconds — bot speed |

BIS produces a **trust score (0–100):** Score >70 → auto-payout. Score 40–70 → soft hold. Score <40 → flagged.

### 2. Detecting a Coordinated Fraud Ring

500 people spoofing simultaneously leaves a statistical fingerprint. Our **Ring Detection Engine** (Flink + Deeplearning4j) watches for:

- **Claim Burst Anomaly** — >15% of zone subscribers filing within 3 minutes = Surge Scrutiny Mode. Real disasters create staggered claims. Coordinated fraud creates synchronized spikes.
- **Telegram / Social Signal Cross-Reference** — R.A.V.E. scans for public group chatter matching zone + timing. Fraud coordination language triggers an immediate zone flag.
- **Device Fingerprint Clustering** — 30+ claims sharing the same spoofing app fingerprint = cluster quarantine.
- **Cell Tower Homogeneity** — Real workers in a storm hit different towers across a zone. A fraud ring from one neighbourhood hits 2–3 towers. Flink detects this instantly.
- **UPI Recipient Graph Analysis** — Post-payout, flagged accounts routing money to the same UPI handles within minutes are logged and escalated to the insurance pool auditor.

### 3. UX Balance — Never Punishing the Honest Worker

```
BIS Score > 70   →  ✅ Auto-Payout. No friction. < 60 minutes.

BIS Score 40–70  →  ⏳ Soft Hold (max 90 min).
                    One passive check: "Tap to confirm you're still in your zone."
                    No documents. No calls. One tap.

BIS Score < 40   →  🔍 Human Review (max 4 hours).
                    Worker notified: "Your claim is being verified.
                    You'll hear back within 4 hours." No silence.

Ring-Level Flag  →  🚨 Zone Quarantine.
                    All zone claims paused. Investigator assigned.
                    Innocent workers receive automatic 24hr
                    subscription extension as compensation.
```

**Network Drop Protection:** If a genuine worker loses GPS signal mid-event (common in heavy rain), their last verified zone location is held for **30 minutes** before any re-verification is needed.

> *The syndicate gets caught. Ravi gets paid. That is the only acceptable outcome.*

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
docker-compose up -d
./mvnw spring-boot:run
```

### Frontend Setup
```bash
cd frontend
npm install
npm run dev
```

### Environment Variables
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

- **Trigger-Not-Claim Logic** — External event triggers payment, not paperwork
- **Sub-60-Minute Liquidity** — Fastest income payout in Indian insurtech
- **₹49/week Affordability** — Protection cheaper than a cup of chai
- **Zone-Level Validation** — Industry-first group-event verification system
- **Behavioral Integrity Score** — Multi-signal fraud detection beyond GPS

---

## 🤝 Team

Built with ❤️ for India's gig workers at **GUIDEWARE DEV TRIALS HACKATHON**

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

## ⚠️ THIS PLATFORM COVERS EXTERNAL INCOME LOSS ONLY

> GigShield pays **only** when a verified, external, zone-level event stops you from working.
> It will **never** cover accidents, injuries, medical bills, vehicle damage, life insurance, or any personal incident — no matter the circumstance.
> This is not negotiable. It is written into an immutable smart contract signed at registration.

---

*"We didn't build insurance. We built a safety net for the working hour."* 🛵⚡
