# apoorva — the climb

My career story as a scrolling mountain climb. A plain static site: no build step, no frameworks.

## Put it live on GitHub Pages
1. Create a new public repo on GitHub. Name it `<your-username>.github.io` to get the address `https://<your-username>.github.io`, or use any name to get `https://<your-username>.github.io/<repo-name>`.
2. Upload everything in this folder (`index.html`, `assets/`, this README) with **Add file → Upload files**, then commit.
3. Go to **Settings → Pages**, choose **Deploy from a branch**, pick `main` and `/ (root)`, then save.
4. Wait a minute or two, then open the address shown on that page.

## Before you share it
- **CV:** add your PDF to this folder and name it `cv.pdf`. The "Download my CV" button links to it.
- **Email:** the site uses `apoorva.k@u.nus.edu`. To change it, edit `EMAIL` in the script near the bottom of `index.html` and the address in the letter section.

## Swapping in the real illustrations
The placeholder art is in `assets/`. Four poses: `me-walk`, `me-chai`, `me-rain`, `me-summit`.
1. Save your images as PNGs with transparent backgrounds, for example `assets/me-walk.png`.
2. In `index.html`, find `const POSES = {...}` near the bottom and change `.svg` to `.png`.
3. Also change the hero image (search for `assets/me-walk.svg`, which appears twice).

Tall images work best, roughly 1:2 (width:height), with the feet at the bottom edge.

## Where to edit the words
Each stop on the trail is an `<article class="ch">` in `index.html`:
- `data-t`: how far up the trail it sits (0 = bottom, 1 = summit)
- `data-pose`: which illustration shows (`walk`, `chai`, `rain`, `summit`)
- `data-pack`: the label that drops into the "Packed so far" backpack
