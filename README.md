# DEBUGGING Symposium — Easy Local Version

A deadline-friendly local version with **zero external packages**. It uses only Node.js built-in modules, so there is no better-sqlite3, node-gyp, Visual Studio, React, Vite, or npm dependency installation problem.

## Run
1. Install Node.js 18+ (Node 22 recommended).
2. Open this folder in VS Code.
3. Open Terminal and run:

```powershell
node server.js
```

4. Open http://localhost:5000

## Admin
URL: http://localhost:5000/admin/login
Username: `admin`
Password: `admin123`

## Flow
Participant registers → waiting room → Admin starts Round 1 → 15 questions → submit → Admin selects participants → Admin starts Round 2 → selected participants receive 5 debugging questions → submit → rankings.

For simplicity, Round 1 uses seeded questions 1–15 and Round 2 uses 16–20 automatically. Admin can add/delete questions. Data is stored in `data.json`.

This is intended for a local college-event demo, not production security/deployment.
