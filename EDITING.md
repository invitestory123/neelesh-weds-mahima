# Editing Guide — Neelesh & Mahima Wedding Invitation

Customer customization guide for `neelesh-mahima` (royal Diggi Palace, Jaipur wedding celebration).

## Primary Customer Data

All text, dates, events, venue, gallery, RSVP, and assets live in:
- `editable/wedding-data.js`

### Configuration fields in `editable/wedding-data.js`:
- **Couple Details**:
  - `couple.groom`: Groom's name (`"Neelesh"`)
  - `couple.bride`: Bride's name (`"Mahima"`)
  - `couple.openingDate`: Date string on cover (`""` to omit, or `"12 · December · 2026"`)
  - `couple.heroDate`: Date badge in hero (`"12 · 12 · 2026"`)
- **Invitation (Grandparents & Parents)**:
  - `invitation.grandparents`: Grandparents' names (`"Shrimati Charan Kaur & Late Shree Nathi Lal"`)
  - `invitation.subtext`: Invitation line (`"Cordially invite you to celebrate the marriage of their grandson"`)
  - `invitation.groom`: Groom's name
  - `invitation.groomParents`: Groom's parents (`"S/o Dr. Pushpa Nagar & Dr. Rakesh Lal"`)
  - `invitation.bride`: Bride's name
  - `invitation.brideParents`: Bride's parents (`"D/o Shri Radheyshyam Chauhan & Smt. Radhika Chauhan"`)
- **Countdown**:
  - `countdown.targetISO`: Target ISO date string (`"2026-12-12T16:00:00+05:30"`)
- **Scratch-to-reveal Save the Date Card**:
  - `scratchCard.day`: Day of week (`"Saturday"`)
  - `scratchCard.date`: Day number (`"12"`)
  - `scratchCard.monthYear`: Month and year (`"December · 2026"`)
  - `scratchCard.city`: Location (`"Jaipur"`)
- **Story**:
  - `story.portraitCaption`: Two-line array caption below the portrait photo
  - `story.text`: Story description text
- **Events**:
  - `events[]`: Array of events with `name`, `date`, `time`, `place`, `mark`
- **Gallery**:
  - `gallery[]`: Array of couple/portrait images with `src`, `title`, `caption`
- **RSVP**:
  - `rsvp.pitaPaksh`: Groom's family & relatives
  - `rsvp.mataPaksh`: Groom's maternal side family & relatives
- **Venue**:
  - `venue.name`: Venue name (`"Diggi Palace"`)
  - `venue.addressLine1`: First line of address (`"Shivaji Marg, C Scheme"`)
  - `venue.addressLine2`: City/Postal code line (`"Jaipur, Rajasthan 302004"`)
  - `venue.cityTag`: Map badge subtitle (`"Touch to explore · Jaipur"`)
  - `venue.mapQuery`: Search query for Google Maps
  - `venue.mapUrl`: Direct link to Google Maps (`"https://maps.app.goo.gl/NXVZdNLmF9cyk8FT8?g_st=iw"`)
- **Assets**:
  - `assets.video`: Opening cinematic video path
  - `assets.flowFrame`: Poster frame image for video
  - `assets.heroArt`: Hero portrait image
  - `assets.storyPhoto`: Story portrait photo
  - `assets.ogImage`: Social share image
  - `assets.bgm`: Background music audio path (`bgm.mp3`)

## Testing

```bash
node --check editable/wedding-data.js
node --check assets/index-DLpsKpIv.js
```
Open `http://localhost:9015/` in browser.
