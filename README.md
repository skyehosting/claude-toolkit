# claude-toolkit — the site

The marketing page for **toolkit v5**, published with GitHub Pages at
<https://skyehosting.github.io/claude-toolkit/>.

One file, `index.html`: no framework and no dependency beyond its three webfonts (Inter Tight, Inter,
JetBrains Mono). It is generated, on the machine that publishes it, from `.toolkit/build/` (kept out of
git: `content.js` holds every word, `final.js` the page; `node build.js`), and checked by a five-judge
design review before it ships. Edit there, rebuild, copy the result over `index.html`, and push: Pages
rebuilds on its own.

The toolkit itself lives in a **private** repository, `skyehosting/claude-toolkit-src`, and
the download links here point at its releases. They 404 for anyone without access, which is
the point: the page is public, the plugin is not.

## Requests for access

The page's **Request access** button opens the issue form in
`.github/ISSUE_TEMPLATE/request-access.yml`: a signed-in GitHub user asks for the download, and the
request arrives here as a public issue labelled `access request`. To grant it, invite that account to
`claude-toolkit-src`, then close the issue. The link carries only `?template=`, because GitHub answers
a link with parameters the visitor may not set (labels, assignees) with a 404.

## Checked at

`node "<toolkit>/cli/capture.js" index.html --set all` — monitors 1920x1080 at 100%, 125%
and 150%, 2560x1440 and 3440x1440 at 100%, a 960x1040 window, a 360x800 phone and an
820x1180 tablet; also a 320x700 phone. Add `?static` to the address for still shots (no fade-ins).
