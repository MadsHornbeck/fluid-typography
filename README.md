# @hornbeck/fluid-typography

![npm](https://img.shields.io/npm/v/@hornbeck/fluid-typography)
![npm](https://img.shields.io/npm/l/@hornbeck/fluid-typography)
![npm](https://img.shields.io/npm/dw/@hornbeck/fluid-typography)
![npm bundle size](https://img.shields.io/bundlephobia/min/@hornbeck/fluid-typography)
![npm bundle size](https://img.shields.io/bundlephobia/minzip/@hornbeck/fluid-typography)

Simple configurable fluid typography and dynamic modular font scale in pure css.

## Install

```bash
npm install --save @hornbeck/fluid-typography
```

## Example

- [codesandbox](https://codesandbox.io/s/hornbeck-fluid-typography-x2myd?file=/src/styles.css)

## Usage

Import the stylesheet in your solution.

```js
import "@hornbeck/fluid-typography";
```

Change base configuation variables if needed:

```css
:root {
  /* Point where the smallest font size and scale should be used */
  --ft-width-min: 24; /* em */
  /* Point where the largest font size and scale should be used */
  --ft-width-max: 90; /* em */
  /* Minimum font size on the :root element, in rem */
  --ft-font-min: 1; /* rem */
  /* Maximum font size on the :root element, in rem */
  --ft-font-max: 1.5; /* rem */
  /* The modular scale used at the smallest point */
  --ft-ratio-min: 1.125;
  /* The modular scale used at the largest point */
  --ft-ratio-max: 1.25;
}
```

Use the fluid sizes in your css for e.g. your `font-size` or `margin`:

```css
p {
  font-size: var(--fluid-0);
}

h6 {
  font-size: var(--fluid-1);
}

h5 {
  font-size: var(--fluid-2);
}

h4 {
  font-size: var(--fluid-3);
}

h3 {
  font-size: var(--fluid-4);
}

h2 {
  font-size: var(--fluid-5);
}

h1 {
  font-size: var(--fluid-6);
}
```
