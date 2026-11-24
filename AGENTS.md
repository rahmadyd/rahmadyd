# AGENTS.md

This is a **GitHub profile repository** - not a code project. It contains only:
- `README.md` - Profile page with stats badges
- `.github/workflows/snake.yml` - Scheduled workflow generating snake animation SVGs to `output` branch

## Workflow
- Runs every 12 hours via cron (`0 */12 * * *`)
- Uses `Platane/snk@v3` to generate snake SVGs
- Deploys to `output` branch via `crazy-max/ghaction-github-pages@v3`

## No build/test/lint commands
This repo has no package.json, no source code, no tests, and no development workflow. The only automation is the snake workflow.