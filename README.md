# GitHub Pages upload kit

The 404 you saw happens because GitHub Pages did not find `index.html` at the site root.

## Upload these files to the ROOT of the repo (not a subfolder)

| File | Action |
|---|---|
| `index.html` | Required. This is the website. |
| `favicon.svg` | Required. Tab icon. |
| `profile.svg` | Required fallback photo (VI hexagon). |
| `Vaibhav_Sudhakar_Ingle_Resume.pdf` | Required. Download Resume button. |
| `.nojekyll` | Required. Stops Jekyll from hiding files. |
| `404.html` | Optional. Sends unknown URLs back to the site. |
| `profile.jpg` | **You add this.** Your photo. Same folder, this exact name. |

Until `profile.jpg` is present, the site shows `profile.svg`.

## GitHub Pages settings

1. Open the repository on GitHub.
2. **Settings → Pages**.
3. **Build and deployment → Source:** Deploy from a branch.
4. **Branch:** `main` (or `master`) and folder **`/ (root)`**.
5. Save. Wait 1–2 minutes, then open the Pages URL.

Do **not** set the folder to `/docs` unless these files actually live in a `docs` folder.

## If the repo is a project site

URL will look like:

`https://vaibhavingle2002.github.io/YOUR-REPO-NAME/`

`index.html` must still be at the **root of that repo**, not inside `src/` or `public/`.

## Exact names for your photo and resume

```
profile.jpg
Vaibhav_Sudhakar_Ingle_Resume.pdf
```

Case-sensitive. `Profile.JPG` will not load.
