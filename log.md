- husky 执行错误
```js
[String: ''] {
  stdout: '',
  stderr: '[STARTED] Preparing...\n' +
    '[SUCCESS] Preparing...\n' +
    '[STARTED] Running tasks...\n' +
    '[STARTED] Running tasks for **/*\n' +
    '[STARTED] eslint . --fix --max-warnings 0\n' +
    '[FAILED] eslint . --fix --max-warnings 0 [FAILED]\n' +
    '[SUCCESS] Running tasks...\n' +
    '[STARTED] Applying modifications...\n' +
    '[SKIPPED] Skipped because of errors from tasks.\n' +
    '[STARTED] Reverting to original state because of errors...\n' +
    '[SUCCESS] Reverting to original state because of errors...\n' +
    '[STARTED] Cleaning up...\n' +
    '[SUCCESS] Cleaning up...\n' +
    '\n' +
    '✖ eslint . --fix --max-warnings 0:\n' +
    '\n' +
    '/Users/kynana/wbProject/github/git-auto-commit/package.json\n' +
    '  2:11  error  Parsing error: Unexpected token :\n' +
    '\n' +
    '✖ 1 problem (1 error, 0 warnings)\n' +
    '\n' +
    'husky - pre-commit hook exited with code 1 (error)\n',
  code: 1,
  cat: [Function: bound ],
  exec: [Function: bound ],
  grep: [Function: bound ],
  head: [Function: bound ],
  sed: [Function: bound ],
  sort: [Function: bound ],
  tail: [Function: bound ],
  to: [Function: bound ],
  toEnd: [Function: bound ],
  uniq: [Function: bound ]
} 
```
- husky 执行正确
```js
[String: '[dev/xxx/xx 0195bdf0e] feat: log\n' +
  ' 1 file changed, 1 insertion(+), 1 deletion(-)\n'] {
  stdout: '[dev/xxx/xx 0195bdf0e] feat: log\n' +
    ' 1 file changed, 1 insertion(+), 1 deletion(-)\n',
  stderr: 'husky > pre-commit (node v14.5.0)\n' +
    '[STARTED] Preparing...\n' +
    '[SUCCESS] Preparing...\n' +
    '[STARTED] Running tasks...\n' +
    '[STARTED] Running tasks for *{.js,ts,vue}\n' +
    '[STARTED] Running tasks for *{.scss}\n' +
    '[SKIPPED] No staged files match *{.scss}\n' +
    '[STARTED] eslint . --fix --max-warnings 0\n' +
    '[SUCCESS] eslint . --fix --max-warnings 0\n' +
    '[STARTED] stylelint --fix\n' +
    '[SUCCESS] stylelint --fix\n' +
    '[SUCCESS] Running tasks for *{.js,ts,vue}\n' +
    '[SUCCESS] Running tasks...\n' +
    '[STARTED] Applying modifications...\n' +
    '[SUCCESS] Applying modifications...\n' +
    '[STARTED] Cleaning up...\n' +
    '[SUCCESS] Cleaning up...\n' +
    'husky > commit-msg (node v14.5.0)\n',
  code: 0,
  cat: [Function: bound ],
  exec: [Function: bound ],
  grep: [Function: bound ],
  head: [Function: bound ],
  sed: [Function: bound ],
  sort: [Function: bound ],
  tail: [Function: bound ],
  to: [Function: bound ],
  toEnd: [Function: bound ],
  uniq: [Function: bound ]
} 
```