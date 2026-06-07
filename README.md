# 🧠 MindCare - AI-Powered Mental Health Application

[![React](https://img.shields.io/badge/React-18.0-blue?logo=react)](https://react.dev/)
[![Firebase](https://img.shields.io/badge/Firebase-Cloud-orange?logo=firebase)](https://firebase.google.com/)
[![Supabase](https://img.shields.io/badge/Supabase-PostgreSQL-green?logo=supabase)](https://supabase.com/)
[![Gemini API](https://img.shields.io/badge/Gemini-API-red?logo=google)](https://ai.google.dev/)
[![License](https://img.shields.io/badge/License-MIT-yellow)](LICENSE)

> **MindCare** είναι μια σύγχρονη εφαρμογή ψυχικής υγείας που χρησιμοποιεί τεχνητή νοημοσύνη και τη τεχνική RAG (Retrieval-Augmented Generation) για να παρέχει προσωπικευμένη ψυχολογική υποστήριξη.

---

## 📋 Περιεχόμενα

- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Εγκατάσταση](#-εγκατάσταση)
- [Χρήση](#-χρήση)
- [Δομή Έργου](#-δομή-έργου)
- [RAG Implementation](#-rag-implementation)
- [Συμβολή](#-συμβολή)
- [Άδεια](#-άδεια)

---

## ✨ Features

### 🤖 AI-Powered Chat
- **4 Διαφορετικοί AI Θεραπευτές:**
  - 🧠 **Dr. Nikos** (CBT - Γνωστική-Συμπεριφοριακή Θεραπεία)
  - 💚 **Dr. Maria** (ACT - Acceptance and Commitment Therapy)
  - 🧘 **Dr. Alex** (Mindfulness - Προσέγγιση βασισμένη σε Ενσυνειδησία)
  - 🌟 **Dr. Elena** (Psychodynamic - Ψυχοδυναμική Θεραπεία)

### 🔄 RAG Technology
- **Vector Embeddings** με Google Gemini API (768-dimensional)
- **Similarity Search** σε Supabase για προηγούμενες συνομιλίες
- **Knowledge Base** με θεραπευτικές τεχνικές
- **Context-Aware Responses** που θυμάται το ιστορικό του χρήστη

### 📊 Mood Tracking
- Καθημερινή παρακολούθηση διάθεσης (1-5 κλίμακα)
- Ιστορικό διάθεσης με οπτικοποίηση
- Heatmap 35 ημερών
- Δυναμικά χρώματα φόντου με βάση τη διάθεση

### 📝 Journal with Sentiment Analysis
- Γραφή προσωπικών σημειώσεων
- Αυτόματη ανάλυση συναισθημάτων (positive, negative, neutral)
- Εκπτώσιμη αναζήτηση με vector similarity
- Κρυπτογραφημένη αποθήκευση

### 🧘‍♀️ Mindfulness Module
- Οδηγόμενες ασκήσεις χαλάρωσης
- 5-4-3-2-1 Grounding Technique
- Body Scan Meditation
- Breathing Exercises

### 🆘 Crisis Support
- **SOS Button** για άμεση βοήθεια
- Σύνδεσμοι σε γραμμές έκτακτης ανάγκης
- Τεχνικές ψυχολογικής ανακούφισης

### 🎨 Modern UI/UX
- **Glassmorphism Design** με blur effects
- **Mobile-First Approach** για όλα τα μεγέθη οθόνης
- **Dark Mode Support**
- Smooth animations και transitions

### 🔐 Security & Privacy
- Firebase Authentication (Email/Password)
- Encrypted data storage
- User-specific data isolation
- GDPR compliant

---

## 🛠️ Tech Stack

### Frontend
- **React 18** - UI Library
- **React Hooks** (useState, useEffect, useContext)
- **CSS3** - Glass Morphism & Modern Design
- **Google Fonts (Inter)** - Typography

### Backend & Database
- **Firebase**
  - Authentication
  - Firestore (NoSQL Database)
  - Real-time Synchronization
  
- **Supabase**
  - PostgreSQL Database
  - pgvector Extension (for Vector Storage)
  - RPC Functions (match_memory, match_knowledge)

### AI & NLP
- **Google Gemini API**
  - LLM (Large Language Model)
  - Embedding Model (embedding-001 - 768 dimensions)
  - Prompt Engineering

### Development Tools
- **React Native with Expo** - Cross-platform development
- **Node.js & npm** - Package management
- **Vite/Create React App** - Build tools
- **VS Code** - IDE

---

## 📦 Εγκατάσταση

### Προαπαιτούμενα
- Node.js (v14 или выше)
- npm ή yarn
- Firebase Account
- Supabase Account
- Google Gemini API Key

### Βήματα

1. **Clone το repository:**
```bash
git clone https://github.com/YOUR_USERNAME/mindcare.git
cd mindcare
```

2. **Εγκατάστησε τις dependencies:**
```bash
npm install
```

3. **Δημιούργησε ένα `.env` αρχείο στη ρίζα του project:**
```env
REACT_APP_FIREBASE_API_KEY=your_firebase_api_key
REACT_APP_FIREBASE_AUTH_DOMAIN=your_firebase_auth_domain
REACT_APP_FIREBASE_PROJECT_ID=your_firebase_project_id
REACT_APP_FIREBASE_STORAGE_BUCKET=your_firebase_storage_bucket
REACT_APP_FIREBASE_MESSAGING_SENDER_ID=your_firebase_messaging_sender_id
REACT_APP_FIREBASE_APP_ID=your_firebase_app_id

REACT_APP_SUPABASE_URL=your_supabase_url
REACT_APP_SUPABASE_KEY=your_supabase_anon_key

REACT_APP_GEMINI_API_KEY=your_gemini_api_key
```

4. **Ξεκίνησε τον development server:**
```bash
npm start
```

5. **Άνοιξε το browser και πήγαινε στο:**
```
http://localhost:3000
```

---

## 💻 Χρήση

### Πρώτη Χρήση
1. Εγγραφή με email και password
2. Δημιουργία προφίλ (όνομα, ηλικία, χώρα)
3. Συμπλήρωση "Doctor Quiz" (10 ερωτήσεις)
4. Επιλογή AI θεραπευτή
5. Ξεκίνησε τη συνομιλία!

### Κύριες Λειτουργίες

#### Chat με AI
```javascript
// Ο χρήστης στέλνει μήνυμα
// MindCare:
// 1. Δημιουργεί embedding του μηνύματος
// 2. Αναζητά παρόμοια memories & knowledge
// 3. Συγκεντρώνει context
// 4. Δημιουργεί response με Gemini API
// 5. Αποθηκεύει τη συνομιλία για μελλοντική χρήση
```

#### Mood Tracking
- Κάνε κλικ στο "Mood" icon
- Επίλεξε τη διάθεσή σου (1-5)
- Δες το heatmap των τελευταίων 35 ημερών

#### Journal
- Κάνε κλικ στο "Journal" icon
- Γράψε τις σκέψεις/συναισθήματά σου
- Το σύστημα αναλύει αυτόματα τα συναισθήματα
- Αναζήτησε παλιές εγγραφές με vector similarity

---

## 📁 Δομή Έργου

```
mindcare/
├── public/
│   ├── index.html
│   └── favicon.ico
├── src/
│   ├── components/
│   │   ├── Chat/
│   │   ├── MoodTracker/
│   │   ├── Journal/
│   │   ├── Mindfulness/
│   │   └── SOS/
│   ├── hooks/
│   │   ├── useAuth.js
│   │   ├── useFirestore.js
│   │   └── useRAG.js
│   ├── utils/
│   │   ├── firebase.js
│   │   ├── supabase.js
│   │   ├── gemini.js
│   │   └── embeddings.js
│   ├── styles/
│   │   ├── global.css
│   │   ├── glassmorphism.css
│   │   └── variables.css
│   ├── App.js
│   └── index.js
├── .env
├── package.json
├── README.md
└── LICENSE
```

---

## 🧠 RAG Implementation

### Αρχιτεκτονική

```
User Input
    ↓
[Embedding Generation] → Google Gemini embedding-001 (768-dim)
    ↓
[Vector Similarity Search] → Supabase (match_memory, match_knowledge)
    ↓
[Context Augmentation] → Συγκέντρωση προηγούμενων συνομιλιών + τεχνικές
    ↓
[LLM Generation] → Gemini API δημιουργεί απάντηση
    ↓
[Memory Storage] → Αποθήκευση embedding σε Supabase για μελλοντική χρήση
    ↓
User Response
```

### Key Features

- **Match Memory**: Ανάκτηση 3 πιο παρόμοιων προηγούμενων συνομιλιών
- **Match Knowledge**: Ανάκτηση 2 πιο παρόμοιων θεραπευτικών τεχνικών
- **Similarity Threshold**: 0.5 (δυνατότητα προσαρμογής)
- **Context Window**: Τελευταίες 6 ανταλλαγές (αποφυγή token limits)

### Databases

**Firestore:**
```json
{
  "users/{uid}": {
    "name": "string",
    "email": "string",
    "profile": {...},
    "chatHistory": [...],
    "moodHistory": [...],
    "preferences": {...}
  }
}
```

**Supabase:**
```sql
-- chat_memory table
CREATE TABLE chat_memory (
  id UUID PRIMARY KEY,
  user_id TEXT,
  doctor_id TEXT,
  content TEXT,
  role TEXT,
  embedding vector(768),
  created_at TIMESTAMP
);

-- doctor_knowledge table
CREATE TABLE doctor_knowledge (
  id UUID PRIMARY KEY,
  doctor_id TEXT,
  content TEXT,
  embedding vector(768),
  created_at TIMESTAMP
);
```

---

## 🤝 Συμβολή

Το MindCare είναι open-source και υποδέχεται συμβολές! 

### Βήματα Συμβολής

1. **Fork το repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/mindcare.git
   ```

2. **Δημιούργησε ένα feature branch**
   ```bash
   git checkout -b feature/AmazingFeature
   ```

3. **Commit τις αλλαγές σου**
   ```bash
   git commit -m 'Add some AmazingFeature'
   ```

4. **Push το branch**
   ```bash
   git push origin feature/AmazingFeature
   ```

5. **Άνοιξε ένα Pull Request**

### Ιδέες Συμβολής

- [ ] Υποστήριξη περισσότερων γλωσσών
- [ ] Νέοι AI θεραπευτές με διαφορετικές προσεγγίσεις
- [ ] Integration με άλλα εργαλεία (Spotify for relaxation music)
- [ ] Mobile app με React Native
- [ ] Video call support με επαγγελματίες
- [ ] Advanced analytics dashboard
- [ ] AI-powered crisis detection

---

## 📊 Δεδομένα & Απόρρητο

MindCare **δεν συλλέγει ή πουλάει** τα προσωπικά δεδομένα των χρηστών.

- ✅ End-to-End Encrypted
- ✅ GDPR Compliant
- ✅ User data ownership
- ✅ No third-party data sharing

---

## 🧪 Testing

```bash
# Run tests
npm test

# Run tests with coverage
npm test -- --coverage

# Run integration tests
npm run test:integration
```

---

## 🚀 Deployment

### Firebase Hosting

```bash
# Install Firebase CLI
npm install -g firebase-tools

# Login to Firebase
firebase login

# Deploy
npm run build
firebase deploy
```

### Vercel

```bash
# Install Vercel CLI
npm install -g vercel

# Deploy
vercel
```

---

## 📚 Αναφορές & Έρευνα

Το MindCare βασίζεται σε πρόσφατη έρευνα για τη χρήση ΤΝ στην ψυχική υγεία:

- **Baiano et al. (2025)** - "Generative artificial intelligence mental health chatbots: A systematic review and meta-analysis of randomized controlled trials" - JMIR Mental Health
- **Gopal et al. (2026)** - "The promise and potential of generative artificial intelligence in mental health care: A Delphi expert consensus study"

---

## 🎯 Roadmap

- [ ] v1.1 - Προσθήκη video call με ψυχολόγο
- [ ] v1.2 - Integration με wearables (Apple Watch, Fitbit)
- [ ] v1.3 - Multi-language support (English, Spanish, German)
- [ ] v2.0 - Mobile app (iOS & Android)
- [ ] v2.1 - Group therapy sessions
- [ ] v3.0 - Enterprise version για χώρους υγείας

---

## 🐛 Bug Reports & Feature Requests

Βρήκες bug ή έχεις ιδέα για νέο feature; 
👉 [Open an Issue](https://github.com/YOUR_USERNAME/mindcare/issues)

---

## 📝 License

Αυτό το έργο είναι licensed υπό την **MIT License** - δες το [LICENSE](LICENSE) αρχείο για λεπτομέρειες.

---

## 👨‍💻 Συγγραφέας

**Γεώργιος Συμεωνίδης** (@YOUR_GITHUB_USERNAME)

- 🎓 Computer Science Student
- 💻 Full-Stack Developer
- 🧠 Passionate about AI & Mental Health

---

## 📞 Επικοινωνία

- **Email**: giorgio.simeon@gmail.com
- **GitHub**: [@YOUR_USERNAME](https://github.com/YOUR_USERNAME)
- **LinkedIn**: [Your LinkedIn Profile]

---

## 🙏 Ευχαριστίες

Ειδικές ευχαριστίες σε:
- **Google** για το Gemini API
- **Firebase** για τα εργαλεία
- **Supabase** για το vector database
- Όλους τους contributors

---

## ⚖️ Disclaimer

> ⚠️ **ΣΗΜΑΝΤΙΚΟ**: MindCare είναι ένα εργαλείο υποστήριξης και **δεν αντικαθιστά** την επαγγελματική ψυχολογική φροντίδα. Σε περίπτωση κρίσης, επικοινώνησε με έναν επαγγελματία ψυχικής υγείας ή καλέσε τη γραμμή έκτακτης ανάγκης.

---

## 📈 Project Stats

![GitHub Stars](https://img.shields.io/github/stars/YOUR_USERNAME/mindcare?style=flat)
![GitHub Forks](https://img.shields.io/github/forks/YOUR_USERNAME/mindcare?style=flat)
![GitHub Issues](https://img.shields.io/github/issues/YOUR_USERNAME/mindcare?style=flat)

---

<div align="center">

**Made with ❤️ for mental health**

⭐ Αν σε αρέσει το project, δώσε ένα star! ⭐

</div>
