# AppADay 141: Court of Honor Citation

**Live app:** https://augustineiacopelli.github.io/appaday-141-court-of-honor-citation/

**Part of AppADay:** https://augustineiacopelli.github.io/appaday/

Court of Honor Citation builds a rank advancement certificate for a Cub Scout Pack or a Scout Troop. Enter the Scout, the rank earned, and an optional favorite moment, and Claude writes a short citation for the certificate. The tone grows with the rank, from warm and simple enough to read aloud to a Lion, to formal and dignified at Eagle, where the citation speaks to the leader and citizen the Scout is becoming. Print the certificate on one letter landscape page or save it as an image to share.

## How it works

Choose Pack or Troop at the top. The rank list, the event name (Advancement Ceremony or Court of Honor), and the signer titles (Cubmaster or Scoutmaster, plus Committee Chair) all switch to match. The unit number and signer names are remembered in your browser, so a leader setting up for a ceremony enters them once.

For each Scout, enter a name, pick the rank, confirm the ceremony date, and optionally add a highlight such as a campout or service project. Generate writes a citation of two or three sentences that uses only the facts you gave it. The citation lands in an editable box, and every change you make shows on the certificate preview immediately. Next Scout clears the name, highlight, and citation while keeping the rank and date, so a whole ceremony can be run through quickly.

Long names shrink to fit on a single line. Print produces one landscape page that matches the preview. Save image draws the certificate at 2200 by 1700 pixels and opens the share sheet on phones or downloads the file on desktop.

## Design

The certificate uses a red, white, and blue palette in Old Glory blue and Old Glory red on a cream field, with a navy border, a red inset rule, a row of stars beneath the unit line, and a navy seal between the signature lines. Names and titles are set in Cinzel and the citation in EB Garamond italic.

## Claude and your API key

Citations are written by Claude (`claude-sonnet-5`) called directly from your browser. Add your own Anthropic API key in Settings (the gear icon). The key is stored only in this browser's local storage and is never sent anywhere except the Anthropic API. Without a key, the app fills in a built in template citation matched to the rank, so it still works offline from the AI.

## Technical notes

A single self-contained `index.html` of vanilla HTML, CSS, and JavaScript with no build step. Google Fonts is the only external request. The certificate is sized entirely in container query units, so the screen preview, the printed page, and the exported image share one set of proportions.

---

*Ship something every day. It compounds.*
