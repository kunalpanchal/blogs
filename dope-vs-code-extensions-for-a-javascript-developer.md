---
slug: dope-vs-code-extensions-for-a-javascript-developer
title: Dope VS Code extensions for a Javascript developer
original-link: https://medium.com/hackernoon/dope-vs-code-extensions-for-a-javascript-developer-7981625f4c4a
datetime: 2018-02-27
ogImage: https://miro.medium.com/v2/resize:fit:3200/1*JYiZDB5AfVAlVLdGmsQ3bg.jpeg
description: Dope VS Code extensions for a Javascript developer
tags:
  - vscode
  - javascript
  - extensions
---
# Dope VS Code extensions for a Javascript developer

According to [Octoverse](https://octoverse.github.com/) 2017, Microsoft’s Visual Studio Code tops the list of _Projects with the most contributors._ Which implies that there are a lot many developers who ==absofreakinlutely love VS Code==.  
Here I have a list of extensions which might not make you a better developer, but for sure would make you feel like one!

![](https://miro.medium.com/v2/resize:fit:3200/1*JYiZDB5AfVAlVLdGmsQ3bg.jpeg)

Image from [https://wallup.net/code-microsoft-visual-studio/](https://wallup.net/code-microsoft-visual-studio/)

A nifty little command would get me the list of VS code extensions I already have installed

```shell
$ code --list-extensionsalefragnani.project-manager  
aaron-bond.better-comments  
eamodio.gitlens  
eg2.vscode-npm-script  
formulahendry.code-runner  
jamespgilbert.comment-label  
schristian-kohler.npm-intellisense  
shardulm94.trailing-spaces  
steoates.autoimport  
streetsidesoftware.code-spell-checker  
whtouche.vscode-js-console-utils  
xabikos.JavaScriptSnippets
```


> A wise man once said : GIFs and JPEGs speak louder than words

## [**NPM Intellisense**](https://marketplace.visualstudio.com/items?itemName=christian-kohler.npm-intellisense)

![](https://miro.medium.com/v2/resize:fit:1400/1*7P4jVq5Vxd51noleeYtLAQ.gif)

## [Git Lens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)

![](https://miro.medium.com/v2/resize:fit:1400/1*DS2aWPI70ydDx4WHkkiJVQ.gif)

## [NPM Scripts](https://github.com/Microsoft/vscode-npm-scripts)

![](https://miro.medium.com/v2/resize:fit:1236/1*zlDVNeborUEB62hy92bOxg.png)

## [Code Runner](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner)

![](https://miro.medium.com/v2/resize:fit:1400/1*OAD4CzbkQz05eCqvy_XNsg.gif)

## [Trailing white spaces](https://marketplace.visualstudio.com/items?itemName=shardulm94.trailing-spaces)

```json
"editor.trimAutoWhitespace": true,  
"files.trimTrailingWhitespace": true,
```


![](https://miro.medium.com/v2/resize:fit:1400/1*EdoDRWiXYnIvrJCLc8uvBg.gif)

Image by [niichie](https://github.com/Niichie)

## [Auto import](https://marketplace.visualstudio.com/items?itemName=steoates.autoimport)

![](https://miro.medium.com/v2/resize:fit:1400/1*dCrNs4ZqjAB9af98ymep5g.gif)

## [Code spell checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker)

![](https://miro.medium.com/v2/resize:fit:1400/1*ncFQTNsT_rBVHce4NpdRMg.gif)

## [Console utils](https://marketplace.visualstudio.com/items?itemName=whtouche.vscode-js-console-utils)

![](https://miro.medium.com/v2/resize:fit:1400/1*U3t9Pm2e3qQGrg64GDPHnQ.gif)

## [Javascript Snippets](https://github.com/xabikos/vscode-javascript)

```javascript
imp→ import fs from 'fs';  
imn→ import 'animate.css'  
imd→ import {rename} from 'fs';  
ime→ import * as localAlias from 'fs';  
ima→ import { rename as localRename } from 'fs';  
enf→ export const log = (parameter) => {console.log(parameter);};  
edf→ export default (parameter) => { console.log(parameter);};  
ecl→ export default class Calculator { };  
ece→ export default class Calculator extends BaseClass { };```

## [Project manager](https://github.com/alefragnani/vscode-project-manager)

![](https://miro.medium.com/v2/resize:fit:1216/1*b3kP28bH9QqVysJnVxj2zg.png)

![](https://miro.medium.com/v2/resize:fit:1214/1*abI2uCz9S_MDGclfDfNbBQ.png)

## [Comment labels](https://marketplace.visualstudio.com/items?itemName=jamespgilbert.comment-labels)

![](https://miro.medium.com/v2/resize:fit:1400/1*5UwCD7DIGtvtSAX2qGkeZA.gif)

## [Better comments](https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments)

![](https://miro.medium.com/v2/resize:fit:918/1*dt0ryLQcGRBFXtYtNPnJeQ.png)

A few more, particularly for ng fans :

- [Angular v5 snippets](https://marketplace.visualstudio.com/items?itemName=johnpapa.Angular2)
- [Angular2 inline](https://marketplace.visualstudio.com/items?itemName=natewallace.angular2-inline)
- [Angular2 material](https://marketplace.visualstudio.com/items?itemName=hardikpthv.AngularMaterial)

Other worthy mentions which either couldn’t make it to the top 12s or were too obvious : [gitlink](https://marketplace.visualstudio.com/items?itemName=qezhu.gitlink), [esLint](https://github.com/Microsoft/vscode-eslint), [chrome-debug](https://github.com/Microsoft/vscode-chrome-debug), [yarn](https://marketplace.visualstudio.com/items?itemName=gamunu.vscode-yarn), [Bracket pair Colorizer](https://marketplace.visualstudio.com/items?itemName=CoenraadS.bracket-pair-colorizer).