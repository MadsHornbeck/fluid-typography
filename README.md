# @hornbeck/react-carousel

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

## Usage

Import the stylesheet in your solution.

```js
import "@hornbeck/fluid-typography";
```

Change base configuation variables if needed:

```css
:root {
  /* Point where the smallest font size and scale should be used */
  --f-width-sm: 24; /* em */
  /* Point where the largest font size and scale should be used */
  --f-width-lg: 90; /* em */
  /* Minimum font size on the :root element, in rem */
  --f-font-sm: 1; /* rem */
  /* Maximum font size on the :root element, in rem */
  --f-font-lg: 1.5; /* rem */
  /* The modular scale used at the smallest point */
  --f-ratio-sm: 1.125;
  /* The modular scale used at the largest point */
  --f-ratio-lg: 1.25;
}
```

Set use the fluid sizes in your css:

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

## Documentation

- [Examples](https://codesandbox.io/s/hornbeck-fluid-typography-x2myd?file=/src/styles.css)
