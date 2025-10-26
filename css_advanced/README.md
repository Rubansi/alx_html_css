# css_advanced

A small collection of intermediate-to-advanced CSS examples and exercises used in the ALX HTML/CSS track. The folder contains a few demo pages, multiple stylesheets, and an images folder with assets used by the examples.

## Contents

- `index.html` — Primary demo page demonstrating layout and advanced CSS techniques.
- `index1.html` — Alternate/example layout showcasing other styles or component variations.
- `styles.css` — Main stylesheet used by the demos.
- `stylesheet.css` — Additional stylesheet with helper rules and alternate styles.
- `images/` and `Images/` — Asset folders containing PNGs (icons, logos, and illustrations) used by the pages. Note: both folders exist in the repository; on case-sensitive filesystems this matters.

Then open `http://localhost:8000/css_advanced/index.html` in your browser.

Option 3 — Use editor extension
- If you use VS Code, the Live Server extension can serve the folder and reload changes automatically.

## Development notes & tips

- Paths are relative in the HTML files; if you move files, update the relative paths to the stylesheets and images.
- There are two image directories: `images/` and `Images/`. On Windows/macOS (case-insensitive by default) this may not be a problem, but on Linux it is. Consider consolidating into a single `images/` folder to avoid confusion.
- The repository includes two stylesheet files (`styles.css` and `stylesheet.css`). Check the HTML `link` tags to see which files are being loaded by each page.
- Test in multiple browsers if you are experimenting with newer CSS features (Grid, custom properties, etc.). Use the browser devtools to inspect computed styles and layout.

## Conventions

- Keep presentation (CSS) separate from content (HTML).
- Use meaningful class names. Consider a lightweight naming convention (BEM) for larger experiments.

## Contributing

If you want to add examples or fixes:

1. Fork the repository.
2. Add a new example directory or update an existing file.
3. Submit a pull request with a description of the change and the files modified.

## Credits & Author

Repository owner: `Rubansi` (ALX student exercises)

## License

No license specified. 

