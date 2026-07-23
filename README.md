# Zelha Roster Report — TikTok influencer analysis

A static, multi-page report scoring Zelha Fitness's creator roster as
fitness-influencer contract candidates. Built from public TikTok metrics by the
AskSidney OS TikTok Content Analyser.

**Pages:** Overview & scorecard · Creator deep-dives · Content research ·
Reposts (proof-of-fit) · Method.

Self-contained: plain HTML + one CSS file, no build step, no JavaScript, no
external assets. Works from `file://` or any static host.

## Host it on GitHub Pages

1. Put this folder in a GitHub repo (either as the repo root, or under `/docs`).
2. Repo **Settings → Pages → Build and deployment**:
   - Source: **Deploy from a branch**
   - Branch: `main`, folder: `/ (root)` or `/docs` to match where you put it.
3. Save. The site publishes at `https://<user>.github.io/<repo>/` in ~1 minute.

`.nojekyll` is included so GitHub serves the files as-is.

Locally: open `index.html` directly, or run `python -m http.server` in this folder.

## Regenerate

The pages are generated from the analyser's exported data:

```bash
python build_site.py path/to/roster_data.json reports/zelha-roster-report
```

Data current as of the date shown in the report footer. Re-pull and rebuild to
refresh.
