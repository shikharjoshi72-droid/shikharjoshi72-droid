# Shikhar Joshi — GitHub Profile README

## Files in this package

- `README.md` — complete profile README
- `.github/workflows/metrics.yml` — generates `profile/metrics.svg`
- `.github/workflows/snake.yml` — generates the animated contribution snake
- `profile/` — destination folder for generated SVG files

## Install into your profile repository

1. Open `https://github.com/shikharjoshi72-droid/shikharjoshi72-droid`.
2. Upload/replace `README.md` at the repository root.
3. Upload the two workflow files, preserving their exact paths:
   - `.github/workflows/metrics.yml`
   - `.github/workflows/snake.yml`
4. Keep the `profile` directory. The workflows write generated SVGs into it.
5. In repository Settings → Actions → General → Workflow permissions, enable **Read and write permissions**.
6. Open the Actions tab and manually run **Generate GitHub Metrics** and **Generate Contribution Snake**.
7. Wait for both runs to finish successfully, then refresh the profile.

## Important notes

- This package does not include generated statistics or snake SVGs; GitHub Actions creates them after installation.
- The workflows assume the default branch is named `main`. If your default branch has a different name, update `committer_branch` in `metrics.yml` and the branch used by the workflows as appropriate.
- Remove the older `.github/workflows/profile-widgets.yml` workflow to avoid duplicate jobs.
- External decorative images (header, typing animation, badges, skill icons and streak card) depend on their respective services being reachable.
