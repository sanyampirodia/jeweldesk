# JewelDesk v1.1 — Firebase-connected owner prototype

This version adds Firebase Email/Password owner sign-in and Firestore sync for orders, customers, manufacturers, stones and payments. It must be served over HTTPS or localhost, not opened as a file:// page.

## Firebase setup
- Email/Password provider enabled and owner user created.
- Firestore owner-only rule published.
- Add the hosting domain under Authentication > Settings > Authorized domains.
- Deploy to a static HTTPS host.

## Limitations and safety
- Owner-only prototype; employee and external manufacturer accounts/permissions are NOT implemented.
- Data sync uses Firestore documents appData/{orders,customers,makers,stones,payments}.
- Existing sample data is fictitious. If a cloud document is absent, demo/local data may still appear. Replace demo records before real use.
- No photo/document upload; Firebase Storage was not enabled.
- Do not enter real customer or financial data until rules, hosting domain, backup and access controls are reviewed and tested.
- Stay on Firebase Spark; do not add billing or upgrade.
