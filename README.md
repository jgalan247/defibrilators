# Jersey Defibrillator Locator

A web-based emergency application for locating Automated External Defibrillators (AEDs) across Jersey, Channel Islands. The app uses geolocation and interactive mapping to help users quickly find the nearest defibrillator in medical emergencies.

## Features

- **Interactive Map**: View all 47+ defibrillator locations across Jersey
- **Geolocation**: Automatically detect your current location
- **Find Nearest AED**: Instantly identify the closest defibrillator with distance calculation
- **Turn-by-turn Directions**: Get walking/driving routes to the nearest defibrillator
- **Emergency Services**: Quick access to call 999 with GPS coordinates
- **Mobile-Responsive**: Works on all devices (phones, tablets, desktop)
- **Offline-Ready Data**: CSV-based data storage for fast loading

## Live Demo

Visit: [https://jgalan247.github.io/defibrilators/](https://jgalan247.github.io/defibrilators/)

## Quick Start

### Option 1: Open Directly
Simply open `index.html` in your web browser.

### Option 2: Run Local Server

```bash
# Python 3
python3 -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Node.js
npx http-server
```

Then navigate to `http://localhost:8000`

## Usage

1. **Allow Location Access**: When prompted, grant location permissions
2. **View Map**: All defibrillators shown as 🚨 icons
3. **Find Closest**: Click "🎯 Closest AED" to identify nearest defibrillator
4. **Get Directions**: Click "🗺️ Get Route" for turn-by-turn navigation
5. **Emergency**: Click "🚨 EMERGENCY" to call 999 with your GPS location

## Technology Stack

- **Leaflet.js** - Interactive mapping
- **Leaflet Routing Machine** - Direction routing
- **PapaParse** - CSV data parsing
- **OpenStreetMap** - Map tiles
- Pure JavaScript (no framework required)

## Data Structure

Defibrillator locations are stored in `Defibrillator.csv`:

```csv
Name,Address,Parish,Postcode,Pad,Latitude,Longitude
Mourier House,Halkett Place,St Helier,JE2 4GH,Pad 1,49.183754,-2.104754
...
```

## Browser Support

- Chrome/Edge (recommended)
- Firefox
- Safari
- Mobile browsers

**Requirements**:
- HTTPS or localhost (for geolocation API)
- JavaScript enabled
- Location services enabled (optional but recommended)

## Contributing

Contributions are welcome! To add or update defibrillator locations:

1. Fork this repository
2. Edit `Defibrillator.csv` with new location data
3. Submit a pull request

## Emergency Information

**Jersey Emergency Services**: 999

This app is designed to assist in emergencies but should not replace calling emergency services. Always call 999 first in a cardiac emergency.

## License

This project is open source and available for public use.

## Credits

Developed for the Jersey community to improve emergency response times and save lives.

## Contact

For questions or to report incorrect defibrillator locations, please open an issue on GitHub.
