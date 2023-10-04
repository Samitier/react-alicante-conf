# React the Good Parts

Speaker: Tejas 

## Demo 1

Criticism about the "bad" parts of React.

He started developing a counter app with vanilla js using browser apis `document.createElement`, `addEventListener` etc. 
Full of side effects hard to test.

Then he did the same thing with React so we could see the value proposition of react and what it brings: pure components, free of side effects.

## What criticism React has

- Performance: it is slow compared to the rest of frameworks. Virtual DOM is slow, React is not reactive.
- Server side react: you need a library to be able to use it in the backend.

## Demo 2 (signals)

Comparing the same code with a loop of 10k values with react and solidJS. The react one re-renders all the time there is a change in state. Solid, using `createSignal` does not. React is less performant because it re-renders 10k components.

UseMemo could solve this, but then you need to "think about it" to use it

## SSR

He did a demo of a "Dog list SPA" that fetches data from an API and renders a list. He talked about the dangers of doing a SPA because it cannot be crawled.

Then he tried to convert it to a SSR using a node server and `renderToString` method from react DOM. So SSR without an additional framework.
He managed to do it, but couldn't fetch the data.

He then talked about ServerComponents, that basically solve that issue.
Server components are async by default and they do not need a useEffect, they can just `const data = await fetch...` directly in the body of the component.

**Opinion**: not fully sure what was the point of his last demo. If he was trying to solve how "easy" you could do SSR with "vanilla" React, he ended up with a lot of spaghetti code when he could have just used a SSR framework.