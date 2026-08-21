# Anna Lukose — E-Portfolio

A single-page site styled as a physical filing system. `index.html` contains everything
(HTML, CSS and JavaScript) so there is nothing to build and nothing to install.

```
index.html                 the whole site
images/                    your photos go here
files/Anna_Lukose_CV.pdf   the CV the Contact page links to
```

---

## 1. Add your photo

Save a portrait as **`images/anna.jpg`** — that is the picture on the front-facing file
on the home page. Portrait orientation works best (roughly 800 × 1000 px). No code
changes needed; the file just has to have that exact name.

Until an image exists, the site shows a striped placeholder telling you which filename
it is waiting for. That is deliberate — nothing looks broken while you gather photos.

## 2. Add the rest of the images

Same idea. Drop these into `images/` using these exact names:

| Filename | Where it appears |
| --- | --- |
| `anna.jpg` | Home — front-facing profile file |
| `anna-working.jpg` | About |
| `hpc-team.jpg` | About — Team South Africa |
| `teaching.jpg` | About — CHPC lecturing |
| `certificate-huawei.jpg` | Education — certification |
| `deans-list.jpg` | Education — Dean's List |
| `competition-award.jpg` | Education — 2nd place |
| `solar-1.jpg` `solar-2.jpg` `solar-3.jpg` | Experience — internship |
| `marine-snow.jpg` | Projects — research pipeline |
| `cluster.jpg` | Projects — HPC |
| `embedded.jpg` | Projects — embedded systems |
| `solar-design.jpg` | Projects — solar |
| `network.jpg` | Projects — data comms |

Screenshots count as artefacts too: a plot from the marine-snow pipeline, a terminal
showing benchmark output, a photo of a lab bench. Those score better than stock images.

To change a caption or filename, search `index.html` for `data-need=` — the filename
appears twice on each image (in `src` and in `data-need`); change both.

## 3. Replace the placeholder links

In `index.html`, search for `YOUR-LINKEDIN` and `YOUR-USERNAME` on the Contact page and
paste in your real profile URLs. If you would rather not publish your phone number,
delete the `<div><dt>Phone</dt>…</div>` line in the same section.

## 4. Publish it (GitHub Pages — free, gives you one link)

1. Create a GitHub account, then a new **public** repository. Name it anything, e.g. `portfolio`.
2. On the repo page choose **Add file → Upload files**, drag in `index.html`, the
   `images` folder and the `files` folder, and commit.
3. Go to **Settings → Pages**. Under *Source* choose **Deploy from a branch**, pick
   `main` and `/ (root)`, and save.
4. Wait about a minute and refresh. Your link appears at the top of that page:
   `https://YOUR-USERNAME.github.io/portfolio/`

That URL is what you hand in. Any file you upload later goes live the same way.

**Netlify Drop** is an alternative if you would rather not use Git: go to
`app.netlify.com/drop` and drag the whole folder onto the page. It returns a live link
in seconds. Rename the site under *Site settings* to get a tidier URL.

## Checking it before you publish

Open `index.html` in a browser by double-clicking it. Everything works locally except
Google Fonts, which need an internet connection to load.
