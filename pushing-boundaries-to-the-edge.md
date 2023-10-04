# Pushing boundaries to the edge

Speaker: Facundo Giulinai

## Introduction

Talks about the benefits about using CDNs when delivering code across the world.
His analogy: a brewery in ARgentina that brings the already brewed beer to Spain, instead of the users having to fly to Argentina to drink it.

## Static Site generation / Jamstack

Generating all the content on build time of a static website so that we can deliver all of it quickly.
But: it needs to be static content. Build times take long. Also if we need dynamic data, we still need to call services that might be allocated around the globe.

## edge computing

Executing server side logic in a distributed way. So not only delivering the static content as closest to the user, but generating that code too.
So a "dynamic" Jamstack.
Another analogy: Heineken also brews the beer in different countries, using the same formula. So they have a brewery as close as where the beer will be consumed.

## Edge and serverless is not exactly the same

Serverless is not happening in different regions of the world unless you explicitly specify it. Basically "the edge" is a mix of CDNs and distributed serverless.

## Advantages of the edge

Better performance, more security (did not specify why), real time insights and easy scalability.

## Some of their use cases

Personalization depending on the region, geolocation, easy AB testing, security (did not specify why).

## Frameworks that do edge computing in React

NextJS uses edge functions. Server side code that can be distributed as CDNs.
He demoed some Next code with some edge functions and middlewares.

**Opinion**: looks cool and some vendors support edge functions out of the box with zero config. For example: Netlify, Cloudflare and Vercel. Can be a cool way to distribute software without having to spend tons of money on devops. Other frameworks do this too, for instance Nuxt (vue). It is not something exclusive for React and definitely interesting to have on the radar for our hobby projects.