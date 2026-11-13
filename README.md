# Alishba's Birthday Countdown

A single-page site for GitHub Pages with:

- A live countdown to **12 December 2026, 12:00 AM PKT**
- One original quote per day (English and Roman Urdu), from 13 November to 12 December
- Daily browser notifications with the day's quote, changing at **12:00 AM PKT**

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole page: countdown, quotes, notifications |
| `sw.js` | Service worker, needed so notifications work on phones |

## Publish on GitHub Pages

1. Push these files to the repository `AunSyedShah/alishba_birthday`.
2. On GitHub, open **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to *Deploy from a branch*, choose branch `main` and folder `/ (root)`, then click **Save**.
4. After a minute the site is live at `https://aunsyedshah.github.io/alishba_birthday/`.

## Turning on notifications

1. Open the site and click **Turn on daily notifications**.
2. Allow notifications when the browser asks.
3. On iPhone: open the site in Safari, tap **Share → Add to Home Screen**, then open it from the home screen and turn on notifications there. iOS only allows notifications for home-screen web apps.

## Important limitation

GitHub Pages is a static host. It cannot send messages on its own. Notifications arrive only while the browser or the installed app is running. If the phone or computer is off, or the browser is closed at 12:00 AM PKT, the quote is sent the next time the site runs. The quote for each day is sent only once.

## Changing quotes or dates

Quotes live in the `QUOTES` list in `index.html`. Quote 1 is for 13 November 2026 and quote 30 is for the birthday. The dates are set by `START` and `BIRTHDAY` in the same file.
