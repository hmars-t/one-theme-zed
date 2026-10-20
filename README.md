# One Theme Zed

One Dark and One Light color themes for Visual Studio Code, ported from the default themes of the [Zed editor](https://zed.dev).

If you like the look of Zed's default themes and want the same palette in VS Code, this extension provides:

- **One Dark**
- **One Light**

Both themes cover the editor, workbench (sidebar, tabs, status bar, panels, menus, inputs), terminal ANSI colors, Git decorations, diff and merge colors, and syntax highlighting (TextMate scopes plus semantic tokens).

## Install

### From the Marketplace

Search for **One Theme Zed** in the Extensions view (`Ctrl+Shift+X`).

### From a `.vsix` file

```sh
code --install-extension one-theme-zed-0.1.1.vsix
```

Or use **Extensions: Install from VSIX...** from the Command Palette.

### Activate

Press `Ctrl+K Ctrl+T` (`Cmd+K Cmd+T` on macOS) and choose **One Dark** or **One Light**.

## Build from source

```sh
npm install -g @vscode/vsce
vsce package
```

This produces `one-theme-zed-<version>.vsix`.

## Publishing (maintainers)

Make sure the `publisher` field in `package.json` matches your publisher ID.

```sh
# Visual Studio Marketplace
vsce login <publisher-id>
vsce publish

# Open VSX (VSCodium, Cursor, and others)
npx ovsx publish -p <token>
```

## Notes and limitations

- Colors are taken directly from Zed's `one.json`, including alpha values.
- Zed uses tree-sitter categories and VS Code uses TextMate scopes, so the syntax mapping is an approximation. Individual languages may look slightly different from Zed.
- Some workbench elements have no Zed counterpart; for those I chose values that fit the palette.

Issues and pull requests are welcome.

## License and attribution

[MIT](LICENSE). The color values originate from the One Dark / One Light themes (MIT, Copyright (c) 2014 GitHub Inc.) as shipped in the Zed repository. See [NOTICE.md](NOTICE.md) for details.

This project is not affiliated with Zed Industries, GitHub, or Microsoft.
