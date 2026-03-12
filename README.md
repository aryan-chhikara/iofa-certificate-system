# IFOA — Certificate Management System
### Assignment 2 | IFOA India AI/ML Development Intern

---

## Overview
A certificate generation and management system for IFOA India flight dispatcher training programs. Supports generating, previewing, and downloading printable A4 PDF certificates.

## Features
- 5 training types: DGCA, EASA, Recurrent, Human Factors, Dangerous Goods
- Search & filter records by name, company, or training type
- Add new trainee records
- Certificate preview modal
- Download as A4 landscape PDF (uses browser print)
- Signatures: Kenneth Kronborg (COO) & Vincent Incammicia (CEO/Instructor)
- Certificate number format: `{BADGE}-{00000}-{YEAR}`
- 12-month validity with auto-computed expiry date
- No API key required — fully offline

## Setup

### 1. Install dependencies
```bash
npm install
```

### 2. Run
```bash
npm start
# Opens at http://localhost:3000
```

### 3. Build for production
```bash
npm run build
```

## Deploy to Vercel
```bash
npm i -g vercel
vercel
```

## Deploy to Netlify
```bash
npm run build
# Drag & drop the build/ folder at app.netlify.com
```

## PDF Download Note
The Download PDF button opens a print-ready HTML page and triggers `window.print()`.
Make sure your browser **allows pop-ups** for the app's domain.
In the print dialog, set: **Layout → Landscape**, **Paper → A4**, **Margins → None**.
