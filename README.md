# Time Tracker (single-file web app)

A tiny, self-hostable time-tracking app. Punch in/out, add breaks, see weekly totals, export CSV/PDF — all in one `index.html`. Data lives in Supabase (Postgres) with Row-Level Security, so each user only sees their own entries. No server needed; works on GitHub Pages.

**Demo:** https://herrweitz.github.io/time-tracker/


## Features
- Start/stop shifts & breaks
- Weekly total, CSV & PDF export
- Email/password auth (Supabase Auth)
- Optional admin view (see all users)
- Runs on any static hosting (e.g., GitHub Pages)

## Quick start (use this instance)
Open the demo → sign up → start tracking.

## Self-host
1. Create a Supabase project.
2. Enable **Auth → Providers → Email**.
3. Copy your **Project URL** and **Publishable/anon key**.
4. In `index.html`, set `SUPABASE_URL`, `SUPABASE_KEY`, and optional `ADMIN_UID`.
5. Run the provided SQL (tables + RLS policies) in the Supabase SQL Editor.
6. Deploy via GitHub Pages (**Settings → Pages**).

> Security: Only publishable/anon keys belong in the frontend. **Never** expose `service_role`.

## Tech
HTML + vanilla JS + Supabase (Postgres + Auth)

License: MIT


---

# Zeit-Tracker (Ein-Datei-Web-App)

Kleine, selbst hostbare Zeiterfassung. Dienst starten/stoppen, Pausen, Wochensumme, CSV/PDF — alles in einer `index.html`. Daten liegen in Supabase (Postgres) mit Row-Level Security, sodass jede*r nur die eigenen Einträge sieht. Kein Server nötig; läuft auf GitHub Pages.

**Demo:** https://herrweitz.github.io/time-tracker/

## Funktionen
- Dienste & Pausen starten/stoppen
- Wochensumme, CSV- & PDF-Export
- E-Mail/Passwort-Login (Supabase Auth)
- Optionales Admin-Dashboard (alle Nutzer)
- Läuft auf statischem Hosting (z. B. GitHub Pages)

## Schnellstart (diese Instanz)
Demo öffnen → registrieren → Zeiten erfassen.

## Selbst hosten
1. Supabase-Projekt anlegen.
2. **Auth → Providers → Email** aktivieren.
3. **Project URL** und **Publishable/anon Key** kopieren.
4. In `index.html` `SUPABASE_URL`, `SUPABASE_KEY` und optional `ADMIN_UID` setzen.
5. Das mitgelieferte SQL (Tabellen + RLS-Policies) im Supabase SQL-Editor ausführen.
6. Über GitHub Pages deployen (**Settings → Pages**).

> Sicherheit: Im Frontend nur publishable/anon Keys verwenden. **Nie** `service_role` veröffentlichen.

## Technik
HTML + Vanilla JS + Supabase (Postgres + Auth)

Lizenz: MIT

<p align="center">
  <a href="https://buymeacoffee.com/weitz">
    <img src="https://img.buymeacoffee.com/button-api/?text=Buy%20me%20a%20coffee&emoji=☕&slug=weitz&button_colour=FFDD00&font_colour=000000&font_family=Inter&outline_colour=000000&coffee_colour=ffffff" alt="Buy Me A Coffee">
  </a>
</p>

