# IQGambit

IQGambit is a static chess practice site. It has no build step or server-side database. The site to publish is in `outputs/chess-club/`.

## Publishing

This repository includes a GitHub Pages workflow in `.github/workflows/publish-pages.yml`. After you publish this repository to GitHub and set Pages to use **GitHub Actions**, every push to `main` will publish the contents of `outputs/chess-club/`.

The Stockfish full-strength engine file is about 95 MiB. Keep GitHub's command-line upload limit in mind: the website upload form has a smaller per-file limit, so publish with GitHub Desktop or Git rather than uploading files through the browser.

Keep both Stockfish engine folders and their `Copying.txt` license files with the site. Progress and saved games stay in each visitor's browser; this version does not provide accounts, cloud sync, multiplayer, or shared club scores.

After publishing, GitHub Pages shows the public address under **Settings → Pages**. For a project repository, the address usually has the form `https://OWNER.github.io/REPOSITORY/`.
