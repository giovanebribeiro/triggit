# triggit
If a file changes on git repo, do something

This package is a node port from [this](https://gist.github.com/sindresorhus/7996717) script (Thanks
Sindre!)

So, basically this script check the git's diff tree and, if specified file changes, execute a command.

The recommended usage for this package is with another great one, called 
[Husky](https://www.npmjs.com/package/husky):

```json
// on package.json
{
  "husky": {
    "post-merge": "triggit \"file_to_check.js\" \"command -to run\""
  }
}
```
