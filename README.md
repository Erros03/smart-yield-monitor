# Smart Yield Monitor

https://github.com/Erros03/sprout-savvy-connect.git check the code structure and add this src/routes/yield-monitoring.tsx — a dedicated page reusing the existing size/ripeness panel styling.
Add /yield-monitoring, /live-stream, /history to the NAV array in src/components/AppShell.tsx so they appear in the sidebar.
Add the Acceptance Rate and Average Diameter stat cards to src/routes/index.tsx (metrics already exposed as metrics.acceptanceRate and metrics.size.avgDiameter).
Add firebase.json with SPA rewrites ({"source": "**", "destination": "/index.html"}) plus .firebaserc pointing at blightdetect-4b3a6.
Run a typecheck/build — the old Realtime Database seed file (firebase-seed.json) is now obsolete and should be replaced with Firestore-shaped sample data.

This project was built with [Lovable](https://lovable.dev).

## Build with Lovable

Continue developing this project in the [Lovable editor](https://lovable.dev/projects/91d6a696-dab1-4b91-b24a-9cf56195680e).

- **Ship faster**: describe what you want to build and Lovable handles the code.
- **Stay in sync**: every change made in Lovable is committed straight to this repository.
- **Full ownership**: this code is yours. Push to `main` on GitHub and your changes sync back into Lovable, ready for your next prompt.

## Development

Prefer working locally? You need Node.js and npm — [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating).

```sh
git clone <this-repository-url>
cd <repository-name>
npm i
npm run dev
```
