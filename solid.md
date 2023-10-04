# Solid

Speaker: Erik Rasmussen

## Into

The started describing what imperative programming is. So telling the computer specifically what you want to do (vanilla js)
Then he talked about declarative programming, the paradigm react uses.
Then he talked about reactive programming: so reacting to changes in data/state. What solid uses (and vue)

## Signals

He talked about Solid's `createSignal`, a way of using reactive programming in react.
The syntax is exactly the same as `useState`, but returning a getter function instead of a value.
the JSX will execute that getter on render, creating a reactive JSX that updates when the signal does.

## How Solid works

React executes the whole component on rerender. Solid only once on init. 
Everything has to be a signal (even props) or else they will execute only once.

## Other Solid benefits

Things like `useEffect` (`createEffect` in solid) do not need dependencies because, since everything is a signal, dependencies can be automatically calculated.
`useMemo` is `createMemo`, also no dependencies.
Other "goodies" like `<Show>` component instead of ternaries. `<For>` component to iterate (no need for keys).
It has `directives` (kinda like angular).

**Opinion**: solid is the "well designed" React. It has been built from scratch to solve all the issues React accumulated over years. It looks A LOT like Vue. It's basically Vue with JSX instead of a separated template. Pretty cool, but its too soon to see what will happen with it.
