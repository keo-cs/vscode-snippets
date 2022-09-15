
# code-snippets

Each snippet is defined under a snippet name and contains the following fields:

* `scope`: comma-separated ids of languages for which the snippet should be available.
  * If `scope` is left empty or omitted entirely, the snippet will be applied to all languages.
* `prefix`: keyword(s) used to select snippet from the shortcut menu (default: `Ctrl` + `Space`)
* `body`: snippet content (i.e. what is expanded when the snippet is inserted).
* `description`: self-explanatory...

* * *

## Example

```json
{
  "Print to console": {
    "scope": "javascript,typescript",
    "prefix": "log",
    "body": [
      "console.log('$1');",
      "$2"
    ],
    "description": "Log output to console"
  }
}
```

* * *

### *Optional* variables

|||
|-|-|
|Tab stops|`$1`, `$2`, `$3`, `etc.`|
|Placeholders*|`${1:A}`, `${2:X}`, `${3:any}`, `etc.`|
|Final cursor position|`$0`|
\* *Placeholders are linked by* `id`. *Entering text in one field will propagate across all other linked placeholders*

* * *

### How to install

#### Windows

* Option 1 (**Recommended**): Clone this repo
  * `git clone https://github.com/kevinolson-cs/vscode-snippets C:\Users\<username>\AppData\Roaming\Code\User\snippets`

* Option 2: Download repository source
  * [Download repo source archive from GitHub](https://github.com/kevinolson-cs/vscode-snippets/archive/refs/heads/main.zip)
  * Extract all `.code-snippets` files to `C:\Users\<username>\AppData\Roaming\Code\User\snippets`

* * *

### Note for colleagues

Please take heed of... heed... heed of... take head of this repository's `.gitignore`; the redacted content of the excluded file is below:

```json
{
  "Escalation reply request": {
    "scope": "markdown",
    "prefix": "reply-request",
    "body": [
    ],
    "description": ""
  },
  "Escalation reply reminder": {
    "scope": "markdown",
    "prefix": "reply-reminder",
    "body": [
    ],
    "description": ""
  },
}
```

* * *
