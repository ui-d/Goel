<p align="center">
  <img src="https://raw.githubusercontent.com/michu1234/Goel/master/src/img/goel_background.jpg" width="100%" alt="Goel logo">
</p>

&nbsp; &nbsp;
<p align=center><img src="https://raw.githubusercontent.com/michu1234/Goel/master/src/img/mit.png"></p>
<p align="center"><img src="https://github.com/michu1234/Goel/blob/master/src/img/goel_logo.jpg?raw=true" width="50px" alt="Goel logo"> </p>
<h1 style="margin-top: -25px" align=center>GOEL </h1>
<h3 style="margin-top: -25px" align=center>Utility SASS Placeholders</h3>

<p align="center">GOEL is an SCSS library, which consists of multiple placeholders, build in utility/functional/atomic style.</p>

## Contents

- [Description](#description)
- [Highlights](#highlights)
- [Install](#intsall)
- [Placeholder](#placeholder)
- [Code comparison](#comparison)
- [Utility placeholder examples](#examples)
- [Usage](#usage)
- [Output](#output)
- [License](#license)


## Description

Goel is a sass placeholder library, allowing to marry functional and semantic approach in css. It will help you write clean, easy to read code, with DRY output.

## Highlights
&nbsp;
This approach comes with multiple benefits for front-end / ui developers.

- match semantic and functional CSS
- create developer-friendly class names using well-known methodologies like BEM, OOCSS
- use a functional approach to CSS
- use well-known architecture like ITCSS
- write clean CSS without unnecessary repetition
- write clean HTML without cluttering it with unnecessary classes
- stop wasting time to set up additional dependencies
- placeholders are not included in output = DRY code
- easy to set up and compose as you like
- easy to control how things look
- easy to extend (new placeholders, mixins, variables, etc.)
- clean and beautiful output, configure as you wish
- simple and minimal syntax


## Install

## PLACEHOLDER

> Sass has a special kind of selector known as a “placeholder”. It looks and acts a lot like a class selector, but **it starts with a % and it's not included in the CSS output**. In fact, any complex selector (the ones between the commas) that even contains a placeholder selector isn't included in the CSS, nor is any style rule whose selectors all contain placeholders,
<br />


```scss
// placeholders
%purple {
  color: purple;
}
%red {
 color: red;
}

p {
  @extend %purple;
}

span {
  @extend %purple;
}

h2 {
  @extend %purple;
}

h1 {
  @extend %purple;
}

```
<p style="font-size: 55px" align="center">👇</p>
&nbsp;&nbsp;

```scss
h1, h2, span, p {
  color: purple;
}

```

&nbsp;

&nbsp;

## Comparison
Lets

<p align="center"><img width="100%" src="https://raw.githubusercontent.com/michu1234/Goel/master/src/img/goel.png" alt="goel comparison" border="0"></p>

## Examples

###### 1 placeholder consists of 1 CSS declaration

```scss
%flex-row {
  flex-direction: row;
}
%flex-row-reverse {
  flex-direction: row-reverse;
}
%flex-col {
  flex-direction: column;
}
%visible {
  visibility: visible;
}
%invisible {
  visibility: hidden;
}

```

## Usage

```html
<div class="menu">

	<div class="menu__item menu__item--green"></div>
	<div class="menu__item menu__item--green"></div>

</div>

```

```scss
.menu {
  width: 500px;
  padding: 20px 40px 20px 40px;

  @extend %flex;
  @extend %flex-col;
  @extend %font-bold;
  @extend %text-center;
  @extend %bg-black;
  @extend %c-white;

  &__item {
    @extend %underline;
    @extend %flex;
  }

  &--green {
    @extend %c-green;
  }
}

```

&nbsp;
&nbsp;

## Output

```scss
.menu {
  @extend %flex;
}
.menu__block {
  @extend %flex;
}
.menu__wrapper {
@extend %flex;
}
.menu__list {
  @extend %flex;
}
.menu__list-item {
  @extend %flex;
}

```
<p style="font-size: 55px" align="center">👇</h>


```css
.menu, .menu__block, .menu__wrapper, .menu__list, .menu__list-item {
  display: flex;
}

```


## License

[MIT](https://github.com/wolfulus/zoya/blob/master/license.md)

