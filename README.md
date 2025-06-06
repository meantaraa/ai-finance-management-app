# 💰 AI Finance Manager

An intelligent, full-stack personal finance manager built with **Next.js**, **React**, **Shadcn UI**, **Prisma**, and **Gemini AI**. Designed to help users **track income/expenses**, **scan receipts with AI**, **manage recurring transactions**, and **generate monthly financial insights**.

---

## 🚀 Features

### 📸 AI Receipt Scanner
- Upload receipt images and auto-extract:
  - Merchant name
  - Amount
  - Date
  - Category
- Pre-fills transaction forms using Gemini AI

### 🧠 Gemini AI Integration
- Powered by **Gemini Pro (Google)**:
  - OCR and parsing of receipts
  - Monthly summaries and financial reports
- Customizable via user API keys

### 🔄 Recurring Transactions
- Create transactions that recur on set intervals
- Automatically executed on due dates
- Throttled to **10 transactions/user/min** for stability

### 🧾 Transaction Management
- Create, update, and delete transactions
- Supports both **income** and **expense** types
- Real-time updates of account balances
- Edit mode dynamically updates forms

### 📊 Dashboard & Visuals
- Display of **5 most recent transactions** per account
- Interactive **pie chart** for monthly expense categories using **Recharts**
- Color-coded category insights

### 📬 Monthly Reports
- Auto-generated on the **1st of each month**
- AI-generated email reports include:
  - Total income
  - Total expenses
  - Net change
  - Expense breakdown by category
- Styled HTML templates sent via email

### 🔒 Bot Protection & Security
- Middleware with **Shield** integration
- Allowlist trusted bots like `Googlebot`
- Protects public and API routes from abuse

### ☁️ Deployment with Vercel
- Fully configured for **Vercel deployment**
- Secure `.env` management and production protection enabled

---

## 🛠️ Tech Stack

| Tool              | Purpose                            |
|-------------------|------------------------------------|
| **Next.js**       | React framework for full-stack app |
| **Shadcn UI**     | Accessible UI components           |
| **Prisma**        | ORM for database operations        |
| **PostgreSQL**    | Primary database                   |
| **Gemini Pro API**| AI-powered receipt parsing         |
| **Recharts**      | Chart visualizations               |
| **Clerk**         | Authentication                     |
| **Resend**        | Email delivery                     |
| **Arcjet**        | Bot protection + middleware        |
| **Vercel**        | Hosting & deployment               |

---

## 🧪 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/meantaraa/ai-finance-management-app.git
cd ai-finance-management-app
```

### 2. Install dependencies
```bash
npm install
```

### 3. Create your `.env` file
```bash
cp .env.example .env
```

---

## ⚙️ Environment Variables

Update the `.env` file with your values:

```env
DATABASE_URL=
DIRECT_URL=

NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/onboarding
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/onboarding

GEMINI_API_KEY=
RESEND_API_KEY=
ARCJET_KEY=
```

---

### 4. Run the app locally
```bash
npm run dev
```

---

## 🌐 Live Demo

🔗 [mynli-ai-finance-manager.vercel.app](https://mynli-ai-finance-manager.vercel.app)

---

## 🧠 Credits

Built with ❤️ by **Antara Chanda**

---

## 📜 License

This project is licensed under the **MIT License**.
