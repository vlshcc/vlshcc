# vlsh.cc

Static website for [vlsh](https://github.com/vlshcc/vlsh), hosted by GitHub Pages
from the root of the `main` branch. `CNAME` configures https://vlsh.cc/.

The page is `index.html`, with styles in `style.css` and inline JavaScript for
installation tabs and copy buttons. No build step or dependencies are required.

Preview from this directory:

```sh
python3 -m http.server 8080
```

Open http://localhost:8080 and check the installation tabs, copy buttons, and
layout on desktop and mobile sizes before changing styles or interactions.

Keep the feature and installation copy aligned with the shell's
[README](https://github.com/vlshcc/vlsh/blob/main/README.md),
[POSIX inventory](https://github.com/vlshcc/vlsh/blob/main/docs/posix-inventory.md),
[testing guide](https://github.com/vlshcc/vlsh/blob/main/docs/testing.md), and
[changelog](https://github.com/vlshcc/vlsh/blob/main/CHANGELOG.md).

Verify download links against the actual GitHub release assets. The current
published tag is `v1.2`, while its package version is `1.2.0`; it includes the Linux
`.deb` and standalone binary, plus FreeBSD and DragonFly binaries, and has no RPM
asset. Source instructions target `main` and may include changes absent from the
published packages. Do not label source updates as a new release until it exists.
