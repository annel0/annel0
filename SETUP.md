# Setup

This directory is ready to be uploaded as the contents of the public GitHub profile repository:

`https://github.com/annel0/annel0`

## First upload

1. Create a **public** repository named exactly `annel0` under the `annel0` account.
2. Upload the **contents** of this folder to the repository root. Do not upload the outer `annel0-profile` directory itself.
3. Open the repository's **Actions** tab and allow workflows if GitHub asks.
4. Run **Refresh profile telemetry** once with `Run workflow`, or wait for the daily schedule.
5. The workflow will replace `assets/live.svg` with current GitHub metrics and keep it refreshed daily.

No Personal Access Token is required. The workflow uses the repository-scoped `GITHUB_TOKEN` supplied by GitHub Actions.

## Recommended profile settings

After the README appears on the profile page:

- Pin 4–6 repositories that best represent current work. `flybrain` is a strong candidate.
- Keep the GitHub bio short. Suggested text:
  `Marketing & AI · self-taught developer · systems, automation, networking & experiments`
- Avoid adding a large pile of external stats widgets. The included telemetry card is intentionally self-hosted.

## Customizing the hero

Edit:

- `assets/hero-dark.svg`
- `assets/hero-light.svg`

Both use only common system fonts, so no font files or extra assets are required.

## Removing dynamic telemetry

Delete:

- `.github/workflows/profile-card.yml`
- `scripts/update_profile_card.py`
- the `Profile telemetry` section in `README.md`

Everything else is static.
