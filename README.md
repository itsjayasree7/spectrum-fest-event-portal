# Spectrum Fest 2026: College Event Portal

A responsive, single-page website for a fictional three-day college festival. Visitors can browse and filter events, view the day-wise schedule, see a gallery, register for an event, and send an enquiry. It is built with HTML5, CSS3, and vanilla JavaScript, with no frameworks or libraries.

> **Academic project.** Spectrum Fest is a made-up event. The contact details are placeholders and no data is sent anywhere.

## Features

- **Home page** with a hero section, festival highlights, and a live announcements panel where you can post new announcements
- **Events section** with 12 events across four categories (Technical, Cultural, Sports, Fun), filterable by category and date
- **Register button on each event** that jumps to the form with that event already selected
- **Schedule** generated from the event data, grouped by day and sorted by time
- **Gallery** of themed tiles built with CSS gradients and emoji, so no image files are needed
- **Registration form** with inline validation:
  - Name: letters only, minimum 3 characters
  - Email: valid format
  - Mobile: 10 digits starting with 6–9
  - Department, year, and event: required
- **Enquiry form** with validation and a confirmation message
- **Responsive layout** with tablet and mobile breakpoints and a collapsible mobile menu
- **Accessibility:** labelled fields, ARIA live regions, visible focus styles, and reduced-motion support

## Tech stack

- HTML5
- CSS3 (custom properties, Grid, Flexbox, media queries)
- Vanilla JavaScript

There are no dependencies and no internet connection is needed.

## Run it

No build step. Clone the repo and open `index.html` in a browser.

```bash
git clone https://github.com/<your-username>/spectrum-fest-event-portal.git
cd spectrum-fest-event-portal
# then open index.html
```

## Project structure

```
├── index.html    # markup, styles and scripts in one file
├── README.md
└── LICENSE
```

## Customising

All event, gallery, and announcement content lives in three arrays at the top of the `<script>`: `events`, `gallery`, and `announcements`. Edit those and the cards, schedule, dropdowns, and gallery update automatically.

## Limitations

- Registrations, enquiries, and new announcements are not saved or sent anywhere. They reset when the page is refreshed.
- There is no backend, so no confirmation email is actually sent.

## Possible next steps

- Save registrations with `localStorage` or a backend
- Prevent duplicate registrations for the same event
- Send real confirmation emails
- Replace the gallery tiles with real photos

## License

[MIT](LICENSE)
