# K-Fanon Marketplace

A minimal, browser-based marketplace for fictional K-pop releases.

## Current features
- Email/password accounts through Firebase Authentication.
- Usernames, display names and preset profile icons.
- Browser-persistent login sessions.
- Create, edit, publish and delete albums, EPs, singles and mixtapes.
- Add track titles and original-artist credits.
- Discover published releases and view their tracklists.
- Private drafts and a personal release library.
- Responsive layout for desktop and mobile.

## Firebase setup
1. In Firebase Authentication, enable **Email/Password**.
2. Create a Firestore database (the project is configured to use the default database).
3. In Firestore, open **Rules**, replace the contents with `firestore.rules`, and publish.
4. Serve the repository with GitHub Pages (Settings → Pages → Deploy from a branch → `main` / `/(root)`).

The Firebase web configuration is in `index.html`. It is intended for client-side use; access control is enforced by Firestore Security Rules.

## Notes
- Profile images currently use preset icons. No Firebase Storage or paid services are used.
- Cover art is linked using an image URL; uploads are not enabled.
- Spotify linking is not included in this first foundation build.
- No Cloud Functions are required.
