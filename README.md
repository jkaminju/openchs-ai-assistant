# OpenCHS AI Assistant 🤖

**Intelligent Call Documentation for GBV & Child Protection Helplines**

[![Phase](https://img.shields.io/badge/Phase-1%20MVP%20Deployed-success)](https://github.com/jkaminju/openchs-ai-assistant)
[![Countries](https://img.shields.io/badge/Deployed-5%20Countries-blue)](https://github.com/jkaminju/openchs-ai-assistant)
[![Impact](https://img.shields.io/badge/Impact-16K%20Hours%2FMonth%20Saved-orange)](https://github.com/jkaminju/openchs-ai-assistant)
[![Award](https://img.shields.io/badge/Award-Runner--up%20MSIS%20549%20GenAI%20Fair-gold)](https://github.com/jkaminju/openchs-ai-assistant)

---

## 🏆 Award

**Runner-Up - Judges' Favorite**  
MSIS 549 GenAI & Agentic Fair, February 2026

---

## 📌 Overview

OpenCHS AI Assistant transforms how counselors document cases of gender-based violence (GBV) and child abuse across Africa. By automatically extracting structured information from natural conversations, it reduces documentation time by 60% and returns **16,000 hours monthly** to direct survivor care.

**Current Deployment:** 5 countries (Kenya, Uganda, Tanzania, Lesotho, Somalia) | 200+ counselors | 120,000+ calls monthly

---

## 🚨 The Problem

Call centers handling child abuse and GBV cases face critical challenges:

- **Administrative Burden**: Counselors spend **60-70% of call time** filling detailed forms instead of supporting survivors
- **Scale Challenge**: **120,000 calls monthly** means thousands of hours wasted on paperwork
- **Delayed Risk Detection**: Critical cases may not be flagged quickly enough
- **Service Gaps**: Every delayed response could mean a child remains in danger

**Impact:** Time spent on forms = Less time helping survivors when they need it most.

---

## ✨ The Solution

### Phase 1 MVP (Deployed)

**Intelligent Call Transcription & Auto-Form Filling**

- 🎯 **Auto-Extraction**: Extracts 19 structured fields from natural conversation
- ⚡ **Lightning Fast**: <1 second processing time
- 📊 **High Accuracy**: 91% average confidence score
- 💡 **Evidence-Backed**: Every field shows source quote + confidence level
- ⚠️ **Risk Detection**: Flags suicidal ideation, immediate danger, child abuse, threats
- ✅ **Human-in-Loop**: AI suggests, counselor reviews, one-click accept

### Key Features

| Feature | Description |
|---------|-------------|
| **Real-time Transcription** | Speech-to-text conversion of counselor-survivor conversations |
| **Structured Extraction** | Automatically populates demographics, incident details, risk assessment, support needs |
| **Risk Flagging** | Instant alerts for critical cases (suicidal ideation, immediate danger, child abuse) |
| **Evidence Citations** | Every extracted field includes source quote and timestamp |
| **Form Auto-Fill** | Suggests values with yellow highlights for counselor review |

---

## 🛠️ Technology Stack

### Phase 1 MVP

| Component | Technology |
|-----------|-----------|
| **Speech-to-Text** | OpenAI Whisper API |
| **AI Extraction** | Anthropic Claude API |
| **Backend** | FastAPI (Python) |
| **Frontend** | React + HTML/CSS |
| **Database** | PostgreSQL |
| **Deployment** | Production (5 countries) |

### Future Phases

- **Phase 2**: Multilingual translation (NLLB-200) for 10+ languages
- **Phase 3**: AI-powered quality assurance for supervisor review

---

## 📊 Impact Metrics

| Metric | Value |
|--------|-------|
| **Time Saved** | 16,000 hours/month returned to survivor care |
| **Efficiency Gain** | 60% reduction in documentation time |
| **Capacity Increase** | 40% more calls handled per counselor |
| **Form Completion** | Improved from 75% → 95% |
| **Processing Speed** | <1 second per call |
| **Confidence Score** | 91% average accuracy |
| **Fields Extracted** | 19 structured fields automatically |

---

## 🌍 Real-World Deployment

### Countries
- 🇰🇪 Kenya
- 🇺🇬 Uganda
- 🇹🇿 Tanzania
- 🇱🇸 Lesotho
- 🇸🇴 Somalia

### Users
- **200+ counselors** using the system daily
- **120,000+ survivors** receiving faster, better-documented care monthly

### Partners
- **UNICEF ESARO** - Regional Implementation
- **UNICEF Venture Fund** - Innovation Support
- **UNFPA** - GBV Prevention
- **GIZ** - Technical Partnership

---

## 🏗️ Architecture

```
┌─────────────────┐
│  Call Audio     │
│  (Live/Upload)  │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ OpenAI Whisper  │ ◄── Speech-to-Text
│      API        │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│   Transcript    │
│   (Text)        │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ Anthropic       │ ◄── Structured Extraction
│  Claude API     │     + Risk Detection
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  Extracted      │
│  Fields (JSON)  │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  PostgreSQL     │ ◄── Store Case Data
│   Database      │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  React UI       │ ◄── Counselor Reviews
│  Form Display   │     + Accepts Suggestions
└─────────────────┘
```

---

## 🎯 Extracted Fields (19 Total)

### Case Management
- Follow-up needed
- Follow-up date
- Counselor notes

### Incident Details
- Incident type
- Incident date
- Incident location
- Perpetrator relationship

### Risk Assessment
- Risk level (Low/Medium/High/Critical)
- Risk indicators
- Safety concerns

### Demographics
- Survivor name
- Survivor age
- Survivor gender
- Contact phone
- Location (district, village)

### Support Needs
- Immediate needs
- Referrals required
- Services needed

---

## ⚠️ Risk Detection

The system automatically flags high-risk indicators:

- 🚨 **Critical**: Suicidal ideation, immediate physical danger
- 🔴 **High**: Threats of violence, weapons involved, perpetrator has access
- 🟡 **Medium**: Escalating violence, child abuse indicators
- 🟢 **Low**: Standard case requiring follow-up

Each risk indicator includes:
- Severity level
- Suggested action
- Confidence score
- Source evidence (quote from transcript)

---

## 💻 Demo Workflow

1. **Select Sample Call** - Choose from pre-loaded demo cases
2. **Play Audio** - 2x speed playback available
3. **Process with AI** - Click button to extract fields
4. **View Results**:
   - Live transcript appears
   - Form auto-fills with yellow suggestions
   - Risk alerts show critical indicators
   - Analytics dashboard displays confidence scores
5. **Review & Accept** - Counselor reviews AI suggestions, accepts or edits
6. **Save Case** - Final case data stored in database

---

## 📈 Success Metrics

### MVP Demonstration (GenAI Fair)
- ✅ Extraction accuracy: **>91%**
- ✅ Processing latency: **<1 second**
- ✅ Zero false negatives on critical risks
- ✅ Runner-up award - Judges' Favorite

### Real-World Deployment
- ✅ **60% reduction** in documentation time
- ✅ **40% increase** in calls handled per counselor
- ✅ Form completeness: **75% → 95%**
- ✅ Deployed in **5 countries**
- ✅ Serving **120,000+ survivors monthly**

---

## 🚀 Future Roadmap

### Phase 2: Multilingual Support
- Real-time translation for 10+ African languages
- NLLB-200 integration
- Expand accessibility to non-English speakers

### Phase 3: AI Quality Assurance
- Automated supervisor review
- Call quality scoring
- Counselor performance insights
- Continuous improvement feedback

---

## 🤝 Contributing

This project is part of the OpenCHS (Open Case Handling System) ecosystem. For collaboration opportunities:

- **Technical Partners**: Contact for API integration
- **Deployment Partners**: Reach out for country-level implementation
- **Funding Partners**: Support expansion to additional countries

---

## 📄 License

This project is part of ongoing humanitarian work. Contact the OpenCHS team for usage and deployment inquiries.

---

## 👥 Team

**Developer**: James Kaminju  
**Institution**: University of Washington - MSIS Program  
**Course**: MSIS 549 - Generative AI & Agentic Systems  
**Quarter**: Winter 2026

---

## 🙏 Acknowledgments

- **Prof. Leo** - 549 Machine Learning Professor for support and knowledge dissemination - Amazing knowledge transfer skills**
- **UW MSIS Faculty** - Project guidance and support
- **UNICEF ESARO** - Regional partnership and deployment support
- **UNICEF Venture Fund** - Innovation funding and mentorship
- **UNFPA** - GBV prevention expertise
- **GIZ** - Technical implementation support
- **OpenCHS Team** - Platform and infrastructure


---

## 📞 Contact

For project inquiries: []

**James Kaminju - jkaminju@gmail.com / james.nganga@bitz-itc.com** - Serving children and families across Africa



---

## 🌟 Recognition

**MSIS 549 GenAI & Agentic Fair - Runner-Up (Judges' Favorite)**  
February 2026 | University of Washington

---

**Making life-saving services more accessible, efficient, and survivor-centered through AI.** 🌍💙
