# Social Quests — Prototype (Surprise Theme)

This repository contains a playable web prototype of **Social Quests** (up to 8 players).
It uses Firebase Firestore for realtime sync and anonymous authentication.

## How to use
1. Create a Firebase project (see below).
2. Update `index.html` by replacing the `npm install firebase` object with your Firebase config.
3. Deploy to Vercel (or Netlify) by connecting this GitLab repository.
4. Open the live link on your phone and create/join rooms.

## Firebase setup (quick)
- Create project at: https://console.firebase.google.com
- Add a Web app and copy the config object (apiKey, authDomain, projectId, etc.)
- Enable Firestore (create DB in test mode) and Authentication → Anonymous sign-in.
- Replace `FIREBASE_CONFIG_HERE` in `index.html` with your config.

## Notes
- Prototype uses simple prompt/confirm dialogs for approvals and accusations for cross-browser simplicity.
- To import 1,000 cards later, replace the `SAMPLE_DECK` array in `index.html` with your JSON or load from `/cards.json`.
