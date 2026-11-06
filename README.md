# Family archive

An encrypted, password-protected family website for GitHub Pages.

Only the access screen and ciphertext are stored in this repository. The password
is shared separately by the family. AES-256-GCM authenticates the payload;
PBKDF2-SHA-256 derives the key with a fresh 32-byte salt and 600,000 iterations.
Decryption happens in the visitor's browser. No analytics or password service.
Refreshing the page or choosing “Закрыть доступ” locks it again.

Publish the repository root from the `main` branch using GitHub Pages.
Never commit the password, unencrypted HTML, original documents or spreadsheets.
The encrypted payload is a snapshot, not a live Google Sheets integration.
