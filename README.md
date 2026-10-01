# HELIX Origin

The [HELIX Origin GitHub Pages homepage](https://helix-origin.github.io/) is a static profile and project directory based on [vCard – Personal Portfolio](https://github.com/codewithsadee/vcard-personal-portfolio) (MIT license; see [LICENSE](LICENSE)).

## Publishing the homepage

In this repository's **Settings → Pages**, publish from the root of the default branch (or deploy that root through a Pages workflow). GitHub Pages serves `index.html` at `https://helix-origin.github.io/`. This repository must be eligible for GitHub Pages under the organization's plan and visibility settings.

## Publishing project subpages

Each project repository publishes **its own** Pages site. In each repository's **Settings → Pages**, choose a branch and site directory containing an `index.html`, or deploy built static files through a Pages workflow. GitHub serves that site at `https://helix-origin.github.io/<repository-name>/`. This homepage links to those paths, but cannot configure or deploy other repositories. Until a project's site is published, its Project page link may return 404; its Source on GitHub link will still work.

To add or rename a project, update its card in `index.html` with the exact case-sensitive repository name in both the Pages URL and GitHub source URL. Use relative asset paths (such as `./assets/style.css`) in each project site so its CSS, scripts, and images resolve beneath `/<repository-name>/`.

To preview this site locally, run `python3 -m http.server` from the repository root and open `http://localhost:8000/`.