## SF Airbnb Listings (First 50 via Fetch/Await)

This page loads the first 50 Airbnb listings from `airbnb_sf_listings_500.json` using JavaScript `fetch` and `await`, and renders:

- Listing Title
- Host name and Image
- Price
- Rating
- Description
- Amenities

### Demo

Deployed on GitHub Pages: [Live site](https://chirag-nx.github.io/)

Replace with your URL after enabling Pages.

### Getting started locally

Browsers block `fetch` for `file:///` URLs. Serve the folder with a local web server.

Option A: Python 3
```bash
cd "A2_JS DOM Self Assessment"
python3 -m http.server 8080
```
Open `http://localhost:5173`.

Option B: Node (npx serve)
```bash
cd "A2_JS DOM Self Assessment"
npx --yes serve -l 8080
```
Then open `http://localhost:5173`.


