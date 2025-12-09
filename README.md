# Vencord Themes

A collection of CSS themes for Vencord (Discord client modification) to change the look and feel of your client.

This repository contains stylesheet files (.css) intended to be loaded by Vencord's theme system. Each file is a standalone theme or a variant. If you're here to preview, install, or contribute themes — welcome!

---

## Table of contents

- What this repo is
- Quick install (user)
- Developer / contributor guide
- File structure & naming
- Compatibility & notes
- Screenshots / previews
- License
- Contact / support

---

## What this repo is

This repository hosts CSS theme files that I like to use.
---

## Quick install (for users)

1. Open Vencord settings in your Discord client.
2. Find the "Themes" section and click "Open Themes Folder" (or open the themes directory used by your Vencord install).
3. Copy the `.css` files from this repository into that folder.
4. Back in Vencord, enable the theme(s) you copied. You may need to reload Discord (Ctrl/Cmd+R) to see changes.

If your Vencord installation uses a different theme loader/plugin, follow that loader's instructions to add or import a new CSS theme. If you're unsure where the themes folder is, check Vencord's documentation or the Vencord settings UI.

---

## Developer & contributor guide

- Want to add a theme?
  - Create a new branch.
  - Add a single `.css` file (or a small folder with a README and assets if needed).
  - Follow the naming conventions below.
  - Submit a PR with screenshots and a short description of the theme.

- Local testing:
  - Copy the theme into your Vencord themes folder and enable it.
  - Use Discord's reload (Ctrl/Cmd+R) and developer tools (Ctrl/Cmd+Shift+I) to inspect and tweak styles.
  - Keep selectors specific and avoid breaking core UI functionality.

- Assets:
  - If a theme needs images or fonts, include them in an `assets/` subfolder and document the usage in a small README next to the theme. Prefer data URIs or hosted CDNs only if allowed by licensing.

---

## File structure & naming

Recommended repository layout:

- themes/
  - my-theme.css
  - my-theme/          (optional folder for complex themes)
    - theme.css
    - assets/
    - README.md
- README.md
- CONTRIBUTING.md
- LICENSE

Naming guidance:
- Use concise, descriptive names (kebab-case preferred), e.g. `midnight-ocean.css`.
- If you publish variants, append `-compact`, `-large-text`, etc.

Include a small header comment at the top of each CSS file with:
- Theme name
- Author
- Version / last updated
- Compatibility notes (if applicable)

Example:
/* Theme: Midnight Ocean
   Author: Jane Doe
   Version: 1.0.0
   Compatible with: Vencord vX.Y+, Discord stable as of 2025-XX
*/

---

## Compatibility & notes

- Themes are dependent on Vencord's theme loader and the structure of Discord's DOM. Updates to Vencord or Discord may break styles; please report compatibility issues in an Issue with reproducible steps.
- Avoid using !important unless necessary — prefer specific selectors to minimize conflicts.
- Be mindful of accessibility: ensure adequate contrast for text and interactive elements.

---

## Screenshots / previews

Please include at least one screenshot (PNG/JPG) named to match the theme (e.g. `midnight-ocean.png`) next to the theme file or in a `previews/` folder. A short caption in the PR or theme folder README is very helpful.

---

## Contributing

Contributions are welcome. Please follow these steps:
1. Fork the repo.
2. Create a branch: `feature/my-theme`.
3. Add your theme files and a short README/screenshot.
4. Open a Pull Request with a description and compatibility notes.

Please keep commits tidy and include meaningful commit messages.

---

## License

This repository does not include a license file yet. If you want permissive reuse, consider adding an OSI-approved license such as MIT or CC BY-SA for themes. If you would like, add a LICENSE file or open an issue to discuss licensing preferences.

---

## Reporting issues / requesting features

Use the repository's Issues to report broken themes, compatibility problems, or to request theme ideas. When filing an issue, please include:
- Theme file name (or link)
- Vencord version and Discord platform (stable / Canary / PTB)
- Steps to reproduce
- Screenshot or console errors if applicable

---

## Credits

Thanks to all contributors and theme designers. If you publish a theme derived from someone else’s work, include attribution in the theme header and theme README.

---

## Contact

If you want me to help add this README to the repository or create a CONTRIBUTING.md or LICENSE file, tell me and I can draft or push the files for you.
