# GoogleClassroom / StudyArea

## GitHub Pages deployment

This ZIP contains the existing website and its original design, features, icons, and assets. The main page (`index.html`) and supporting files are at the repository root.

1. Extract this ZIP.
2. Upload the contents (including `index.html`, the three icon PNGs, `games/`, `images/`, and this README) to the root of your GitHub repository.
3. In GitHub, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, select your branch (usually `main`) and the `/(root)` folder, then save.

## Games

The game collection in `index.html` contains 50 entries, with the supplied game URLs and thumbnail URLs. The original site layout and game-player behavior are preserved.

**Note:** Cowboy Safari (`/cowboy-safari.embed`), Run 3 (`/run-3.embed`), and Soflo Wheelie Life (`/soflo-wheelie-life.embed`) were supplied as relative paths. They will work only if matching routes/files are available on the deployed site.

Some third-party game sites may block iframe embedding or change availability independently of this website.

## Movies

The Movies tab embeds `https://cineby.ninja/movies/` and includes an **Open Movies** fallback link. The destination may prevent third-party iframe embedding; if that happens, use the fallback link.
