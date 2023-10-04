# Lightning talks

## tRPC better than REST/GRAPHQL

Speaker: Devlin Duldlulao

### Intro

Basically a tool to develop type-safe APIs in Typescript.

### Demo

He did a demo with NextJS with TRPc where he changed one of the parameters in the backend and the types were correctly inferred in the frontend code.

He also batched HTTP requests. He fetched multiple entities with a single HTTP request.

### Summary

https://trpc.io/

--------

## Common pitfalls in React Native

Speaker: Dan Neciu

### Intro

React native: does not wrap an app like Ionic, but compiles it to actual native code…

### Pitfalls:

1- Fonts: Roboto by default. Ypu can install new fonts with `expo install` and use them. But if you use a "normal" import to use it, it imports all the fonts of a package. This breaks apps very easily. You need to import a specific font.

2- Local storage: you can use the local storage while developing, but when using it in production it wont work. You need to use a package for that.
Also JSON.parse throws exception in production but not when using emulators/simulators.

3- Render text: you cannot use HTML elements (for example when fetching it from an API). You need to use a library.

4- Short circuit evaluations will crash the app if they are not boolean `{ foo && <Bar /> }` should be `{ Boolean(foo) && <Bar 7> }`.

### TLDR

Be careful about emulators. Always test on real phones.

--------

## Maximizing React Performance with Devtools: Profiler and Components

Speaker: Jelena Maravic

### Intro

She explained the React Devtools.

### Issues found with devtools

- Creating components inside other components. Component funcs should be declared outside
- Set incorrect values for initial state in stores
- Not moving state down the component tree to avoid unnecessary rerenders.
- Not using React.memo to memoize components.
- Wrapping a component in React.memo, but not its children. Memoization does not "cascade" down.
- Not memoizing provider values.

---------

## Codemods: how to ship without breaking changes

Speaker: Lukaz Nowak

### Intro

Explained what a feedback loop is when building software and how important it is for the loops to be as fast as possible,
Then he explained what negative impacts breaking changes have over the feedback loop. Users will not update to versions that have breaking changes.

### Automating the process

jscodeshift is a library that helps with that. A codemod is a piece of code that will change some code to fix breaking changes.

### Demo

He showed an example of a comdemod.

### Testing

Since codemods are functions with one input and one output. They can be easily unit tested.

----------

## Seek and you shall find your way to fun!

Speaker: Kevin Maes

### Introduction

He talked about Graph theory and mazes. A "traditional" 2d maze is just a graph set up in a matrix.

### Algotrithms and state charts

Any algorithm can be represented as a state chart to see a visual representation of it.

### Recursive backtracker

He explained an algorithm to navigate a graph. He then showed a maze generation tool he made with this recursive backtracker:
https://mazes.vercel.app

----------


