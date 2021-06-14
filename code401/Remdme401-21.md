# Components and Props

Component are  like JavaScript functions. They accept arbitrary inputs (called “props”) and return React elements describing what should appear on the screen.
Components let you split the UI into independent, reusable pieces, and think about each piece in isolation.

the component allows you to use ES6 class to define a component


# Rendering a Component

we can encountered React elements that represent DOM tags, and However, elements can also represent user-defined components.

When React sees an element representing a user-defined component, it passes JSX attributes and children to this component as a single object. We call this object “props”.


# Composing Components

Components can refer to other components in their output. This lets us use the same component abstraction for any level of detail. A button, a form, a dialog, a screen: in React apps, all those are commonly expressed as components.

