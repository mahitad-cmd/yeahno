# AERO // Elite Weather Intelligence

AERO is a premium static weather dashboard built as a single-file web experience. It delivers a modern editorial interface with live weather search, hourly trend visualization, and a multi-day forecast ledger.

This repository is hosted at `https://github.com/mahitad-cmd/yeahno.git` and the default branch is `main`.

## What it includes

- `weather.html` — all HTML, CSS, and JavaScript in one static page
- Responsive design for desktop and mobile
- Search-driven weather lookup by city name
- Current weather metrics: temperature, humidity, wind, sunrise, and sunset
- 24-hour hourly forecast strip
- 5-day forecast ledger
- Heatwave advisory banner for hot conditions
- Demo fallback simulation when API access is unavailable

## Features

- Live OpenWeatherMap integration for current and forecast data
- Fallback mode when `API_KEY` is missing or request fails
- Elegant typography with Google Fonts
- Lucide icon rendering via CDN
- Built to run without a build system or server-side code

## Setup

1. Clone this repository:

```bash
git clone https://github.com/mahitad-cmd/yeahno.git
cd yeahno
```

2. Open `weather.html` in a browser.

### Configure an OpenWeatherMap API key

To enable live weather data, add your OpenWeatherMap API key:

1. Sign up at [OpenWeatherMap](https://openweathermap.org/).
2. Create an API key.
3. Open `weather.html` and update the `CONFIG` block:

```js
const CONFIG = {
    API_KEY: 'YOUR_API_KEY_HERE',
    ENDPOINT: 'https://api.openweathermap.org/data/2.5/'
};
```

4. Replace `'YOUR_API_KEY_HERE'` with your actual key.

## Usage

- Type a city name in the search input.
- Press Enter to load the weather data.
- If the API fails or the key is missing, the page falls back to simulated demo data automatically.

## Notes

- Temperature is displayed in degrees Celsius (`°C`).
- Wind speed is shown in meters per second (`m/s`).
- The app is designed for static hosting and requires only a browser.

## Deployment

Deploy `weather.html` to any static hosting platform:

- GitHub Pages
- Netlify
- Vercel
- Surge
- Any static file server

## Contributing

This repo is currently a single-file project. If you want to enhance it, you can:

- add an API key management workflow
- make units toggle between Celsius and Fahrenheit
- improve error handling and user messaging
- localize the interface for multiple languages

## License

Provided as-is with no warranty.
