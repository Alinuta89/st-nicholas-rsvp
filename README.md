# St. Nicholas Party RSVP

No-sign-in RSVP page for the St. Nicholas Party (Sat Dec 5, 4:00 PM).

- **Guests open:** https://alinuta89.github.io/st-nicholas-rsvp/
- **Where the answers live:** every RSVP is a row on the **RSVPs** tab of the "St. Nicholas Party RSVP" Google Sheet, and **Start here** keeps the tally. Everyone sees the running list ("Who's coming") on the page itself.
- **Backend:** a small Google Apps Script web app in that Sheet. It saves the rows and emails each family their personal edit link. Its code (`Code.gs`) is kept out of this repo on purpose.

## Day to day

- Change your RSVP: use the personal link from your email, or "Lost your link?" at the bottom of the page.
- Reminders: in the Sheet, open **Extensions → Apps Script**, pick `sendReminders`, press **Run**.
- After any change to `Code.gs`: **Deploy → Manage deployments → Edit → Version: New version → Deploy**. The page keeps the same backend address.

## Privacy

Anyone with the link can see family names, kids' ages and boy/girl, and dishes. Emails and edit codes stay in the Sheet. `noindex` keeps search engines from listing the page. The street address loads from the backend, so it isn't written in this public repo.
