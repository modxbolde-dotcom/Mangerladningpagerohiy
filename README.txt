PIXEL FIREBASE LANDING + MANAGER (mobile-first)

Firebase setup:
1. Open firebase-config.js.
2. Replace https://YOUR-DATABASE-URL with your exact Realtime Database URL from Firebase Console.
3. Both pages use the same database path: /landingPage.
4. Host both pages over HTTPS. ES modules may not work when opening index.html directly from file storage.
5. Open manager page, edit settings and press Save changes. The public landing page listens for live updates.

The app config contains only databaseURL, as requested. This relies on your Realtime Database being accessible with the current rules.
WARNING: public read/write rules (true/true) let anyone read, overwrite or delete database data. Do not use them for sensitive or production data.
The Auto-approve switch only saves a setting; it does not itself approve Telegram join requests.
