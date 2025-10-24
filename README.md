# ThreatSim

**ThreatSim** is a **React + TypeScript web application** designed as an interactive cybersecurity learning platform. It provides a safe environment to practice cybersecurity challenges while tracking progress and achievements.

## 🌐 Live Demo
[https://threatsim-app.vercel.app/](https://threatsim-app.vercel.app/)

## 🚀 Features

- **Authentication System**  
  - Email/password login  
  - Google OAuth login  
  - Persistent user sessions  

- **Data Persistence & Progress Tracking**  
  - Challenge progress automatically saved in localStorage  
  - Tracks user statistics, achievements, and completed challenges  
  - Visual progress indicators  

- **Challenge Categories**  
  - Web Exploitation  
  - Reverse Engineering  
  - Steganography  

## 🏗️ Technical Details

- **Frontend:** React 18 + TypeScript  
- **Styling:** Tailwind CSS  
- **State Management:** React Context API  
- **Routing:** React Router  
- **Data Storage:** LocalStorage  

## ⚡ Setup Instructions

1. Clone the repository:  
   ```bash
   git clone <repo-url>
   cd ThreatSim
   npm install
   ```

2. Configure Google OAuth credentials in `.env`:

   ```env
   VITE_GOOGLE_CLIENT_ID=your_google_client_id_here
   VITE_APP_NAME=ThreatSim
   VITE_APP_VERSION=1.0.0
   ```

3. Run the development server:

   ```bash
   npm run dev
   ```

4. Open your browser at `http://localhost:5173`

## 💾 Data Storage

- `threatSim_user` — Authentication data  
- `threatSim_challenge_{challengeId}_{userId}` — Individual challenge progress  
- `threatSim_progress_{userId}` — Overall progress and statistics  

## 📂 Project Structure

```
src/
├── components/         # React components for challenges and UI
├── contexts/           # AuthContext for state management
├── pages/              # Pages like Login, Journey, SimulationLab
├── utils/              # Data persistence utilities
└── main.tsx            # App entry point
```

---

**ThreatSim** is ready to use for learning and practicing cybersecurity challenges. 🔐
