# 🎵 MJ Song Ranker

Ranking game for Michael Jackson, Jackson 5 and The Jacksons using A-vs-B song comparisons.

## Project structure

```text
mj-ranking/
├── index.html
├── README.md
├── .gitignore
├── LICENSE.txt
└── assets/
    └── image-*.png
```

The images are stored separately in `assets/` so that `index.html` stays lightweight and easy to version/deploy.

## Stack

- HTML / CSS / JavaScript
- Firebase Authentication (Google)
- Cloud Firestore
- IndexedDB

## Deployment

Recommended:

```text
GitHub → Render → Firebase
```

Render can host this as a static site. Firebase provides Google authentication and cloud persistence.

## Development

Serve the folder through HTTP rather than opening `index.html` directly with `file://`:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Security

Firestore data is intended to live under:

```text
users/{userId}/...
```

and be protected using the authenticated user's Firebase UID.

## Status

🚧 In development.
