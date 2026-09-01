# Knight Rider Operations — Dispatch Demo

Internal operations demo for Knight Rider Transportation. Static site (no build step) backed by a live Supabase project.

## Structure
- `index.html` — the entire app (login, dashboard hub, trip dispatch module, driver module)
- `logo.png` — company logo, background removed, referenced by index.html

## Deploy
This is a static site — no build command needed. On Vercel: Framework Preset = "Other", no build/output settings required, just deploy the root.

## Demo logins
All passwords: `demo1234`
- admin@knightriderbus.com (admin / dispatch view)
- devon@knightriderbus.com (driver view)
- kester@knightriderbus.com (driver view)
- anand@knightriderbus.com (driver view)

## Notes
- Backend is a live Supabase project (see SUPABASE_URL / SUPABASE_KEY in index.html).
- Auth is demo-grade (plaintext password match against an open `staff` table) — not production security.
- Row Level Security is enabled on all tables but policies are fully open (`using (true)`) for demo purposes.
