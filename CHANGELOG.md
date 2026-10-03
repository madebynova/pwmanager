# Changelog

All notable changes to the Password Manager are listed here.

---

## [Unreleased]

_(none)_

---

## 2026-02-16 22:00

- **UI:** Changelog is now inside the app: open the vault, scroll to the bottom of the sidebar, and click “Changelog” to expand or collapse it.
- **UI:** Same eye icon (open when visible, closed when hidden) on the master password fields: Setup screen (master + confirm) and Unlock screen.
- **Feature:** “Remember me on this device” on Setup and Unlock. When checked, your master password is stored locally so the app can unlock automatically until you click “Forget me” in Settings or clear browser data / reset PC. Use “Forget me (lock and clear remembered password)” in Settings to lock and stop auto-unlock.

---

## 2026-02-16 21:45

- **UI:** Show/Hide password is now an eye icon: closed eye when the password is hidden, open eye when visible. Applies to the Add entry form and to each entry row in the list.
- **Feature:** Categories are now custom. Type any category name when adding an entry; existing categories from your entries appear as suggestions (datalist and filter dropdown). The category filter is populated from your saved entries.

---

## 2026-02-16 21:26

- **Add:** Show / Hide toggle for the password field in the Add entry form. You can reveal or mask the password you type or paste before saving.
- **Add:** This changelog (CHANGELOG.md) with dates and times for updates.

---

## 2026-02-16 20:15

- **Layout:** App now fills the full screen (1920×1080). Viewport set to 100vw × 100vh with no overflow.
- **Layout:** Vault uses a two-column layout: fixed sidebar (form, generator, settings) and main area (search + entry list) that uses the rest of the width.
- **UI:** Dark theme tweaks (darker background, indigo accent, clearer borders).
- **UI:** Cleaner typography and spacing; focus states on inputs; hover states on entry rows.
- **UI:** Setup and Unlock screens centered in the viewport with short subtitles.
- **Responsive:** Below 900px width, layout stacks (sidebar on top, then entry list).

---

## 2026-02-16 18:00

- **Initial release:** Single-file password manager (index.html).
- **Security:** AES-GCM encryption, PBKDF2 key derivation (250,000 iterations), vault in localStorage. Master password never stored.
- **Features:** Master password setup and unlock, add/edit entries (site, username, password, category, notes), search and category filter, password generator (length 12–32, options, strength indicator), show/hide and copy password per entry, clear vault, export/import encrypted backup.
- **Lock:** Auto-lock on page reload and after 5 minutes of inactivity.
