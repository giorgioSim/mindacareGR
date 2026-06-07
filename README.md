# 🧠 MindCare - AI-Powered Mental Health Application

[![React](https://img.shields.io/badge/React-18.0-blue?logo=react)](https://react.dev/)
[![Firebase](https://img.shields.io/badge/Firebase-Cloud-orange?logo=firebase)](https://firebase.google.com/)
[![Supabase](https://img.shields.io/badge/Supabase-PostgreSQL-green?logo=supabase)](https://supabase.com/)
[![Gemini API](https://img.shields.io/badge/Gemini-API-red?logo=google)](https://ai.google.dev/)
[![License](https://img.shields.io/badge/License-MIT-yellow)](LICENSE)

> **MindCare** είναι μια σύγχρονη εφαρμογή ψυχικής υγείας που χρησιμοποιεί τεχνητή νοημοσύνη και τη τεχνική RAG (Retrieval-Augmented Generation) για να παρέχει προσωποποιημένη ψυχολογική υποστήριξη.

---

## 📋 Περιεχόμενα

- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Εγκατάσταση](#-εγκατάσταση)
- [Χρήση](#-χρήση)
- [Συμβολή](#-συμβολή)

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
- Αναζήτηση με vector similarity
- Κρυπτογραφημένη αποθήκευση

### 🧘‍♀️ Mindfulness Module
- Καθοδηγόμενες ασκήσεις χαλάρωσης
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

## 💻 Χρήση

### Πρώτη Χρήση
1. Εγγραφή με email και password
2. Δημιουργία προφίλ (όνομα, ηλικία, χώρα)
3. Συμπλήρωση "Doctor Quiz" (10 ερωτήσεις)
4. Επιλογή AI θεραπευτή
5. Ξεκίνησε τη συνομιλία!

---

## 🤝 Συμβολή

Το MindCare είναι open-source και υποδέχεται συμβολές! 

---

> ⚠️ **ΣΗΜΑΝΤΙΚΟ**: MindCare είναι ένα εργαλείο υποστήριξης και **δεν αντικαθιστά** την επαγγελματική ψυχολογική φροντίδα. Σε περίπτωση κρίσης, επικοινώνησε με έναν επαγγελματία ψυχικής υγείας ή καλέσε τη γραμμή έκτακτης ανάγκης.

---


<div align="center">

**Made with ❤️ for mental health**

⭐ Αν σ αρέσει το project, gimme a star! ⭐

</div>
