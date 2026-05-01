# NIS Prep Website — Changelog

## [1.3.1] - 2026-05-01

### Changed
- Phone and iPad frames switch to brand blue (#3D6EDB) in dark mode for better contrast
- Phone frame border thinned to 5px in dark mode
- iPad frame border set to 10px in dark mode
- Blue-tinted drop shadow on both frames in dark mode

## [1.3.0] - 2026-05-01

### Fixed
- Mobile horizontal overflow (blank stripe on right side of screen)
  - Added `overflow-x: hidden` to `html` element — iOS Safari requires it on the root, not just `body`
  - Phone duo sections now show a single phone at ≤600px (two 200px frames exceeded mobile viewport width)
  - iPad frame made responsive (`width: 100%`) to prevent overflow on small screens

## [1.2.0] - 2026-04-30

### Added
- `confirm.html` — email confirmation landing page, shown after user clicks verification link
- `reset-password.html` — password reset landing page; handles both PKCE (`?code=`) and implicit (`#access_token=`) flows, exchanges token via Supabase JS SDK, shows success state after password update

## [1.1.0] - 2026-04-30

### Changed
- Pricing section updated to show introductory 50% off with crossed-out $19.99 original price

## [1.0.0] - 2026-04-30
- Initial launch at coreexamlayups.com
- GitHub Pages deployment with custom domain
- HTTPS enabled via Cloudflare + GitHub Pages
- Privacy policy page live at coreexamlayups.com/privacy.html
