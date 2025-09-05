🎥 LiveLink (Video Conferencing App)
📌 Overview
LiveLink application is built with Next.js, TypeScript, Tailwind CSS, Clerk, and Stream API. It enables users to securely log in, create meetings, and utilize key video-conferencing features such as recording, screen sharing, and participant management.

The application is responsive, secure, and designed to replicate the core functionalities of professional video conferencing platforms.

⚙️ Tech Stack
Next.js 14 (App Router)

TypeScript

Tailwind CSS (with shadcn UI)

Clerk (Authentication)

Stream (Video Conferencing)

🔋 Features
✅ Authentication – User login/signup with Clerk (email/password or social providers).
✅ Start New Meetings – Configure video/audio before joining.
✅ Meeting Controls – Record, mute/unmute, screen share, emoji reactions, participant list, and role-based permissions.
✅ Exit / End Meeting – Leave a meeting or end it for everyone.
✅ Schedule Meetings – Create and manage future meetings.
✅ Upcoming Meetings Page – Quick access to scheduled meetings.
✅ Past Meetings & Recordings – Review meeting history and recordings.
✅ Personal Room – Shareable personal link for quick meetings.
✅ Join by Link – Join meetings easily with distributed links.
✅ Responsive Design – Works seamlessly across desktop, tablet, and mobile.

🤸 Quick Start
Follow these steps to run the project locally:

1. Prerequisites
Make sure you have installed:

Git

Node.js

npm

2. Clone the Repository
bash
git clone https://github.com/ShivamChoughule1/LiveLink.git
cd zoom-clone
3. Install Dependencies
bash
npm install
4. Set Up Environment Variables
Create a .env file in the project root with:

text
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=

NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up

NEXT_PUBLIC_STREAM_API_KEY=
STREAM_SECRET_KEY=
👉 Replace the values with your Clerk and Stream credentials.

5. Run the Project
bash
npm run dev
Open http://localhost:3000 🚀

🕸️ Code Snippets
🎨 Global Styles – app/globals.css
css
@tailwind base;
@tailwind components;
@tailwind utilities;

/* Stream UI overrides */
.str-video__participant-list {
  background-color: #1c1f2e;
  border-radius: 10px;
  padding: 10px;
  color: white;
}

.glassmorphism {
  background: rgba(255, 255, 255, 0.25);
  backdrop-filter: blur(4px);
}
🎨 Tailwind Config – tailwind.config.ts
ts
extend: {
  colors: {
    dark: {
      1: "#1C1F2E",
      2: "#161925",
      3: "#252A41",
    },
    blue: {
      1: "#0E78F9",
    },
  },
  backgroundImage: {
    hero: "url('/images/hero-background.png')",
  },
}
📂 Assets
All UI assets and icons are available in the public/ directory.
You can also access them from this folder.

🚀 Future Improvements
🔹 Add recording storage via a cloud service
🔹 Implement chat & breakout rooms
🔹 Expand theme customization (dark/light mode)
🔹 Integrate AI-based noise suppression