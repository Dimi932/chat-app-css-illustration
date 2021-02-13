# Front-end Style Guide

## Layout

The designs were created to the following widths:

- Mobile: 375px
- Desktop: 1440px

## Colors

### Primary

#### Text

- Pale Violet (sub-heading at the top of the app UI): hsl(276, 100%, 81%)
- Moderate Violet (chat on the left): hsl(276, 55%, 52%)
- Desaturated Dark Violet (chat on the right): hsl(271, 15%, 43%)
- Grayish Blue (placeholder text): hsl(206, 6%, 79%)
- Very Dark Desaturated Violet (main heading): hsl(271, 36%, 24%)
- Dark Grayish Violet (paragraph): hsl(270, 7%, 64%)

#### Gradients

These two colors are the vibrant background colors you see throughout the design and are applied as a linear gradient:

- Light Magenta: hsl(293, 100%, 63%)
- Light Violet: hsl(264, 100%, 61%)

### Secondary

- White: hsl(0, 0%, 100%)
- Light Grayish Violet (app background): hsl(270, 20%, 96%)
- Very Dark Desaturated Violet (submit button background): hsl(271, 36%, 24%)
- Very Light Magenta (radio button outline): hsl(289, 100%, 72%)

## Typography

### Body Copy

- Font size: 16px

### Font

- Family: [Rubik](https://fonts.google.com/specimen/Rubik)
- Weights: 400, 500, 700


:root {
/* ----- backround colrs -----*/
  --Light Magenta: hsl(293, 100%, 63%);
  --Light Violet: hsl(264, 100%, 61%);
/* ------Text colors ---------*/
--Pale Violet (sub-heading at the top of the app UI): hsl(276, 100%, 81%);
--Moderate Violet (chat on the left): hsl(276, 55%, 52%);
--Desaturated Dark Violet (chat on the right): hsl(271, 15%, 43%);
--Grayish Blue (placeholder text): hsl(206, 6%, 79%);
--Very Dark Desaturated Violet (main heading): hsl(271, 36%, 24%);
--Dark Grayish Violet (paragraph): hsl(270, 7%, 64%);

@media (max-width:1000px) {

.wrapper {
  display: grid;
  grid-template-rows: 800px 250px;
  grid-template-columns: 1fr 1fr;
  height: auto;
  padding: 0 16px;
}
.suspended-box {
  position: absolute;
  width:45vw;
}
.phone {
  grid-column: span 2;
  justify-self: center;
  align-self: center;
  margin: 0;
  z-index: 1;
}
.message {
  grid-column: span 2;
  width: auto;
  text-align: center;
  margin: 0;
  align-self: center;
}
.box {
  position: absolute;
  left:60vw;
  bottom: -182px;
  width:40vw;
  top: unset;
}
.attribution {
  left:auto;
  bottom: -160px;
}
}

@media (max-width:600px) {

.wrapper {
display: grid;
grid-template-areas:
"header phone footer"
"header message footer"
}
.wrapper {
grid-template-columns: none;
grid-template-rows: none;
}

.phone {
grid-area: phone;
margin-top: 110px;
align-self: unset;
}
.message {
grid-area: message;
margin: 800px 0 100px 0px;
}
.box {
left: 55%;
width: 45%;
bottom: -223px;
opacity: 0.3;
}

}
