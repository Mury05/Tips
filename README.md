# Tips
C'est un dépot pour mes tips
# Commandes pour la connexion via SSH

``bash
ssh-keygen -t ed25519 -C "email@mail.com"
``

``bash
ssh -T git@github.com
``

# Code pour la configuration de base d'un fichier vue dans les snippets de vscode

```js
{
// Place your snippets for vue here. Each snippet is defined under a snippet name and has a prefix, body and
// description. The prefix is what is used to trigger the snippet and the body will be expanded and inserted. Possible variables are:
// $1, $2 for tab stops, $0 for the final cursor position, and ${1:label}, ${2:another} for placeholders. Placeholders with the
// same ids are connected.
// Example:
// "Print to console": {
//  "prefix": "log",
//  "body": [
//      "console.log('$1');",
//      "$2"
//  ],
"description": {
    "prefix": "vvue",
    "body": [
      "<script setup>\n\n",
      "</script>\n\n",
      "<template>\n",
      "<div>\n",
      "$1\n",
      "</div>\n",
      "</template>\n\n",
      "<style scoped>\n\n",
      "</style>"
    ],
  }
}
```
