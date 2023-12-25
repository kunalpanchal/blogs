---
title: "Does any harm? #typescript"
slug: does-any-harm-typescript
datetime: 2019-02-28
original-link: https://codeburst.io/does-any-harm-typescript-c811ad3b00e8
ogImage: https://cdn-images-1.medium.com/max/1600/1*8E1vvTeneKKggEheo_1qtg.jpeg
tags:
  - typescript
  - web-development
description: Why not to use "any" anywhere?
---
> Why not to use “any” anywhere.

![](https://cdn-images-1.medium.com/max/1600/1*8E1vvTeneKKggEheo_1qtg.jpeg)

Photo by [Isaac Benhesed](https://unsplash.com/@isaacbenhesed?utm_source=medium&utm_medium=referral) on [Unsplash](https://unsplash.com?utm_source=medium&utm_medium=referral) edited by [Kunal Panchal](https://medium.com/u/7bad53f42af2)

[TypeScript](http://www.typescriptlang.org/) is a superset of JavaScript which primarily provides **optional** static typing, classes, and interfaces. Many of us JS maniacs love typescript as its strongly typed. The [State of Javascript survey](https://2018.stateofjs.com/javascript-flavors/overview/) states that more than 46% of users have _Used it, would use again_. Typescript is the 4th [Most Loved, Dreaded, and Wanted Languages](https://insights.stackoverflow.com/survey/2018/#technology-most-loved-dreaded-and-wanted-languages) according to StackOverflow surveys 2018. Those are really good numbers for a language which is just a wrapper for javascript which provides statically typed superpowers.

While that being said, many of us still end up misusing typescript by very frequently using the “any” keyword everywhere. If you do not turn on **noImplicitAny**, then any variable declarations will implicitly be of type any and this can be really bad. If you plan to use type “any**”** for any of your variables then, make sure it is well justified! Strongly typed languages usually do not offer such flexibility. How often do we come across a variable code declaration section such as this one, where we end up explicitly using any for simplicity:

```typescript
// app.component.ts
export class AppComponent {
  name = 'Angular';
  showBanner: any = false;
  items:any=[
    {
      title:'Game of Thrones',
      desc:'A Game for the throne',
      chars:['Jon snow','Aegon Targaryen']
    },
    {
      title:'White Collar',
      desc:'Neal, A con artist',
    }
  ]
}
```
Typescript class with “any” used for all the variables.

Typescript is no more strongly typed if you end up using **any** everywhere & anywhere. If you are really confused about types then leave this hectic task to the compiler as the compiler automatically deduces the type for you. If you want to explore the dynamically typed flexibility that javascript has to offer then using typescript doesn’t make much sense.

May it be function parameters or a very simple object, it is better if everything is strongly typed. If you are creating a library, it is always a good practice to create an interface for the object that your library would receive. This way you can make sure the end-user using your library gets all the errors fixed during the development phase and avoid facing issues during runtime. Declaring an interface in typescript is pretty straight forward:

```typescript
interface Item {  
   title: string;  
   desc: string;  
   chars?: string[];  
}
```

Use interfaces, use proper types for all the variables and avoid using any explicitly anywhere. Now your code should look something like this:

```typescript
// app.component.ts
interface Item {
  title: string;
  desc: string;
  chars?: string[];
}

export class AppComponent {
  private name: string = 'Angular';
  private showBanner: boolean = false;
  private items: Item[] = [
    {
      title: 'Game of Thrones',
      desc: 'A Game for the throne',
      chars: ['Jon snow', 'Aegon Targaryen']
    },
    {
      title: 'White Collar',
      desc: 'Neal, A con artist',
    }
  ]
}
```

f you are a lazy developer who ends up using **any** all the time then its a good idea to enable [TSLint](https://palantir.github.io/tslint/) and turn on the [no-any](https://palantir.github.io/tslint/rules/no-any/) rule, which would restrict you from using any explicitly. Believe me, using typescript with “any” everywhere does harm, better get used to using types in typescript.

Thanks for reading. I would love to hear your feedback, thoughts, and questions if you have any. Ping me on twitter [@kay_2695px](https://twitter.com/kay_2695px) and we could discuss this further.