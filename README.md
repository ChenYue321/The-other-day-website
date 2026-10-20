**English** | [简体中文](README.zh-CN.md)

# The other day

Official website of the WeChat public account "the other day".

A website for saving my and my friends' practice works, and also to exercise my HTML-related skills.
Feel free to make any suggestions on programming since this is the first repo of mine and I had little experiences. And have no idea of any rules of the website

## Project structure

```
index.html          Home
basic_info.html     Basic information
members.html        Members
people/             Individual member pages
category/           Article categories (by year / by author)
style.css           Site-wide stylesheet
header_bg.jpg       Header background image
```

## Local preview

Opening the pages on your own machine, without going through GitHub or the deployed site.
Changes show up instantly, there is no wait for Pages to rebuild, and half-finished work never goes live.

Two ways:

**1. Open `index.html` directly**

The address bar will show `file:///...`. For a purely static site this is enough, and it looks almost identical to the live site.

**2. Run a local server**

```bash
python3 -m http.server 8000
```

Then visit <http://localhost:8000/>. Closer to the live environment, since it runs over `http://` rather than `file://`.
Once the site grows features that read local files, `file://` will be blocked by browser security policy and this becomes necessary.

The three kinds of address:

| Address | What it is |
|---|---|
| `file:///.../html/index.html` | A file on your disk, no network involved |
| `http://localhost:8000/` | A temporary server on your machine, visible only to you |
| `https://chenyue321.github.io/The-other-day-website/` | The live site, visible to everyone |

Workflow: preview locally → commit → push to `main` → wait for Pages to rebuild (about a minute) → live site updates.

## License

- **Written content**: CC BY-NC-SA 4.0, full text in [LICENSE](LICENSE).
  You may share and adapt it, but you must give appropriate credit, you may not use it for commercial purposes,
  and any adaptation must be distributed under the same license.
- **Code** (HTML / CSS): MIT, full text in [LICENSE-CODE](LICENSE-CODE).
  Take it and do whatever you like.

The header background image `header_bg.jpg` may be third-party material. Its copyright remains with its
original author and it is not covered by the licenses above.
