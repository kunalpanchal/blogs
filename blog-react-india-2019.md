---
title: React India 2019 🏖
slug: react-india-2019
description: React India Conference 2019 at Goa summarized
ogImage: https://thepracticaldev.s3.amazonaws.com/i/g9coqiefdw7kj32k8gh4.jpeg
author: Kunal
featured: false
draft: false
datetime: 2019-10-02
tags:
  - GraphQL
  - React
  - conferences, 
  - javascript
---

React India 2019 was organized at Goa this time and it was a blast. Undoubtedly beach conferences are the best. What can go wrong when you have a private beach to hang out after all those fantastic talks? 


![Alt Text](https://thepracticaldev.s3.amazonaws.com/i/m74ljxxgucuee8hn013l.png)


So ask me what was the React conference about. Obviously React? **Nah!** 
It was more about GraphQL this time. Sure there were a few react talks too 😆. I will try to link a playlist for all of those talks along with this blog post as soon as they are available on youtube. This article is majorly about a few lovely talks that I really enjoyed and what are my learning outcomes. So let me summarize the 2-day conference in three important points.

## GraphQL everywhere

Many talks highlighted the rising need for a REST API alternative. GraphQL comes to the rescue. [Shruti Kapoor](https://twitter.com/shrutikapoor08) in her talk lays down the basics about GraphQL and how it can be rightly used within our applications. She explains how is it that we can use react hooks to ease the integration with React. 

After this [Nader Dabit](https://twitter.com/dabit3) talks about how developers are using GraphQL as an API gateway to accomplish things that you may have never thought possible. Quite elaborately he explains how we can use AWS Amplify to make a GraphQL without any hassle. I was really impressed by all of those live demos. 

[Eesh Tyagi](https://twitter.com/EtEesh) then explains how at Cleartrip they have used GraphQL to avoid the unnecessary over fetching of verbose data and manipulation on the client. He then presents a really small demo showing how they were able to reduce the document load time from over 3 seconds down to a few milliseconds by adding Redis caching at GraphQL server, and it was astonishing.

Many other developers like [Kiran Abburi](https://twitter.com/kiran_abburi), [Tanay Pratap](https://twitter.com/tanaypratap), [Shahidh K Muhammed](https://twitter.com/shahidh_k), and others in their talk, mentioned the importance of frontend developers having control over the data they need. It doesn't make much sense to accept the same data across all of the clients, as the need is quite different. Surely your play station doesn't need all of the data from the API that your phone requires or the other way around. Amazing tools like [Hasura](https://hasura.io/), [Crystallize](https://crystallize.com/) etc are made to ease the whole setup process. Whatsoever if you have no idea about what GraphQL is, then this is the right time to get started. You can begin with the well laid GraphQL documentation.

## Performance is of prior importance

Everybody says this and everybody knows this: Built a performant app, not something sluggish. It's about how deep can it get? 
`Date.now` in javascript gives you the precision of _1ms_. What if you need to build something which requires more precision. I didn't know there existed an API called [Performance](https://developer.mozilla.org/en-US/docs/Web/API/Performance) which could be used to achieve this. Many other such tiny tips and tricks by [Ritesh Kumar](https://twitter.com/ritz078) were really insightful. 

Ritesh in his talk tells about the bottlenecks he faced by building his open-source project Raaga. Later [Abinash Mohapatra](https://twitter.com/twistedfork88) explains how his team at Flipkart built a really sophisticated image uploader which is really performant. Both the speakers explain how you could leverage web workers to make the most out of it.

The cherry on the top was the talk by [Rajat Kumar](https://twitter.com/rajatkumar), an Engineer from Netflix. He explains how Netflix hacked Webpack for building a really good A/B testing solution. Internally they use AST to identify conditional dependencies in their dependency graphs and combined them to built a server-side JS+CSS bundler, and it's really fast.

IMHO Netflix has one of the most amazing engineering team out there. Stay updated to their [Netflix Technology Blog](https://medium.com/@NetflixTechBlog) for the latest articles.

## Open-source community culture 

There was a major emphasis on the whole open-source culture that we have. Though many companies leverage OSS as a source of brand equity and recruiting, among other advantages. Not all open-source projects are a success. There were many open-ended questions. How supportive, are we to new developers in the community? How seamless is the whole onboarding experience? etc.

[Carolyn Stransky](https://twitter.com/carolstran) gave one of the most relatable talks. She argues on the fact that we developers, once we are fluent with a framework/technology, we end up introducing it as "simple". While its simple for you now it might not be to a newcomer due to a steep learning curve or due to improper documentation. 


> "We mistake familiarity for simplicity - Carolyn Stransky"


[Jason Lengstorf](https://twitter.com/jlengstorf) explains how open source can also be intimidating to newcomers, and occasionally unwelcoming. He explains how GatsbyJS has managed to build a strong OSS community by following some really simple principles and by being supportive of all the contributions.

[Jani Eväkallio](https://twitter.com/jevakallio)'s talk was a wake-up call. Something that makes you question are we doing it all right? We do know React is eating the web. According to npm, 63% of JavaScript developers use React. But is it for the better? Something to ponder about.


---

# What Else you got?

Apart from all the scheduled tech talks, I had a chance to meet many amazing attendees and speakers out there. There were really good community talks happening parallelly. In fact, my friend [Mohit Karekar](https://mohitkarekar.com) had a chance to present one of the open-source projects he and I had been working on for a while now, [Shaai JS](https://shaaijs.tech). This is something you should check out if you are into blogging. Best of all I enjoyed the beaches at Goa and had a couple of beers with my friends. On the whole, it was a weekend well spent. As I said initially said:

> "It's a beach conference, what could go wrong?"


![React India family together. Yes, you can't find me in here.](https://thepracticaldev.s3.amazonaws.com/i/g9coqiefdw7kj32k8gh4.jpeg)


I couldn't cover all the talks too well here, they were all too good. Some amazing really well-known speakers such as [Sunil Pai](https://twitter.com/threepointone), [Siddharth Kshetrapal](https://twitter.com/siddharthkp) and [Ives van Hoorne](https://twitter.com/CompuIves) also gave their talks. Head over to twitter and follow [@react_india](https://twitter.com/react_india) for more updates. So after all of these amazing talks, how is it that you perfectly end a React conference? By announcing JSConf India.

---

Thanks for reading. I look forward to meeting many more of you JS Fanatics at other conferences. Look out for the [community page][react-conferences] on [reactjs.org] for more such conferences. Meanwhile, you can browse some of my other [articles][kunalpanchal-blog] or [projects][kunalpanchal-work] and come say Hi! on [twitter][twitter-my].


[kunalpanchal-work]: https://kunalpanchal.in/work
[kunalpanchal-blog]: http://blog.kunalpanchal.in
[twitter-my]: https://twitter.com/kay_2695px
[react-conferences]: https://reactjs.org/community/conferences.html
[reactjs.org]: https://reactjs.org
