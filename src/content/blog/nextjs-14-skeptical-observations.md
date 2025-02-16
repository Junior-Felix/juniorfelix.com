---
title: "Next.js 14: Skeptical Observations"
description: "In this article, I discuss my concerns with the release of NextJs 14."
pubDatetime: 2023-11-26T21:00:00.000Z
ogImage: "/assets/images/next-js-14-preview.jpg"
featured: false
slug: nextjs-14-skeptical-observations
tags: ["reflections"]
---

A few releases ago, I'd wholeheartedly recommend Next.js to both friends and foes whenever a React frameworks discussion arose. With this latest release, my enthusiasm has waned. Next.js has taken a more "futuristic" persona, moving at a blazingly fast pace, and it feels like a significant portion of its community is being left behind. In this article, I will narrow my focus on [the release of Next.js 14](https://nextjs.org/blog/next-14), and my concerns related to it.

![test](/assets/images/mark-jackson-what.jpg)

## Table of contents

## Next.js 14 Release Notes

The cliff notes from this release are:

- No new APIs.
- Performance improvements for [Turbopack](https://turbo.build/pack).
- Server Actions are stable now.
- Partial Prerendering can be previewed now.

💡 The official release blog post provides a more in-depth explanation. Click <a target="_blank" rel="noopener noreferrer nofollow" href="https://nextjs.org/blog/next-14">here </a>to read, but kindly come back! I'm not done yet.

## My Concerns with this Release

### The Canary vs. Production Conundrum

With certain decisions, Next.js blurs the line between experimental and stable features. Some of these decisions include:

- **Turbopack's premature promotion**: It is concerning that despite Turbopack not passing all the tests for both App router and Pages router, it is prominently featured in the official release notes as a significant improvement. Moreover, these margins of improvement are boldly highlighted despite its unstable nature. It is worth noting that Turbopack is not the default bundler when running the `next dev` command, further contributing to this ambiguity.
- **Server actions confusion**: Recently, the React team shared a post on X announcing the availability of server actions in React Canary, as shown [here](https://twitter.com/reactjs/status/1716573234160967762). From the replies, you can tell that the developer community is confused if server actions are a feature of Next.js or React. Additionally, the presence of server actions in React Canary implies their instability within React, even though they may be considered stable in the context of Next.js. The lingering ambiguity adds to the complexity of the situation.

![](/assets/images/canary-stable.jpg)

### Reevaluating the Major Release Label

Despite Next.js 14 being a major release, it lacks the substantial changes that are typically associated with major releases. The nature of the updates included in this release is more aligned with what I'd expect from a minor release. It's worth noting that Next.js has a relatively high frequency of version releases, especially when we consider that version 1 was initially released in October 2016.

### Introducing Partial Prerendering

The Next.js 14's accompanying blog post acknowledges the complexities introduced in prior releases. However, in the next paragraph, Next.js 14 introduces partial prerendering, which adds further complexity. While it does not introduce new APIs, it is probably a new concept to many which does not make it any easier digest. Additionally, the release does not provide a lot of details on it; and promises to do so in a future minor update.

## Conclusion

Contrary to the skepticism I've expressed in this article, I'm still bullish on Next.js. I recognize their willingness to push the React community forward, but at the same time, I'm not sure if this is the way to get us there. Maybe, this is similar to the pushback React faced when it was first introduced to the JavaScript community. However, I am no wizard with a pondering orb to make those conclusions.
