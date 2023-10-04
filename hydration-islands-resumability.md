# Hydration, Islands, Resumability, etc.

Speaker: Matheus Alburquerque

## Description

Brief history about webdev. How it all started: SSR first (PHP, Ruby, etc), SPA later (Js frameworks), then SSR but a client app, 

## Hydration

How do we build around this concept, how do we test it.
The "uncanny valley" people can see things, but they cannot interact with it until js is downloaded and evaluated.

## Islands architecture

Selectively, progressively enhance bits of SSR Html with js.
Scripts are delivered and hydrated independently.
There are parts of our app that do not need to be hydrated: for example text.

## Marko & Astro

Frameworks focused in islands architecture.
In Astro you can explicitly say if you want your components rendered, hydrated, etc.

## Resumability

Do some work, pause and resume in the browser. So clients do not redo work.
Qwik.

## Streaming SSR selective hydration

Some parts of the app hydrates faster.

## Server components

Server components never get served to the client. Attempt to bring the islands architecture to vanilla React.

**Opinion**: nice overview about how far we went regarding SSR in FE development. He shared lot of interesting links and condensed a lot of information here. Need to find the slides :(.