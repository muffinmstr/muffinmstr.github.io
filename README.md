# Trade Board

A small website for trading items in a video game. Everyone lists the items they're willing to trade, finds who has what they want, and sends a trade request. The other player answers **Yes** or **No**, and a request nobody answers is automatically declined after **5 minutes**.

The page lives on GitHub Pages and keeps its data in a free Supabase project. There's no server for you to run.

---

## How to use it

### 1. Set up your profile (My stash tab)
- **Display name** and **Preferred meeting code**: other players see these in search.
- **I'm available to trade right now**: turn this on to appear in other people's searches, and off when you're busy. Flipping it saves right away.
- Tap **Save profile**.

### 2. List what you'll trade
Pick a value from each of the four dropdowns, set a quantity, and tap **Add**. Use **Remove** to take an item off.

### 3. Find a trade (Find tab)
Choose from the four dropdowns. "Any" means no filter on that one. Players who are online right now show a green **online** marker and are listed first.

### 4. Request a trade
Set a quantity and tap **Request trade**. The other player gets a notification, and it auto-declines after 5 minutes so you can ignore it if you are busy.

### 5. Answer a request (Requests tab)
Tap **Yes** or **No**. Once accepted, both sides see the meeting code. Finished requests have a **Clear** button, or use **Clear all finished** at the top. Clearing only hides them on your own device.

---

## Which devices and browsers work

| Device | Browser | Status |
|---|---|---|
| Windows | Any modern browser | Works fully, including sound and alerts |
| Android | Meta browser | Works |
| Android | Other browsers (Chrome, Firefox, etc.) | Not tested yet |
| iPhone / iPad | **Safari** | Works. Add it to your Home Screen for alerts (steps below) |
| iPhone / iPad | **DuckDuckGo** | Works |
| iPhone / iPad | Google (Chrome), Bing, Firefox | **Doesn't work properly.** Use Safari or DuckDuckGo instead |

Based on our own testing, not an official compatibility list.

### Windows
Open the site and use it. Click anywhere on the page once so the browser allows sound, then go to **My stash → Alerts** to press **Enable browser alerts** and **Test sound**.

### Android
The Meta browser is the one we've tested and it works. Other Android browsers haven't been tested yet, so they may or may not work. If you try one, check that sound and alerts work with **Test sound** and **Enable browser alerts** in the Alerts section of the My stash tab.

Open the site and use it. Tap the page once to allow sound. Browser alerts and sound only work while the page is open on your screen, so keep it open and the screen on while you're waiting for trades.

### iPhone / iPad (Safari or DuckDuckGo)
1. Open the site in **Safari** or **DuckDuckGo**. Chrome, Bing and Firefox on iPhone didn't work in our testing (see below).
2. Tap the **Share** button, then **Add to Home Screen** (you may need to tap **View More** first to see it), then **Add**.
3. Open the app from its **Home Screen icon**, not from the browser.
4. Go to **My stash → Alerts** and tap **Enable browser alerts**, then allow notifications.
5. Tap the page once to allow sound and press **Test sound**. If you hear nothing, check that the side switch isn't on silent and the volume is up.

Browser alerts need iOS 16.4 or newer.

### Why it doesn't work in Google, Bing, or Firefox on iPhone
Every iPhone browser uses Apple's own browser engine, but each app decides which features it supports, such as installing a site to the Home Screen, notifications and sound. In our testing, Chrome (Google), Bing and Firefox on iPhone didn't give a working Home Screen app icon, browser alerts or reliable sound, while Safari and DuckDuckGo did. We don't know exactly why, and it could change when those apps update. If yours doesn't work, switch to Safari or DuckDuckGo.

---

## Things to know
- **Alerts only work while the page or app is open.** A closed app, or a locked phone, can't get a request. Real background notifications would need push notifications, which this version doesn't have.
- **Your identity is saved in your browser.** Clearing your browser data creates a new anonymous player, and your old listing stops showing in search after about 14 days.
- **Trades aren't tracked in the game.** The site only connects players and arranges the meeting. After an accepted trade, update your own item quantities.
- **Free Supabase projects pause after about a week without use.** If the page shows a database error, open the Supabase dashboard and resume the project.
- If the page looks outdated after an update, close it and reopen it, or refresh the page twice.
