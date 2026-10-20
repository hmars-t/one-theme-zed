# Third-party notice and attribution

The color values in this extension are derived from the **One Dark** and **One Light** themes that ship with the [Zed editor](https://github.com/zed-industries/zed), specifically `assets/themes/one/one.json`.

## License of the source material

The directory `assets/themes/one/` in the Zed repository contains its own `LICENSE` file: the **MIT License, Copyright (c) 2014 GitHub Inc.** The same entries are listed for "One Dark" and "One Light" in `assets/themes/LICENSES` in that repository, pointing to the Atom `one-dark-ui` / `one-light-ui` packages.

This is separate from the license of the rest of the Zed repository, which is licensed primarily under GPL-3.0-or-later with Apache-2.0 components where marked. No Zed source code is included in this extension, only theme color values from the MIT-licensed theme directory.

The license text is reproduced in [LICENSE](LICENSE), together with the copyright line for this port.

## What was changed

- Zed's theme schema was mapped to the VS Code theme format (workbench `colors`, TextMate `tokenColors` and `semanticTokenColors`).
- Zed syntax categories (for example `keyword`, `function`, `property`) were mapped to matching TextMate scopes. This mapping is an approximation.
- UI colors were mapped to the closest VS Code workbench keys. A few derived values (for example hover and active button shades) were chosen by hand.

Source snapshot: `zed-industries/zed`, commit `1d8a29e1e2f65b6be6c176f90af801286ac11cc4` (2026-10-20).

## Trademarks

This project is not affiliated with, endorsed by, or sponsored by Zed Industries, Inc., GitHub, Inc., or Microsoft. "Zed", "Atom", and "GitHub" are trademarks of their respective owners.
