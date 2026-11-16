# Auditor timesheets

A single-page prototype for monthly auditor timesheets: staff log hours and transport claims, the manager approves, marks pending or rejects, and drafts an email to the staff member.

- Static site: one `index.html`, no build step, no dependencies.
- Data is stored in the visitor's browser (`localStorage`). There is no login or backend yet.
- Fonts load from Google Fonts; the page falls back to system fonts if offline.

## Deploy to Vercel

1. Push this folder to a GitHub repository (files at the repo root).
2. In Vercel, choose **Add New → Project** and import the repository.
3. Framework preset: **Other**. Leave Build Command and Output Directory empty.
4. Click **Deploy**.

Or from the command line: `npx vercel --prod` in this folder.

## Run locally

Open `index.html` in a browser, or run `npx serve .`.

## Next steps

- Real login and shared storage, so staff and manager see the same data.
- Server-side email sending (the prototype only opens a mail draft).
