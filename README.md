# Global Digital ID Landscape

Interactive visualization of digital ID systems worldwide for BC Government Digital Trust Initiative.

![Preview](preview.png)

## Features

- **45+ jurisdictions** tracked across 20+ countries
- **Subnational coverage**: US states, Canadian provinces, Australian states
- **Filters**: Status (Live/Spec), Region
- **Deep details**: Technology specs, metrics, no-device solutions
- **Verified URLs**: All links tested and working

## Quick Start

### Option 1: GitHub Pages (Recommended)

The site is hosted at: **Coming soon**

1. Enable GitHub Pages in repo Settings → Pages
2. Deploy from `main` branch
3. Visit: `https://krobinsonca.github.io/global-digital-id/`

### Option 2: Local Development

```bash
# Clone the repo
git clone https://github.com/krobinsonca/global-digital-id.git
cd global-digital-id

# Start a local server (required for fetch to work)
python3 -m http.server 8080

# Open in browser
open http://localhost:8080
```

Or use any static server:

```bash
# Node.js
npx serve .

# PHP
php -S localhost:8080
```

## Data Source

All data lives in `data.json` - edit this file to update jurisdictions:

```json
{
  "jurisdictions": [
    {
      "name": "Country Name",
      "flag": "cc",
      "region": "eu",
      "status": "production",
      "issuanceModel": "single",
      "url": "https://...",
      "technology": "...",
      "description": "...",
      "details": [...],
      "nodevice": [...],
      "metrics": [{"label": "...", "value": "..."}]
    }
  ]
}
```

### Fields

| Field | Description |
|-------|-------------|
| `status` | `production` (live) or `specification` (planned) |
| `issuanceModel` | `single` (one ID/person), `multiple` (multiple IDs), `cloud` (account-based) |
| `isSubnational` | `true` for states/provinces |
| `parent` | Parent country for subnationals |
| `nodevice` | How users without devices can verify |

## Project Structure

```
global-digital-id/
├── index.html      # Main visualization
├── data.json       # Single source of truth
├── flags/          # Country flag images (PNG)
├── presentation.html # Slide deck (optional)
└── README.md
```

## License

MIT
