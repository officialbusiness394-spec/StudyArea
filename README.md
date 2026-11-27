# GoogleClassroom / StudyArea

## GitHub Pages deployment

This is the complete static website. The main page (`index.html`) and its image assets are at the repository root, so you can upload these files directly to the root of a GitHub repository.

1. Extract this ZIP.
2. Upload `index.html`, `classroom-icon.png`, `docs-icon.png`, and this README to your repository's root (not inside an extra nested folder).
3. In GitHub, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, select your branch (usually `main`) and the **/(root)** folder, then save.

## Movies tab

The Movies tab embeds `https://cineby.ninja/movies/` and includes an **Open Movies** fallback link to the same page. The site may prevent third-party iframe embedding through its own security policy; if that happens, visitors can use the fallback link.

The YouTube Shorts tab/code and the soundboard are not included. The previous movie embeds and services have been removed. Existing games, visual design, layout, and icons are retained.

## Additional UGS games

The site includes the 30 UGS games from the previous build plus 8 remaining safe titles from the supplied list. Among Us is already in the original game collection, so it is not duplicated. The two weapon-focused titles in the supplied list were not added.

UGS HTML files are fetched as text and then rendered inside the game's iframe using `srcdoc`. This handles jsDelivr's `text/plain` content type for HTML files. The game wrappers retain their own `<base>` URL where supplied so their remote assets can load. A working internet connection and availability of the third-party CDN are required.
