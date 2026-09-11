# Pest Seal website

## Run locally
npm install
npm run dev

## Deploy
Push this folder to a GitHub repo, then import it at vercel.com or netlify.com
(Import Project -> GitHub). Both auto-detect Vite and build automatically.

## Connect bookings to your Google Calendar (Cal.com)
1. Create a free account at cal.com and connect your Google Calendar under
   Settings -> Apps -> Google Calendar.
2. Create two event types:
   - "Free Inspection & Quote" (e.g. slug: free-inspection)
   - "Seal Service" (e.g. slug: seal-service)
3. Open src/App.jsx and near the top, set:
   - CAL_USERNAME to your cal.com username
   - CAL_EVENT_SLUGS.inspection / .seal to your two event slugs
4. Redeploy. Every booking made on the site will now appear on your Google
   Calendar automatically -- Cal.com also emails the customer a confirmation
   and calendar invite.
