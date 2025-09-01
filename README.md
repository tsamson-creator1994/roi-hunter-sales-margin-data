
# ROI Hunter Business Data – Public Feed

This folder is ready to be published as a public, shareable CSV link (similar to a product feed). It includes:

- `roi_hunter_business_data.csv` – your data file
- `index.html` – a simple landing page that links to the CSV
- `.nojekyll` – prevents Jekyll processing on GitHub Pages

## Option A: Publish via GitHub Pages (Open & Free)

1. Create a **public** GitHub repository (e.g., `roi-hunter-business-data`).
2. Upload the contents of this folder to the repository root.
3. In **Settings → Pages**, set **Build and deployment** to **Deploy from branch**, and pick `main` (root).
4. After it deploys, your CSV will be available at:

```
https://<your-user-or-org>.github.io/roi-hunter-business-data/roi_hunter_business_data.csv
```

Use that URL in ROI Hunter as your Business Data source.

## Option B: Publish via Amazon S3 (Public Object)

1. Create an S3 bucket (e.g., `roi-hunter-business-data`), enable public access for the object or use a bucket policy.
2. Upload `roi_hunter_business_data.csv` with **Content-Type: text/csv**.
3. The public URL will be something like:

```
https://<bucket>.s3.<region>.amazonaws.com/roi_hunter_business_data.csv
```

## Option C: Any Static Host

You can also host these files on Netlify, Cloudflare Pages, Google Cloud Storage, Azure Blob Static Website, or your own server. Ensure the CSV is publicly readable and served with `text/csv` if possible.

## Pairing in ROI Hunter

- Pairing field: **first column** (e.g., `Product ID`)
- Map the remaining columns as attributes.
- Update cadence: daily is typical.

