# Countdown to 30 November

A one-page countdown to the last day at Malteser International: Monday 30 November 2026, 17:00 Cologne time (21:30 in Colombo). After that it switches to counting the days full time on Southern Innovation Hub and Serendib Impact.

The sun, with a Maltese cross in it, rises over the horizon as November runs down. Weekdays left are counted on Cologne time.

## Change the date or time

Edit `CONFIG` at the top of the script in `index.html`:

```js
const CONFIG = {
  end:   "2026-11-30T17:00:00+01:00",   // last day, end of business (Cologne)
  start: "2026-11-01T00:00:00+01:00",   // the sun starts rising from here
  home:  { label: "Cologne", tz: "Europe/Berlin" },  // working days follow this clock
  also:  { label: "Colombo", tz: "Asia/Colombo" },
};
```

## Preview another moment

Add `?now=` to the URL, for example `?now=2026-11-30T16:00:00%2B01:00` (the last hour) or `?now=2026-12-05T09:00:00%2B01:00` (after the switch).

## Hosting

Plain static files, no build step. Served with GitHub Pages from the root of the default branch. On a phone, use "Add to Home Screen" to open it like an app.

Fonts: Bodoni Moda and Hanken Grotesk, both under the SIL Open Font License, self-hosted in `fonts/`.
