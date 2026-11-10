WELSEAT PARTNER PANEL — MOTION EDITION

Included:
- index.html and app.js
- firestore.rules

Firebase:
1. Confirm Email/Password sign-in provider is enabled.
2. Authentication > Settings > Authorized domains: add welseat.github.io.
3. Create Firestore database.
4. In Firestore Rules, publish firestore.rules from this package.
5. Ensure admins/{YOUR_FIREBASE_ADMIN_UID} exists with role = "admin".
6. Deploy index.html and app.js to the ROOT of the new GitHub Pages repository.

GitHub Pages:
- Repository Settings > Pages > Deploy from branch > main / root.
- Wait for deployment, then open the published URL.

Partner account:
- Mobile + password login uses a Firebase Auth email alias internally. It is NOT SMS OTP.
- Email is optional profile information.
- New registrations are Pending until admin updates partners/{uid}.approved=true and status="Approved".
- Lead submissions are disabled until approval.
- Admin panel must use matching Firestore schema/rules to manage partners and leads.

Important:
- Commission is set by admin after verifying a successful order. This panel does not automatically verify WooCommerce purchases or transfer money.
- Existing localStorage records are not automatically migrated.
- Bank account details are sensitive. Limit admin access and do not share screenshots publicly.
- Firebase free tier has quotas and may require billing if usage grows.
