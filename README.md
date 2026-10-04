# LEVEL UP — Gaming Club Website

## Project Overview

LEVEL UP is a responsive, multi-page website for a fictional gaming club, created as a university project. It introduces the club, compares gaming zones and prices, and shows a static booking form. All website content is in English.

## Technologies

- HTML5
- CSS3
- Bootstrap CSS, stored locally in `vendor/bootstrap/`

## Pages

- **Home — `index.html`:** Club introduction, gaming illustration, and three benefits.
- **Gaming Zones — `zones.html`:** Standard PC, VIP PC, and Console Zone cards with equipment lists.
- **Pricing — `pricing.html`:** A table of demo rates in KZT and package notes.
- **About — `about.html`:** The fictional club story, equipment, and house rules.
- **Booking — `booking.html`:** A static form with name, email, gaming zone, date, and time fields.

## Implemented Features

The pages share navigation and a footer. The current page is marked with `aria-current="page"`. The site includes responsive layouts, three local SVG illustrations, a scrollable pricing table, labeled form fields, skip links, and visible keyboard focus styles.

| Requirement | Implementation |
| --- | --- |
| Semantic HTML and shared navigation | All five HTML files use `header`, `nav`, `main`, and `footer`, with shared `.nav-list` links. `section` and `article` organize content in `index.html`. |
| Images, lists, `div`, and `span` | `zones.html` uses `img` with descriptive `alt` text, `ul.feature-list`, `div.zone-content`, and `span.popular-badge`. `about.html` includes `ol.rules-list`. Images are in `images/`. |
| Pricing table | `pricing.html`: `table.price-table`, `caption`, `thead`, `tbody`, and `th` with `scope`. `.table-wrapper` in `css/style.css` allows horizontal scrolling. |
| Booking form | `booking.html`: `form#booking-form`, linked `label` elements, four inputs, one `select`, a `type="button"` button, and a visible demo notice. |
| CSS classes and ID selectors | `css/style.css`: classes such as `.zone-card` style repeated content; `#hero` and `#hero h1` style the Home introduction. |
| Flexbox | `css/style.css`: `.header-content`, `.nav-list`, `.footer-content`, and `.button-group` use `display: flex` with wrapping. |
| CSS Grid | `zones.html` uses `.zones-grid`; `css/style.css` sets `display: grid` and three columns by default. |
| Relative and absolute positioning | `css/style.css`: `.zone-card` uses `position: relative`; `.popular-badge` uses `position: absolute` to place the Popular label on the VIP card in `zones.html`. |
| Bootstrap Grid and utility classes | `index.html`: `.container`, `.row`, `.col-12`, `.col-lg-6`, and `.col-md-4`; utilities include `.g-4`, `.mb-0`, `.mt-3`, `.text-center`, and `.align-items-center`. |
| Tablet and mobile media queries | `css/style.css`: `@media (max-width: 992px)` changes the zone grid to two columns and places navigation below the brand. `@media (max-width: 576px)` changes it to one column and reduces headings and spacing. |

## Project Structure

```text
assignment3-web/
├── index.html
├── zones.html
├── pricing.html
├── about.html
├── booking.html
├── README.md
├── css/
│   └── style.css
├── images/
│   ├── standard-pc.svg
│   ├── vip-pc.svg
│   └── console.svg
└── vendor/
    └── bootstrap/
        ├── bootstrap.min.css
        ├── bootstrap.min.css.map
        └── LICENSE
```

## How to Run

Double-click `index.html` to open it in a browser, then use the navigation to visit the other pages. Keep the folders together so styles and images load correctly. No server or installation is needed.

## Demo Limitations

The club and its prices are fictional. Prices are shown in KZT.

The booking form is a static demonstration. It does not send, store, or process personal information and does not create bookings. Its `type="button"` button does not submit or validate the form. The visible notice reads: "Demo form only. No booking will be made."

## Deployment

Deployment is pending. A public URL will be added after publishing.
