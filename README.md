# Zalmi Hostel Management System

A complete hostel management web app built with Next.js and Tailwind CSS.

## Features

- **Dashboard** — Live overview of students, occupancy, rent collected/pending, and profit
- **Rooms** — 10 rooms (A1–A4, B1–B4, C1, C2) with correct seat counts, visual seat map
- **Students** — Add/edit/remove students, track rent paid and remaining, filter by payment status
- **Expenses** — Track IESCO (electricity), WASA (water), PTCL (WiFi), laundry, cleaning, maintenance, warden salary
- **Finance** — Full profit & loss: total rent income minus all expenses = net profit

## Room Layout

| Room | Seats | Block |
|------|-------|-------|
| A1   | 3     | A     |
| A2   | 4     | A     |
| A3   | 3     | A     |
| A4   | 4     | A     |
| B1   | 3     | B     |
| B2   | 4     | B     |
| B3   | 3     | B     |
| B4   | 4     | B     |
| C1   | 5     | C     |
| C2   | 4     | C     |

**Total: 36 seats**

## Getting Started (Local)

```bash
# Install dependencies
npm install

# Run development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000)

## Deploy to Vercel (Free)

### Step 1 — Push to GitHub
1. Create a new repository on [github.com](https://github.com) named `zalmi-hostel`
2. Open terminal in this folder and run:
```bash
git init
git add .
git commit -m "Initial commit — Zalmi Hostel Management"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/zalmi-hostel.git
git push -u origin main
```

### Step 2 — Deploy on Vercel
1. Go to [vercel.com](https://vercel.com) and sign in with GitHub
2. Click **"Add New Project"**
3. Select your `zalmi-hostel` repository
4. Click **"Deploy"** — Vercel auto-detects Next.js, no config needed
5. Your site is live in ~60 seconds at `https://zalmi-hostel.vercel.app`

## Data Storage

Data is stored in the browser's **localStorage**. It persists between sessions on the same device/browser. For multi-device access, you would need a database (e.g. Supabase — free tier available).

## Tech Stack

- **Next.js 14** — React framework
- **Tailwind CSS** — Styling
- **Lucide React** — Icons
- **localStorage** — Data persistence
