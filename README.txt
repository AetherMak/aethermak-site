
# AetherMak Static Site — v1

This package is ready to deploy on Vercel (or any static host). It uses a **central, versioned CSS** at `/css/aethermak.v1.css`.
Generated: 2025-09-24 22:03:58 AST

## Structure
- `/index.html` — flagship homepage (Vision 2030 default + palette switcher)
- `/css/aethermak.v1.css` — central design system (three palettes + RTL)
- `/legal/privacy.html` — bilingual privacy policy
- `/legal/recording.html` — bilingual recording policy

## Deploy on Vercel
1. Create a new Vercel project → "Import Project" → drag & drop this zip (or push to Git).
2. Framework preset: **Other** (it's a static site).
3. Build command: **None**
4. Output directory: **/** (root)
5. After the first deploy, add your domain in Vercel:
   - Root: `aethermak.com`
   - Optional: add subdomain later `portal.aethermak.com` (for app/portal)

## DNS (at your domain registrar)
- For root `aethermak.com`: add A/ALIAS or use Vercel's recommended config in the dashboard.
- For subdomains (e.g., `portal.aethermak.com`): add **CNAME** → `cname.vercel-dns.com`.

## Notes
- Palette & language preferences are saved in localStorage.
- To update styles later, ship `/css/aethermak.v2.css` and update pages gradually.
- Legal footer links already point to `/legal/privacy.html` and `/legal/recording.html`.
