# ⚖️ Weightage Labs - Risk Intelligence Platform

A comprehensive risk analytics platform featuring credit risk modeling, fraud detection, VC analytics, and forensic audit capabilities.

🔗 **Live Demo**: [https://vramesh45.github.io/weightagefraudlab](https://vramesh45.github.io/weightagefraudlab)

---

## 🎯 Features

### 📉 Credit Risk Module
- **PD (Probability of Default)** calculation using logistic regression
- **LGD (Loss Given Default)** estimation with recovery analysis
- **EAD (Exposure at Default)** tracking
- **ECL (Expected Credit Loss)** - IFRS 9 compliant
- Interactive staging migration analysis
- Historical portfolio performance tracking
- RAROC (Risk-Adjusted Return on Capital) metrics

### 🛡️ Fraud Detection
- Real-time anomaly scoring engine
- Multi-factor fraud indicators (velocity, device, behavior)
- Live fraud feed with risk classifications
- Pattern recognition and alert system
- Historical fraud trend analysis

### 📊 VC Analytics
- Automated KYC verification and scoring
- Financial health analysis
- Portfolio company performance tracking
- Risk assessment across multiple dimensions
- Due diligence report generation

### 🔬 Forensic Audit
- AI-powered expense anomaly detection
- Legal fee analysis and benchmarking
- Fraud pattern identification
- Compliance tracking
- Audit trail documentation

---

## 🚀 Technology Stack

- **Frontend**: React 18 (via CDN)
- **Styling**: Custom CSS with design system
- **Charts**: Custom SVG-based data visualizations
- **Fonts**: JetBrains Mono + Sora (Google Fonts)
- **Deployment**: GitHub Pages
- **Build**: None required - single HTML file

---

## 📦 Installation

### Quick Start (Local Development)

```bash
# Clone the repository
git clone https://github.com/vramesh45/weightagefraudlab.git

# Navigate to the directory
cd weightagefraudlab

# Open in browser (option 1: direct)
open index.html

# Or use a local server (option 2: Python)
python3 -m http.server 8000
# Visit: http://localhost:8000

# Or use Node.js (option 3: npx)
npx serve .
```

### Deployment to GitHub Pages

1. Go to **Settings** → **Pages**
2. Under **Source**, select **Deploy from a branch**
3. Select branch: `main`, folder: `/ (root)`
4. Click **Save**
5. Your site will be live at: `https://vramesh45.github.io/weightagefraudlab`

---

## 🎨 Customization

### Update Branding

Edit `index.html`:

```javascript
// Line 2193-2194: Company name
<div style={{fontSize:14,fontWeight:700,color:C.white,letterSpacing:".12em"}}>YOUR COMPANY</div>
<div style={{fontSize:9,color:C.cyan,letterSpacing:".22em"}}>TAGLINE</div>

// Line 6: Page title
<title>Your Company - Risk Intelligence Platform</title>

// Line 2250: Footer
<span style={{color:C.cyan}}>YOUR PLATFORM NAME · v2.0</span>
```

### Modify Color Scheme

Lines 31-36 contain the design tokens:

```javascript
const C = {
  bg:"#05080f",      // Main background
  panel:"#080d18",   // Panel background
  green:"#00e5a0",   // Success color
  cyan:"#20d0e0",    // Primary accent
  blue:"#4a9eff",    // Secondary accent
  // ... modify as needed
};
```

---

## 📊 Module Details

### Credit Risk Calculations

**PD Model (Logistic Regression)**:
```
PD = 1 / (1 + e^(-z))
where z = β₀ + β₁(age) + β₂(income) + β₃(dti) + β₄(defaults) + ...
```

**ECL Calculation (IFRS 9)**:
```
ECL = PD × LGD × EAD × Discount Factor
```

**RAROC**:
```
RAROC = (Expected Return - Expected Loss) / Economic Capital
```

### Fraud Scoring

Multi-factor model considering:
- Transaction velocity patterns
- Device fingerprint anomalies
- Behavioral deviations
- Geographic inconsistencies
- Historical fraud patterns

Score ranges:
- 0-20: Clean
- 20-40: Low risk
- 40-60: Medium risk
- 60-80: High risk
- 80-100: Critical

---

## 🔒 Security & Compliance

⚠️ **Important Disclaimers**:

1. **Demonstration Only**: This platform is for demonstration and educational purposes
2. **Not Licensed**: Not a licensed financial institution or advisory service
3. **No Real Data**: Do not process real customer PII or financial data
4. **Consult Professionals**: Always consult qualified professionals for actual risk decisions

**Data Privacy**:
- All calculations run client-side (browser)
- No data transmitted to external servers
- No cookies or tracking (unless you add analytics)

---

## 📈 Performance

- **Bundle Size**: ~250KB total (including all dependencies)
- **Load Time**: <1 second on modern connections
- **Runtime**: Pure client-side, no backend required
- **Browser Support**: All modern browsers (Chrome, Firefox, Safari, Edge)

---

## 🛠️ Development Roadmap

Potential enhancements:

- [ ] Real-time data integration (API connectors)
- [ ] User authentication system
- [ ] Database backend for persistence
- [ ] Advanced ML models (Python backend)
- [ ] Multi-currency support
- [ ] Export to Excel/CSV functionality
- [ ] Mobile-responsive improvements
- [ ] Dark/Light theme toggle

---

## 📝 License

This project is provided as-is for demonstration purposes.

**Usage Terms**:
- ✅ Personal portfolio use
- ✅ Educational purposes
- ✅ Internal company demos (with proper disclaimers)
- ❌ Production use without proper licensing
- ❌ Processing real customer data
- ❌ Financial advisory services

---

## 👨‍💻 Author

**Varun Ramesh**
- Credit & Risk Professional
- 5+ years in Risk Analytics
- ICE Clear Europe (NYSE)

---

## 🙏 Acknowledgments

Built with:
- [React](https://react.dev/) - UI framework
- [JetBrains Mono](https://www.jetbrains.com/lp/mono/) - Developer font
- [Sora](https://fonts.google.com/specimen/Sora) - UI font

---

## 📧 Contact

For questions, collaboration, or feedback:

- **Email**: [your.email@example.com]
- **LinkedIn**: [Your LinkedIn Profile]
- **Portfolio**: [Your Portfolio URL]

---

## ⚖️ Risk Disclosure

All models, scores, and calculations are for **demonstration purposes only**. This platform is **not a licensed financial institution**. Always consult qualified professionals before making financial or risk management decisions.

---

**Last Updated**: March 2026  
**Version**: 2.0  
**Status**: 🟢 Active Development
