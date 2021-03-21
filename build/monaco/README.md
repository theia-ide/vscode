# Steps to publish a new version of monaco-editor-core

## Generate monaco.d.ts

* The `monaco.d.ts` is now automatically generated when running `gulp watch`

## Bump version

* increase version in `build/monaco/package.json`

## Generate npm contents for monaco-editor-core

* Be sure to have all changes committed **and pushed to the remote**
* (the generated files contain the HEAD sha and that should be available on the remote)
* run gulp editor-distro

## Publish

* `cd out-monaco-editor-core`
* `npm publish`

## Disclaimer
Microsoft does not endorse, build, test or publish this extension, nor are they involved with it in any other way. The only association is that they own the copyright of these extensions and the rest of vscode's [source code](https://github.com/microsoft/vscode/tree/main/extensions), which they released under the [MIT License](https://github.com/microsoft/vscode/blob/main/LICENSE.txt). A copy of the license is included in this extension. See LICENSE-vscode.txt
    "Original VS Code sources are Copyright (c) 2015 - present Microsoft Corporation."

## What is this extension? Do I need it?
TL;DR: If you are running \`VS Code\`, \`Code OSS\` or derived product built from the VS Code repository, such as [VSCodium](https://github.com/VSCodium/vscodium), you do not need to install this extension since it's already present - "built-in".
Built-in extensions are built-along and included in \`VS Code\` and \`Code OSS\`. In consequence they may be expected to be present and used by other extensions. They are part of the [vscode GitHub repository](https://github.com/microsoft/vscode/tree/main/) and generally contribute basic functionality such as textmate grammars, used for syntax-highlighting, for some of the most popular programming languages. In some cases, more substantial features are contributed through built-in extensions (e.g. Typescript, Markdown, git, ...). Please see the description above to learn what this specific extension does.
