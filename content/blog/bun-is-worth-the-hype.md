---
title: 'Bun is WORTH the hype!'
description: "Let's see why I think it deserves the hype"
date: 'March 28, 2023'
slug: 'bun-is-worth-the-hype'
excerptString: "Let's see why I think it deserves the hype"
---

Let's see why I think it deserves the hype
<!--more-->
<img src="/images/blog/dc4b461906b54a5c433a1ba16c78657537a9a272.png" alt="Bun Logo" width="200"/>

# What is Bun?
Bun, much like NodeJS is a JavaScript runtime, or so it's commonly explained as. It's much more feature packed than NodeJS, it's a full JavaScript/TypeScript toolkit. It's complete with a bundler, test-runner, and a npm-compatible package manager. Basically a JavaScript runtime on steroids

# Features

## (Almost) NodeJS Compatible
Most of the Node API is implemented in Bun, allowing most npm packages to work flawlessly.

![Vite running with Bun](/images/blog/60112455a78b764e99599a33199c183f02fe7321.png)

Above is an image showing Vite (vue template) running with Bun. This is good for many reasons, mainly because every Node project can quickly become a Bun project with barely any hiccups, allowing for faster adaptation... you know, unlike Deno (hihi)

## Out of the box TS support
Now, this is most what I love about Bun
```shell
bun foo.ts
```
Being able to run TypeScript out of the box is one of the biggest upsides for me. No ts-node usage in development and transpiling before production. To /paraphrase Bun's [documentation](https://bun.sh/docs/runtime/typescript#running-ts-files), Bun internally transpiles TS to JS, and that the additional overhead from directly executing TS files is negligible.

As a developer, this is great, honestly, installing 0 packages rather than 2 packages (typescript and ts-node) is a better developer experience overall. I want to write code as soon as everything setup, and making that setup easy and fast, that is what's important for developer experience.

## Speed
Ah yes, one of the main selling points of Bun. It's blazing fast.

![bun install benchmark](/images/blog/41f44af335cc3aea190bb0be43bd3946eb8229f5.png)

Above is a benchmark of npm-compatible package managers, and it shows ``bun install`` steaming ahead of all the other packagers. I've been hearing this since day 1 of Bun's public existence, it's kind of the magnum opus of the project. Like imagine having dependencies installed in a fraction of a second, that's unheard of. I've had times where I stared at npm installing dependencies for a whole minute, and honestly I'd choose ``bun install`` anyday.

In all fairness though, I haven't run the above benchmark myself, but here's the [GitHub repo](https://github.com/oven-sh/bun/tree/main/bench/install) to the benchmark the guys at Oven, the company behind Bun, used, so you can see for yourself. Honestly, in actual experience, I've found bun install is blazing fast, no need for numbers when I couldn't even blink before it finished installing dependencies

As for the runtime itself, I'm sure all of you reading this who's in the JavaScript community has seen a benchmark of how fast it is, so I don't think I have to be a broken record on this one.

## Even more features?
Honestly I'm too lazy to run down all the features of Bun. It is so feature-packed that I think we'll be here for all day, and it's 2am as of writing this, so I need to sleep. If you want to find out more, do visit [Bun.sh](https://bun.sh) for a full primer on Bun

# Is Bun a Node killer?
No. Node is definitely here to stay. Just like how PHP is still here, despite of its obvious inferiorities compared to other languages (don't come at me, I code PHP too). I think it's going to develop it's own community, but won't necessarily kill the NodeJS community. And as I said that Bun was largely Node-compatible is the primary reason it's easy to adapt into an existing project. I guess you can say it's piggybacking off the Node ecosystem as of right now, but that's not to say it won't form it's own ecosystem eventually. I guess I can link you to a [great video](https://www.youtube.com/watch?v=1xoy8Q5o8ws) that t3.gg did on this matter

# What do I think?
Personally, I think I'm gonna adapt Bun into my JS/TS projects from now on, I think it's pretty cool that it provides everything you commonly need, access to the abundant Node ecosystem, a bundler, and a blazing fast runtime. I've been following Bun's development on [Jarred Summer's twitter](https://twitter.com/jarredsumner) since the first day of Bun's public existence and it's been cool to see it grow and mature to the project it is today. It is defintely worth the hype around it, and I hope to see it grow more.