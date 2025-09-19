## SF Airbnb Listings (First 50 via Fetch/Await)

This page loads the first 50 Airbnb listings from `airbnb_sf_listings_500.json` using JavaScript `fetch` and `await`, and renders:

- Name
- Description
- Amenities
- Host name and photo
- Price
- Thumbnail
- Rating

Creative additions:
- Favorites with localStorage and a “Show favorites only” toggle
- Live search (name/amenities) and minimum rating filter
- Dynamic theme accent based on the average price of the displayed set

### Demo

Deployed on GitHub Pages: [Live site](https://YOUR_GITHUB_USERNAME.github.io/REPO_NAME/)

Replace with your URL after enabling Pages.

### Getting started locally

Browsers block `fetch` for `file:///` URLs. Serve the folder with a local web server.

Option A: Python 3
```bash
cd "A2_JS DOM Self Assessment"
python3 -m http.server 5173
```
Open `http://localhost:5173`.

Option B: Node (npx serve)
```bash
cd "A2_JS DOM Self Assessment"
npx --yes serve -l 5173
```
Then open `http://localhost:5173`.

### Project structure

- `index.html`: Markup, minimal styles, and controls
- `script.js`: Fetches JSON, renders first 50, filters, favorites, dynamic accent
- `airbnb_sf_listings_500.json`: Data source

### Implementation notes

- `fetch('airbnb_sf_listings_500.json')` loads the dataset; render caps at 50 items.
- Amenities are JSON-stringified arrays in the dataset; parsed via `JSON.parse`.
- Description may contain HTML; it’s normalized to text before display.
- Favorites persist in `localStorage` under the key `sf_favorites`.

### Deploying to GitHub Pages

1. Push this folder to a GitHub repository.
2. Settings → Pages → set branch to `main` (or `master`) and root.
3. Save. Copy the provided URL and update the Demo link above.

### Credits

Dataset: In-course sample subset of San Francisco Airbnb listings.


