# SCSS Function Rem

Package for integrating `SCSS Function Rem` in a web environment.

![npm](https://img.shields.io/npm/v/@bu0nq/scss-function-rem?style=for-the-badge)
![npm](https://img.shields.io/npm/dt/@bu0nq/scss-function-rem?style=for-the-badge)
___

## Installation

This package can be deployed automatically using NPM:

```
npm i @bu0nq/scss-function-rem
```

## Usage

Import in your project depending on your setup:

```scss
@use "@bu0nq/scss-function-rem" as *;

.demo {
    font-size: rem(16px);
}
```

## Namespace

You can change the namespace during import and use the rem function with a different namespace:

```scss
@use "@bu0nq/scss-function-rem" as to;

.demo {
    font-size: to.rem(16px);
}
```

## Changing baseline

By default, `function-rem` uses a base size of 16 pixels, but you can change this value using the `$baseline` command and using the baseline parameter to adjust the size of the main font.

```scss
@use "@bu0nq/scss-function-rem" as * with (
  $baseline: 10
);

.demo {
    font-size: rem(16px);
}
```

Execution result:

```css
.demo {
    font-size: 1.6rem;
}
```
