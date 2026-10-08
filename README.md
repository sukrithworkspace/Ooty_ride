# 🌿 OotyRide

A premium Ooty sightseeing and vehicle trip request website. It is a single-file site (HTML, CSS and JavaScript in `index.html`) with no build step and no dependencies. Bookings are prepared in the browser and sent to your team through WhatsApp.

## ✨ Features

- **AI Trip Planner**: pick the number of people, days and travel style, and get a recommended vehicle, a day-wise route and a rough price estimate
- **20 sightseeing places** across Ooty, Coonoor, Kodaikanal and Munnar, with category filters
- **Map and nearby help**: each place opens a Google Maps view with tabs for restaurants, medical shops and hospitals
- **Vehicle guide**: Sedan, SUV, Innova and Tempo Traveller, recommended automatically by group size
- **4-step booking flow**: group, places, vehicle and details, then a pre-filled WhatsApp message
- **Change / Cancel** requests sent through WhatsApp
- **Live weather**: current conditions and a 7-day forecast from [Open-Meteo](https://open-meteo.com/) (no API key needed), plus travel-date advice
- **Traveller reviews**, stored in the visitor's browser
- **Built-in chat assistant** for places, vehicles, prices and booking
- **Emergency section** with quick links to 112 and your team
- Fully responsive layout with a mobile bottom bar and bottom-sheet modals

## 🚀 Getting Started

1. Download or clone this repository.
2. Open `index.html` in any modern browser.

That's all. There is nothing to install.

## ⚙️ Configuration

Open `index.html` and edit these two lines near the top of the `<script>` section:

```js
const WA_NUMBER = "919999999999";     // WhatsApp number with country code, no +
const CALL_NUMBER = "+919999999999";  // Phone number for the Call buttons
```

### Other things you can customise

| What | Where in `index.html` |
|------|-----------------------|
| Places, photos and descriptions | `PLACES` array |
| Vehicles and capacities | `VEHICLES` array |
| Price per day for each vehicle | `estimate()` function |
| Planner day-wise routes | `routes` inside `createPlan()` |
| Colours and theme | CSS variables in `:root` |

## 🌐 Deploy on GitHub Pages

1. Create a new repository and upload `index.html` and `README.md`.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select the `main` branch and the `/ (root)` folder, then click **Save**.
5. Your site will be live at `https://<your-username>.github.io/<repository-name>/` after a minute or two.

## 🖼️ About the images

Some place and vehicle images are linked from external websites. These links can expire or block hotlinking. If a place image fails to load, the site shows a green gradient instead. For a reliable production site, add your own photos:

1. Create an `images/` folder in the repository.
2. Add your photos, for example `images/doddabetta.jpg`.
3. Update the `image` field of each item in `PLACES` and `VEHICLES` to the new path.

## 📝 Notes

- This is a **front-end only** project. Bookings and reviews are stored in the visitor's own browser (`localStorage`), so you will not see them on a server. Your real booking records arrive through WhatsApp.
- Prices shown are **rough estimates** only. Final pricing is confirmed by your team.
- The weather forecast needs an internet connection.

## 🛠️ Tech Stack

- HTML5, CSS3 (cascade layers, grid, flexbox) and vanilla JavaScript
- Google Fonts: Cinzel and Outfit
- Open-Meteo API for weather
- Google Maps embeds for place maps

## 📄 License

All rights reserved © 2026 OotyRide, unless you choose to add an open-source license (for example MIT) to this repository.

## 📞 Contact

**OotyRide**, Ooty, Nilgiris, Tamil Nadu, India

Add your WhatsApp, phone and email details here.
