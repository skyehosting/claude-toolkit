# claude-toolkit — the site

The marketing page for **toolkit v5**, published with GitHub Pages at
<https://skyehosting.github.io/claude-toolkit/>.

One file, `index.html`: no build step, no framework, no dependency beyond two webfonts.
Edit it and push — Pages rebuilds on its own.

The toolkit itself lives in a **private** repository, `skyehosting/claude-toolkit-src`, and
the download links here point at its releases. They 404 for anyone without access, which is
the point: the page is public, the plugin is not.

## Checked at

`node "<toolkit>/cli/capture.js" index.html --set all` — monitors 1920x1080 at 100%, 125%
and 150%, 2560x1440 and 3440x1440 at 100%, a 960x1040 window, a 360x800 phone and an
820x1180 tablet.
