# MDX for Visual Studio Code

This extension adds language support for [MDX](https://github.com/mdx-js/mdx).

## What about `.md` files?

The extension automatically recognizes `.mdx` files. If MDX files in your project end with `.md` instead, you can tell VS Code to treat them as MDX by adding the following to your workspace settings:

```json
"files.associations": {
  "*.md": "mdx"
},
```
