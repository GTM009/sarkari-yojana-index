# SarkariYojanaIndex v4

## Deploy → Vercel
1. vercel.com → New Project → drag this ZIP
2. No build settings → Deploy

## Deploy → Netlify  
1. netlify.com → Sites → drag this folder/ZIP
2. Live in ~30 seconds

## Admin Credentials
Username: admin | Password: sarkari@2025
(Not shown on login page — keep safe)

## Firebase Realtime Database (for live chat)
1. console.firebase.google.com → niha-994b8
2. Build → Realtime Database → Rules tab
3. Set rules to allow read/write:
   { "rules": { ".read": true, ".write": true } }
4. Publish rules — chat goes live immediately

## Chat Features
- 💬 User chat: floating PiP, click ✕ to close (auto-closes after 5s idle)
- Messages disappear after 8s (with countdown)
- 🛡️ Admin Monitor: full chat panel (bottom-left)
  - Admin can READ all messages (including expired, shown dimmed)
  - Admin can SEND messages
  - Admin can DELETE any message
  - Admin can edit their chat display name (✏️ button)
  - Minimize → header strip, tap header to expand again
  - 📊 Monitor button in dashboard to reopen if closed
  - New message badge on Monitor button when closed
