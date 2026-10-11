# P2P Trade Board

A static trading page. No backend: players' browsers connect directly to each other (WebRTC via [Trystero](https://github.com/dmotz/trystero), which uses public WebTorrent trackers just to introduce peers).

## Deploy
1. Put `index.html`, `config.json` and this README in a GitHub repo.
2. Settings → Pages → deploy from the `main` branch (root).
3. Share the Pages URL.

## Configure (`config.json`)
- `appId`: change to something unique so you only meet your own community.
- `room`: players in the same appId + room see each other.
- `dropdowns`: the 4 dropdowns (label + options). Every stash item is one choice from each dropdown; searching uses the same dropdowns, where "Any" skips a filter. Keep the count the same for everyone in a room, and use the same options so listings line up.

## Limits
- You only see players who are online with the page open. Nobody online = empty board.
- Requests and the 5-minute auto-decline run in the browsers. Alerts only fire while the tab is open.
- Your profile and stash are saved in your own browser (localStorage) and are re-shared when you connect.
- There are no accounts, so anyone can use any name. Check the person at the meeting code.
- Some strict networks block WebRTC; those players may not connect.
