# Chris & Kristina – Save the Date

An interactive save the date for the wedding of Chris Nicolaou and Kristina Langer on Saturday 28 August 2027.

Live at https://chrisandkristina.au

## What it does

- Opens on a sealed envelope with petals drifting in the background.
- Tapping the envelope breaks the wax seal, folds the flap up to show the lining, and lifts a rolled scroll out. The scroll unrolls, the flowers bloom and the names write themselves in.
- Shows a live countdown to the wedding day.
- Plays music once the envelope is tapped, with a speaker button to mute it.
- Has an "Add to calendar" button. On Android it opens Google Calendar with the date filled in, on iPhone (Safari) it opens Apple Calendar's add screen, and on other devices it offers a choice of the two.
- Responds to touch: dragging a finger or moving the mouse leaves a trail of gold sparkles, nudges the petals and tilts the card. Tapping the flowers scatters petals.
- The envelope button under the scroll closes it again so it can be replayed.
- Scales to fit any phone, tablet or computer screen.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The whole page: layout, styling, animation, fonts and script in one file. |
| `music.mp3` | The track that plays when the envelope is opened. Optional: without it, the page plays a built-in piano piece. |
| `save-the-date.ics` | The calendar entry used for Apple Calendar and Outlook. Google Calendar uses a link inside `index.html` instead. |
| `preview.jpg` | The image shown when the link is shared in Messenger or a text. |
| `CNAME` | Created by GitHub Pages. Holds the custom domain, so don't delete it. |

File names are case sensitive and the page looks for them exactly as written above.

## Hosting

The site is hosted on GitHub Pages from the `main` branch, root folder, with the custom domain `chrisandkristina.au`.

DNS is managed at VentraIP:

- Four `A` records on the bare domain pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153` and `185.199.111.153`
- One `CNAME` record for `www` pointing to `sergen93.github.io`

## Making changes

- **Text, names or date:** edit `index.html`. If the date changes, also update the countdown target (search for `Date.UTC`), `save-the-date.ics` and the Google Calendar link (search for `calendar.google.com`).
- **Music:** replace `music.mp3` with another file of the same name. Keep it to a few megabytes so it loads quickly on mobile data.
- **Link preview image:** replace `preview.jpg` with another image of the same name, 1200 × 630 pixels.

After committing, GitHub Pages republishes the site within a minute or two. Phones may show the old version for a short while until their cache refreshes, and apps such as Messenger can keep an old link preview for links that were already shared.

## Notes

- The countdown runs to midnight at the start of 28 August 2027, Queensland time.
- Phone browsers only allow sound after a tap, so the music starts when the envelope is opened.
- The fonts, Pinyon Script and Cormorant Garamond, are built into `index.html`, so the page makes no requests to outside services. Both are under the SIL Open Font License.
- Guests who have "reduce motion" switched on in their phone settings get a still version with no petals or animation.
- Only use music the couple has the right to share publicly, since the file can be downloaded from this repository.
