# Splitr

<img width="1896" height="812" alt="Splitr Dashboard" src="https://github.com/user-attachments/assets/cbef8263-8e0f-4125-85bf-4b0d12dfe6bc" />

## 🚀 Overview  

**Splitr** is a modern expense-sharing platform designed for roommates, couples, and groups who want to manage shared finances without awkward money conversations.  

From rent and groceries to trips and subscriptions, Splitr keeps track of who paid what, who owes whom, and automatically calculates balances — making settlements fast, transparent, and stress-free.  

Built with a clean UI and real-time architecture, Splitr focuses on simplicity, automation, and clarity.

---

## ✨ Features  

### 🔐 Authentication & User Management  
- Secure authentication with Clerk  
- Protected routes and user-specific data isolation  
- Personalized dashboard per user  

---

### 👥 Group Management  
- Create and manage multiple groups  
- Add and remove members  
- Track expenses separately per group  
- Clear balance overview per group  

---

### 💸 Expense Tracking  
- Add shared expenses with payer and participants  
- Split bills equally with automatic balance calculation  
- Real-time updates across users  
- Transparent breakdown of every transaction  

---

### 📊 Smart Dashboard  
- Overview of total expenses per group  
- See who owes you and whom you owe  
- Clean UI for quick financial clarity  
- Spending visualization for better money awareness  

---

### 🔔 Smart Reminders  
- Track pending balances  
- Automated reminders for unsettled payments  
- Reduce awkward follow-ups between friends  

---

### 🧠 AI-Powered Monthly Summaries  
- AI-generated monthly spending insights  
- Email summaries of group expenses  
- Highlights spending patterns and key breakdowns  
- Keeps everyone financially informed  

---

### ⚡ Real-Time Functionality  
- Instant balance recalculations  
- Live updates powered by backend sync  
- Consistent state across devices  

---

### 📱 Responsive Design  
- Optimized for desktop, tablet, and mobile  
- Smooth and intuitive user experience  
- Accessible and minimal interface  

---

## 🛠️ Tech Stack  

- **Next.js**  
- **React**  
- **JavaScript**  
- **Tailwind CSS**  
- **Shadcn/UI**  
- **Clerk (Authentication)**  
- **Convex (Backend & Real-time DB)**  
- **Inngest (Background Jobs & Emails)**
- **Google Gemini (AI Insights Generation)**  

---

## 🧩 Technical Challenges & Solutions  

### 1️⃣ Real-Time Balance Calculation  

**Challenge:**  
Ensuring accurate balance updates across multiple users when expenses are added or modified in real time.

**Solution:**  
Used Convex’s reactive database model to automatically trigger recalculations on expense mutations. Optimized queries to prevent unnecessary re-renders and maintain UI performance.

---

### 2️⃣ Data Isolation & Ownership Protection  

**Challenge:**  
Preventing users from accessing or modifying other groups' financial data.

**Solution:**  
Implemented strict user-based access checks at the backend level. Every expense, group, and balance query validates membership before returning data.

---

### 3️⃣ Automated Email Workflows  

**Challenge:**  
Generating monthly AI summaries without blocking the main app experience.

**Solution:**  
Used Inngest to schedule and process background jobs. AI summaries are generated asynchronously and sent via email without impacting real-time app performance.

---

## 🚀 Future Improvements  

- Unequal and percentage-based split support  
- Payment gateway integration (Stripe / UPI)  
- In-app settlement tracking  
- Export expense reports (PDF/CSV)  
- Advanced analytics with AI-driven budgeting suggestions  
- Mobile app version (React Native)  

## 💡 Why Splitr?  

Because shared expenses shouldn’t ruin friendships.  

Splitr brings **clarity, automation, and peace of mind** to group finances — so you can focus on living, not calculating.
