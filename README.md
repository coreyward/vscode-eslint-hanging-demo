# vscode-eslint-hanging-demo

This is a reproduction example of a VSCode “Code Helper (renderer)” process hanging at 100% CPU indefinitely.

## Reproduction steps:

1. Open the repo in VSCode with the ESLint plugin active
2. Run `yarn install`
3. Open the `highcharts-editor.complete.min.js` file

This should trigger the issue.

This was observed using the following:

VScode Version: 1.41.1
Commit: 26076a4de974ead31f97692a0d32f90d735645c0
Date: 2019-12-18T14:57:51.166Z
Electron: 6.1.5
Chrome: 76.0.3809.146
Node.js: 12.4.0
V8: 7.6.303.31-electron.0
OS: Darwin x64 19.2.0
ESLint Plugin: 2.0.15
