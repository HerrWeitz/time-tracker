# Time Tracker (single-file web app)

A tiny, self-hostable time-tracking app. Punch in/out, add breaks, see weekly totals, export CSV/PDF — all in one `index.html`. Data is stored in Supabase (Postgres) with Row-Level Security, so each user only sees their own entries. No server needed; works on GitHub Pages.

**Demo:** https://HerrWeitz.github.io/time-tracker/  

## Features
- Start/stop shifts + pauses (breaks)
- Weekly sum, CSV + PDF export
- Email/password auth (Supabase Auth)
- Optional admin view (see all users)
- Runs anywhere static hosting is available

## Quick start (use this instance)
Open the demo link → sign up → start tracking.

## Self-host
1. Create a Supabase project.
2. Enable **Auth → Providers → Email**.
3. Copy your **Project URL** and **Publishable (or anon) key**.
4. Edit `index.html`: set `SUPABASE_URL`, `SUPABASE_KEY`, and optional `ADMIN_UID`.
5. Run the provided SQL (tables + RLS policies) in Supabase SQL Editor.
6. Deploy with GitHub Pages (Settings → Pages).

> Security note: Only publishable/anon keys belong in the frontend. **Never** commit `service_role`.

## Tech
HTML + vanilla JS + Supabase (Postgres + Auth).

License: MIT
