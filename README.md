# EODigitalTwins

A ready-to-publish Jupyter Book for Earth Observation Digital Twins.

## Before publishing

Replace `maralbayaraa` in `WhitePaper/_config.yml` and in the URL below with your GitHub user or organization name.

Published book URL:

`https://maralbayaraa.github.io/EODigitalTwins/`

## Build locally

```bash
python -m venv .venv
source .venv/bin/activate  # Windows PowerShell: .venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
jupyter-book build WhitePaper
```

Open `WhitePaper/_build/html/index.html` in a browser.

## Upload to GitHub

Create an empty GitHub repository named `EODigitalTwins`, then run:

```bash
git init
git branch -M main
git add .
git commit -m "Initialize EODigitalTwins Jupyter Book"
git remote add origin https://github.com/maralbayaraa/EODigitalTwins.git
git push -u origin main
```

In GitHub, open **Settings > Pages** and set **Source** to **GitHub Actions**. Every push to `main` will rebuild and deploy the book.

## Structure

- `WhitePaper/`: Jupyter Book source
- `WhitePaper/_config.yml`: title, repository, and build settings
- `WhitePaper/_toc.yml`: navigation and chapter order
- `.github/workflows/deploy-book.yml`: GitHub Pages deployment
- `requirements.txt`: pinned build dependencies

## License

The template is available under the MIT License. Replace or extend the license if your book content requires different terms.
