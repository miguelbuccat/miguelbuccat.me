---
title: 'Bun is WORTH the hype!'
description: "Let's see why I think it deserves the hype"
date: 'March 27, 2023'
slug: 'bun-is-worth-the-hype'
excerptString: "Let's see why I think it deserves the hype"
---

Let's see why I think it deserves the hype
<!--more-->
<img src="/images/blog/dc4b461906b54a5c433a1ba16c78657537a9a272.png" alt="Bun Logo" width="200"/>

# What is Bun?
Bun, much like NodeJS is a JavaScript runtime, or so it's commonly explained as. It's much more feature packed than NodeJS, it's a full JavaScript/TypeScript toolkit. It's complete with a bundler, test-runner, and a NodeJS-compatible package manager. Basically a JavaScript runtime on steroids

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

As a developer, this is great, honestly, installing 0 packages rather than 2 packages (typescript and ts-node) is a better developer experience overall.