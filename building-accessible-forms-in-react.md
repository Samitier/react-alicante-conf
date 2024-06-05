# Practical guide to building accessible forms in React

Speaker: Jateryna Porshnieva

## Introduction

What accessibility is and what is it for.

## Accessibility tricks

- Use mac voiceover or the accessibility tab in Chrome devtools to debug.
- label by default will be the content of an element or the label of an input.
- `focus-visible` css pseudo class for focus only via keyboard (not mouse focus).
- no aria is better than bad aria
- aria-labelledby to point to an element with the label
- aria-describedby to point to an element that describes it. Can accept multiple elements separated by comma.
- aria-hidden hides element from readers. For stuff that will make no sense to be read (example, the asterisk in required fields in forms).
- aria-required, for required form fields instead
- aria-invalid, for invalid form fields
- you should add icons next to text where color is important (for colorblind people). For example, "red" errors should go next to an error icon. Not enough just with the color.
- aria live regions. For when the content changes and we have to "focus" the reader in certain parts of the dom. Example: warnings, toasts, notifications, etc. Can be polite (won't interrupt) or assertive (will interrupt current sentence).
  - Role alert does assertive interrupt by default
  - Role status does polite interrupt by default
- use `eslint-jsx-ally` for additional help detecting accessibility issues on lint.
- lots of methods to test accessibility with "vanilla" react testing library (no plugins needed).

## Random TIL

- react has useId hook, which gives you a unique id for your elements (no need uuid)
- Resource for accessibility topics: a11ycasts on youtube

**Opinion**: one of the best talks of the conference. The density of information here was incredible and it made me realize how extremely simple accessibility is when you know how it works.

Found the talk on [youtube](https://www.youtube.com/watch?v=gxwJCF8dqh8).
