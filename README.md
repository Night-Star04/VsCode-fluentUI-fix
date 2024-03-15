# Used to fix Fluent UI issues and introduce some custom projects

## Repair parts

1. Fix terminal tabs cut off

   - [Repair Source](https://github.com/TheOld/vscode-fluent-ui/issues/56)
   - editor_chrome.css#L256 ~ 264

2. Fix search widget replacement input cut off

   - [Repair Source](https://github.com/TheOld/vscode-fluent-ui/pull/58)
   - editor_chrome.css#L1444 ~ 1446

3. Fix sidebar shifts the contents of the bar upwards

   - [Repair Source](https://github.com/TheOld/vscode-fluent-ui/pull/59)
   - editor_chrome.css#L1448 ~ 1451

## Custom projects

1. Adjust the transition fillet between the path column and the editor container
   - editor_chrome.css#L211
2. Adjust the tabs and path column white space between
   - editor_chrome.css#L253
3. Adjust the color overlap error of selected items in the sidebar
   - editor_chrome.css#L859

## How to use

1. Close Visual Studio Code.
2. Copy editor_chrome.css to extension css folder path and replace the original file. (See Remarks for the path of the css folder.)
3. Run Visual Studio Code as administrator.
   - Windows: Right-click on the Visual Studio Code shortcut and select `Run as administrator`.
   - MacOS: Open a terminal and run `sudo /Applications/Visual\ Studio\ Code.app/Contents/MacOS/Electron`.
   - Linux: Open a terminal and run `sudo /usr/share/code/code`.
   - Note: This is important, the extension won't work otherwise.
4. Run `> Fluent UI: Reload` from the command palette.

## Remarks

Fluent UI version: 3.9.0
Visual Studio Code version: 1.87.2
Visual Studio Code extension css folder path:

- Windows: `%USERPROFILE%\.vscode\extensions\leandro-rodrigues.fluent-ui-vscode-3.9.0\out\css\editor_chrome.css`
- MacOS: `~/.vscode/extensions/leandro-rodrigues.fluent-ui-vscode-3.9.0/out/css/editor_chrome.css`
- Linux: `~/.vscode/extensions/leandro-rodrigues.fluent-ui-vscode-3.9.0/out/css/editor_chrome.css`
