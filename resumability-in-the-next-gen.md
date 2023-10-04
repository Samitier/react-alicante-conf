# Resumability in the next generation frontend framework 

Speaker: Ruby Jane Cabagnot

## Introduction

Talking about the hydration step in SSR.

## What about Qwik

It does not need an hydration step. Page can be interactive without downloading and executing js in th client -> called resumability

## How?

Qwik serializes the closures & restores them in the FE.

## Demo

She demoed how Qwik works. You can see that it only downloads js when you press buttons or interact with the site and it only downloads what it needs to do the action.

## Rules

- Don't mix React components and Qwik components in the same file.

**Opinion**: interesting to check and build something with it.