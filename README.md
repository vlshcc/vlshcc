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
published tag and package version are `v1.2.1` and `1.2.1`. The release includes
Linux `.deb` and `.rpm` packages, a standalone Linux binary, cross-compiled
FreeBSD and DragonFly binaries, and `SHA256SUMS`. Keep installation examples
aligned with these exact asset names.

Release v1.2.1 includes ordered builtin/external redirections, shell-local
variables and export tracking, field splitting after expansion, positional
parameters, multiline simple-command lists, command lookup statuses 126/127,
and interactive backslash continuations. Continued commands are recalled and
saved as one history entry; Ctrl+C cancels the whole command.

Keep the remaining grammar gaps visible: command substitution, arithmetic,
compound commands, functions, subshells, here-documents, and background jobs.
The shell's `help syntax`, `help export`, `help set`, and `help shift` explain the
current command language and builtins. When editing feature copy, check that
internal anchor links and release download URLs still resolve to the intended
sections and assets.
