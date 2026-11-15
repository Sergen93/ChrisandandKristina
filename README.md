# Chris & Kristina – Save the Date

An interactive save the date for the wedding of Chris Nicolaou and Kristina Langer on Saturday 28 August 2027.

Live at https://chrisandkristina.au

## What it does

- Opens on a sealed envelope. Tapping it lifts the wax seal, folds the flap up and unrolls a scroll with the details.
- Shows a live countdown to the wedding day.
- Plays music once the envelope is tapped, with a speaker button to mute it.
- Has an "Add to calendar" button that adds the date to the guest's calendar.
- Scales to fit any phone, tablet or computer screen.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The whole page: layout, styling, animation and script in one file. |
| `music.mp3` | The track that plays when the envelope is opened. Optional: without it, the page plays a built-in piano piece. |
| `save-the-date.ics` | The calendar entry behind the "Add to calendar" button. |
| `preview.jpg` | The image shown when the link is shared in Messenger or a text. |
| `CNAME` | Created by GitHub Pages. Holds the custom domain, so don't delete it. |

File names are case sensitive and the page looks for them exactly as written above.

## Hosting

The site is hosted on GitHub Pages from the `main` branch, root folder, with the custom domain `chrisandkristina.au`.

DNS is managed at VentraIP:

- Four `A` records on the bare domain pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153` and `185.199.111.153`
- One `CNAME` record for `www` pointing to `sergen93.github.io`

## Making changes

- **Text, names or date:** edit `index.html`. If the date changes, also update the countdown target (search for `Date.UTC`) and `save-the-date.ics`.
- **Music:** replace `music.mp3` with another file of the same name. Keep it to a few megabytes so it loads quickly on mobile data.
- **Link preview image:** replace `preview.jpg` with another image of the same name, ideally 1200 × 630 pixels.

After committing, GitHub Pages republishes the site within a minute or two. Phones may show the old version for a short while until their cache refreshes.

## Notes

- The countdown runs to midnight at the start of 28 August 2027, Queensland time.
- Phone browsers only allow sound after a tap, so the music starts when the envelope is opened and won't play if the phone is on silent.
- Fonts are Pinyon Script and Cormorant Garamond, loaded from Google Fonts.
- Only use music the couple has the right to share publicly, since the file can be downloaded from this repository.
