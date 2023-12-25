---
slug: how-secure-is-your-environment-file-in-node-js
title: How secure is your environment file in Node.JS ?
datetime: 2017-10-07
original-link: https://codeburst.io/how-secure-is-your-environment-file-in-node-js-7c4d2ed0d15a
tags:
  - nodejs
  - javascript
  - security
  - npm
---
I bet [dotenv](https://www.npmjs.com/package/dotenv) is the easiest way out. You create a .env file and include this sing==le li==ne of code within your project :

`require(‘dotenv’).config()`

And BAM !! You are done and good to go. **But wait how secure is it ?**

Recently many fake Malicious NPM packages were found which work the same way as the real ones, but they fetch your process environment files and send them to a third-party server when you install them.

[Oscar B on X: "@kentcdodds Hi Kent, it looks like this npm package is stealing env variables on install, using your cross-env package as bait: https://t.co/REsRG8Exsx" / X (twitter.com)](https://twitter.com/o_cee/status/892306836199800836?ref_src=twsrc%5Etfw%7Ctwcamp%5Etweetembed%7Ctwterm%5E892306836199800836%7Ctwgr%5Eb88be3e532fb5a8210989a03ff890e728712c9d0%7Ctwcon%5Es1_&ref_url=https%3A%2F%2Fcdn.embedly.com%2Fwidgets%2Fmedia.html%3Ftype%3Dtext2Fhtmlkey%3Da19fcc184b9711e1b4764040d3dc5c07schema%3Dtwitterurl%3Dhttps3A%2F%2Ftwitter.com%2Fo_cee%2Fstatus%2F892306836199800836image%3Dhttps3A%2F%2Fi.embed.ly%2F1%2Fimage3Furl3Dhttps253A252F252Fpbs.twimg.com252Fmedia252FDGIcUNyXsAAY1Jf.jpg253Alarge26key3Da19fcc184b9711e1b4764040d3dc5c07)

This could be extremely dangerous as the your process environments could contain secret keys, tokens, DB strings and what not.

# Solution ?

## Try [secure-env](https://www.npmjs.com/package/secure-env)

The only problem here is that you write a few more lines of code.

```shell
# on your terminal/cmd
$ npm install -g secure-env
$ secure-env .env -s mySecretPassword

// in your node.js file
global.env =  require('secure-env')({secret:'mySecretPassword'});
```

This packages helps you generate a `env.enc`,which is then decrypted later in the code and can be assigned to any variable. The variable now contains the key value pair in the env file as an Object, which could be later used anywhere in your project. As you see, here we can decide where to assign the values in decrypted environment file and it doesn’t get assigned to`process.env`by default.

You may download and deep dive into other options that are available in [secure-env](https://www.npmjs.com/package/secure-env) to know more. Feel free to contribute to the [code](https://github.com/kunalpanchal/secure-env).

# Other solutions

- [What to do if am a user](https://iamakulov.com/notes/npm-malicious-packages/#what-to-do-if-im-a-user)?
- [What to do if am a library developer?](https://iamakulov.com/notes/npm-malicious-packages/#what-to-do-if-im-a-library-developer)