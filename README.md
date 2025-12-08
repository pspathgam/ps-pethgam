# School Portal Prototype (Client-side)
This is a **demo prototype** of a school portal designed to run locally (no server required). It demonstrates:
- Student dashboard (results, submit home tasks, quiz, leaderboard)
- Teacher dashboard (assign tasks, view submissions)
- Face-capture attendance demo (captures photos using camera)
- Templates: Marksheet and MDM statement
- Scrolling news & notifications

## How to run
1. Download and unzip the package.
2. Open `index.html` in a modern browser (Chrome, Edge, Firefox).
3. For camera access open `attendance.html` and click "Start Camera".

## Production notes (how to make this real)
To make this a real cross-device multi-user system you will need:
1. A backend service (Firebase Realtime Database or Firestore is free tier friendly).
2. Authentication (Firebase Auth for email/password or phone OTP).
3. File storage (Firebase Storage) for task attachments and attendance photos.
4. Optional: a small server (Node.js) for advanced features and role management.

### Quick Firebase integration pointers
- Create a Firebase project, enable Firestore, Auth, and Storage.
- Replace localStorage usage in `assets/js/app.js` with API calls to Firestore.
- Secure rules to ensure teachers can only write tasks and students only submit for their class.

If you'd like, I can:
- Convert this prototype to use Firebase (generate the updated files).
- Customize marksheet and MDM templates you provide.
- Package everything into a ready zip — already done here as a demo.

