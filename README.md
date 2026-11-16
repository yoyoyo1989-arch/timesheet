# Auditor timesheets

A single-page prototype for monthly auditor timesheets: staff log hours and transport claims, the manager approves, marks pending or rejects, and drafts an email to the staff member.

- Months: use the month picker at the top. Each month has its own timesheets; the deadline is the 25th of the following month.
- Manager view: a list with tabs (All, Pending, Approved, Rejected, Not submitted) and a detail panel for each timesheet with Approve, Mark pending and Reject.
- Jobs: **Manage jobs** adds, edits and deletes jobs. Edits update every timesheet using the job. On a timesheet, each row has a job picker to change its job.
- Team: **Manage team** adds, renames or removes people. Removing someone deletes their timesheets in every month.
- Edit: managers can open any timesheet and choose **Edit timesheet**. Approved or pending sheets are reopened as Not submitted.
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
