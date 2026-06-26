# 🚀 Setup Guide — Manav Agarwal GitHub Profile

## Step 1 · Create the profile repository

1. On GitHub, create a **new repository** named exactly: `manav-agarwal`
   (must match your GitHub username exactly)
2. Make it **Public**
3. Do **not** initialize with a README (you'll push this one)

---

## Step 2 · Push this repository

```bash
cd github-profile
git init
git add .
git commit -m "feat: initialize premium github profile"
git branch -M main
git remote add origin https://github.com/manav-agarwal/manav-agarwal.git
git push -u origin main
```

---

## Step 3 · Create required secrets

Go to **Settings → Secrets and variables → Actions** in your repo.

| Secret name | Value | Purpose |
|---|---|---|
| `METRICS_TOKEN` | GitHub Personal Access Token (PAT) with `read:user`, `repo`, `read:org` scopes | lowlighter/metrics |

### How to create a PAT:
1. GitHub → Settings → Developer Settings → Personal Access Tokens → Fine-grained tokens
2. Scopes needed: `repo` (full), `read:user`, `read:org`
3. Copy token → Add as `METRICS_TOKEN` secret

---

## Step 4 · Enable GitHub Actions

Go to **Settings → Actions → General** → Allow all actions → Save

---

## Step 5 · Run workflows manually (first time)

Go to **Actions** tab and run each workflow manually:

1. **🐍 Contribution Snake** — generates the snake animation
2. **📊 GitHub Metrics** — generates metric SVGs
3. **🔄 Daily Profile Refresh** — stamps timestamp

After first run, everything updates automatically on schedule.

---

## Step 6 · Personalise your links

Find and replace these placeholders in `README.md`:

| Placeholder | Replace with |
|---|---|
| `manav-agarwal` (username) | Your actual GitHub username |
| `manavagarwal@email.com` | Your real email |
| `linkedin.com/in/manav-agarwal` | Your LinkedIn URL |
| `leetcode.com/manav-agarwal` | Your LeetCode username |
| `codolio.com/profile/manav-agarwal` | Your Codolio profile |
| `codeforces.com/profile/manav-agarwal` | Your Codeforces handle |
| Springer paper links | Your actual paper DOIs |

---

## Step 7 · Update Springer paper links

In the Research section, replace the placeholder Springer links with your actual DOIs:

```
https://doi.org/10.1007/your-paper-doi-here
```

---

## Workflows at a glance

| File | Schedule | Purpose |
|---|---|---|
| `snake.yml` | Every 12h + push | Contribution snake animation |
| `metrics.yml` | Daily at 1 AM UTC | GitHub metric SVGs |
| `profile-update.yml` | Daily at 5:30 AM UTC | Refresh timestamp |
| `daily-refresh.yml` | Daily at midnight | Orchestrates all above |
| `readme-sync.yml` | On push to main | Validates README integrity |

---

## Optional customisation

**Change accent color:** Find `#6366f1` (indigo), `#8b5cf6` (violet), `#06b6d4` (cyan) throughout and replace with your preferred palette.

**Add Spotify Now Playing:**
```markdown
[![Spotify](https://spotify-github-profile.kittinanx.com/api/view?uid=YOUR_SPOTIFY_UID&cover_image=true&theme=novatorem&show_offline=false&background_color=0d1117&interchange=true&bar_color=6366f1&bar_color_cover=true)](https://spotify-github-profile.kittinanx.com/api/view?uid=YOUR_SPOTIFY_UID&redirect=true)
```

**Pin repositories:** Go to your GitHub profile and click "Customize your pins" to feature your best repos.

---

## Support

If this profile helped you — ⭐ the repo!
