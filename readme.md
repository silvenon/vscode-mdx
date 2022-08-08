# MDX for Visual Studio Code (deprecated)

_**Note**: This extension has been deprecated in favor of the [official MDX extension](https://marketplace.visualstudio.com/items?itemName=unifiedjs.vscode-mdx)._

---

Adds language support for [MDX](https://github.com/mdx-js/mdx).

## Installation

You can install this extension from the [Marketplace](https://marketplace.visualstudio.com/items?itemName=silvenon.mdx).

## What about `.md` files?

By default the MDX language is applied only to `.mdx` files. If MDX files in your project end with `.md`, you can tell VS Code that by adding the following to your workspace settings:

```json
"files.associations": {
  "*.md": "mdx"
},
```

Note that once you do that, any settings associated to `[markdown]` will stop applying to `.md` files. For example, if you had something like this in your settings:

```json
"[markdown]": {
    "editor.wordWrap": "wordWrapColumn",
    "editor.wordWrapColumn": 100
},
```

You probably want to replace it by this: 
```json
"[mdx]": {
    "editor.wordWrap": "wordWrapColumn",
    "editor.wordWrapColumn": 100
},
```

## Auto-close tags

If you want VS Code to automatically close tags while you type, you can install [Auto Close Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-close-tag) and configure it to also include the language `mdx`:

```json
"auto-close-tag.activationOnLanguage": [
  "xml",
  "php",
  "...",
  "mdx"
]
```

