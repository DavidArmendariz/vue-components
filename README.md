# Vue components

I learned how to use inject and provide in Vue. In summary, what I learned here:

## Component Communication Overview

- Components are used to build UIs by combining them
- Components build **"parent-child"** relations and use **"unidirectional data flows"** for communication

## Props (parent => child)

- "Props" are used to pass data from a parent to a child component
- Props should be defined in advance, possibly in great detail (type, required, etc)

## Custom Events (child => parent)

- **"Custom Events"** are emmitted (via `$emit`) to trigger a method in a parent component
- Custom events can **carry data** which can be used in the called method

## Provide-inject

- If data needs to be passed accross multiple components ("pass-through"), you can use **provide/inject**.
- Provide data in a parent component, inject it into a child component
