KIREHE HEALTH CENTERS DATA MANAGEMENT SYSTEM

FILES
- Code.gs
- Index.html
- Admin.html

INSTALL
1. Open the Google Apps Script project attached to your spreadsheet.
2. Replace/add Code.gs, Index.html and Admin.html using these files.
3. Save the project.
4. Run setupSystem() once from the Apps Script editor and approve permissions.
5. Run createFirstAdminNow() once only if no active Admin account exists.
6. Deploy > New deployment > Web app.
   Execute as: Me
   Who has access: choose the most restrictive option that fits your organization.
7. Open the deployed /exec URL for the main app.
   Admin console: same URL with ?page=admin (example: .../exec?page=admin)

INITIAL ADMIN (only if createFirstAdminNow() succeeds)
Username: admin
Password: KireheAdmin2026#
Change this password immediately after first login and do not share it.

IMPORTANT
- Do not use real patient-identifying data until your organization has reviewed access controls and data-protection requirements.
- The system stores facility-level health summaries; avoid entering patient names, IDs, or sensitive personal details in free-text descriptions.
- Apps Script HTML pages must be opened through the deployed Apps Script Web App URL; google.script.run will not work if the HTML files are opened directly from a local folder or served by Vercel.
- Admin page access is enforced in backend functions, not just hidden in the interface.
