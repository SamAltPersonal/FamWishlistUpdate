# Wishlist Links — GitHub Pages

A lightweight, responsive wishlist directory. It uses no framework or build step and follows each visitor's device/browser light or dark preference.

## Files

- `index.html` — website layout, styling, favicon loading, and rendering
- `people.json` — the list of people and their links
- `images/` — upload photos or icons here

## Add or edit a person

Open `people.json` on GitHub and click the pencil (Edit) button. Copy an existing person object and change the fields:

```json
{
  "name": "Taylor Smith",
  "note": "Christmas 2026",
  "image": "images/taylor.jpg",
  "links": [
    {
      "label": "Amazon wishlist",
      "url": "https://www.amazon.co.uk/your-wishlist"
    },
    {
      "label": "Other gift ideas",
      "url": "https://example.com/list"
    }
  ]
}
```

- `name` is required.
- `note` is optional; use it for “Birthday”, “Christmas 2026”, etc.
- `image` is optional. Upload the image into `images/`, then enter its path. Use an empty string (`""`) for initials instead.
- `links` can contain as many links as you need. Each link needs a `url`; `label` is optional and defaults to the website domain.
- Keep the commas and quotation marks valid JSON. Separate people with commas, but do not add a comma after the final person.

## Upload a photo

1. Open the repository on GitHub.
2. Open the `images` folder.
3. Choose **Add file → Upload files**.
4. Upload the image and commit the change.
5. In `people.json`, set that person's `image` to e.g. `"images/taylor.jpg"`.

Use simple filenames without spaces, such as `taylor.jpg` or `sam-icon.png`.

## Publish with GitHub Pages

1. Create a repository on GitHub (for GitHub Free, use a public repository).
2. Upload `index.html`, `people.json`, and the `images` folder contents to the repository's root.
3. Open **Settings → Pages**.
4. Under the build/deployment section, select **Deploy from a branch**.
5. Choose the `main` branch and `/(root)`, then save.
6. Wait for deployment and open the URL shown on the Pages settings screen.

The website is public. Anyone with the URL can view the names, photos, and wishlist links, and the repository contents may be public too. Avoid including private information.

## Notes

- Link favicons are loaded from Google's favicon endpoint. A fallback arrow appears if a favicon can't be loaded.
- GitHub Pages can take a few minutes to publish changes.
- This is a static site, so there is no sign-in/admin page. Make changes in GitHub and commit them.
