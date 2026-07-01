# The Scenic Route

This repo takes advantage of a GitHub pages deployment to deploy and host each of the Scenic Route games. The repo name must remain as `caminocomms.github.io`. A CNAME and route 53 record is created to map the GitHub pages installation to https://scenicroute.caminocomms.com/.

We take advantage of the repo directory structure to map a path prefix (subdirectory) to a different `index.html`

E.g:
- https://scenicroute.caminocomms.com/flappy-bird/
- https://scenicroute.caminocomms.com/gold-fish/

The original crossword game is served at both the site root and prefix `crossword`. 

## Adding a new game

Create a folder with the name of the required path prefix and upload the `index.html` file (+ external assests if required etc). Ensure the `.html` file is named to `index.html`.

On committing, the GitHub Actions pages deploy will automatically run, upon success the new game will be accessible at https://scenicroute.caminocomms.com/{folder-name}
