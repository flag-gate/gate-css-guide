# Gate CSS Guide

> Beyond our style code, my friend

"Writing CSS is hard. Even if you know all the intricacies of position and float and overflow and z-index, it’s easy to end up with spaghetti code where you need inline styles, !important rules, unused cruft, and general confusion."

1. [Structure](#1-structure)
2. [Components](#2-components)
3. [Principles](#3-principles)
4. [Style](#4-style)

## 1. Structure

Our CSS structure is based in on three pillars in the following order:

### grid

Here comes all the styles related to the shape of the elements; Grid structure, size, height, width, padding and others.

Example:

```css

header{
  display: flex;
  justify-content: space-between;
  align-items: baseline;
}

.feelings > *{
  height: 6em;
  border-top: 1em solid #e5e5e5;
}

```

### palette

Related tonality and color of the elements.

Example:

```css

.logo{
    fill: currentColor;
}

.bar-chart{
    background-color: #f2f2f2;
}

```

### typography

Related to all typography. As font style; weight, size, shape, family and others.

```css

body{
  font-family: "gotham_rounded";
  font-size: 2vw;
  letter-spacing: 0.0025em;
  text-rendering: geometricPrecision;
}

p{
  font-weight: 100;
}

```

## 2. Components

To define yet.

## 3. Principles

Changes that have the same reason to happen must change together. In other words, do not repeat a definition of color, margin, others. If two elements always have the same color, this should be only defined in a CSS rule.

## 4. Style

Writing our CSS in a consistent way makes it more readable for everyone. Take this bit of CSS:

```css

.feelings{
  height: 100%;
  padding: 1em 0;
  box-sizing: padding-box;
}

```

It sticks to these style rules:

-   Use a new line for every selector and every declaration.
-   Add a single space between the property and value, for example `prop: value;` and not `prop:value;`.
-   No underscores or camelCase for selectors.

