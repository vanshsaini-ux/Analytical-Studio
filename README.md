# Medharthi CRM Analytics

Static web app (no backend, no build). Upload a LeadSquared CRM export (.csv / .xlsx) and get
Overview, Trends (WoW / MoM / QoQ), Breakdown and an Explorer for manual analysis.
Files are processed in the browser only and are never uploaded.

## Files
- `index.html`: the whole app
- `vercel.json`: hosting config (clean URLs, no-index header)

## Deploy
1. Push this repo to GitHub (keep it private).
2. Vercel: Add New > Project > import this repo.
3. Framework Preset: Other. Build Command and Output Directory: leave empty. Deploy.
4. Project Settings > Deployment Protection: enable Vercel Authentication to restrict access.

## Update
Edit `index.html` and commit. Vercel redeploys automatically.

## Notes
- SheetJS and Chart.js load from cdnjs, so internet access is required.
- Dates are auto-detected as MM/DD/YYYY (LeadSquared) or DD/MM/YYYY.
