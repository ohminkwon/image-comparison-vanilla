[![Netlify Status](https://api.netlify.com/api/v1/badges/8c51fb0a-cb29-4acb-9cfd-8c75dd74001f/deploy-status)](https://app.netlify.com/sites/image-comparison-vanilla-ohminkwon/deploys)

# image-comparison

![image-comparison](./images/examples/comparison-effect.gif)

π [DEMO](https://image-comparison-vanilla-ohminkwon.netlify.app/)

3D μν°μ€νΈ λ° νν¬λμ»¬ μν°μ€νΈλ₯Ό μν μ°μ΄λ λλ νμ€μ³ λ³κ²½μ λν κ²°κ³Όλ¬Ό μ°¨μ΄λ₯Ό λΉκ΅νκΈ° μν ν¬νΈν΄λ¦¬μ€ κΈ°λ₯ λ§λ€κΈ° μμ  μλλ€.

## Font Awesome

[`Font Awesome`](https://fontawesome.com/) μμ μ κ³΅νλ λ¨Έν°λ¦¬μΌ μμ΄μ½μ λ¬΄λ£λ‘ μ¬μ©ν  μ μμ΅λλ€.

```html
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta2/css/all.min.css">
```

λ€μκ³Ό κ°μ΄ μ¬μ©ν  μ μμ΅λλ€.

```html
<i class="fas fa-chevron-left"></i>
```

## tilt.js

[`vanilla-tilt.js`](https://micku7zu.github.io/vanilla-tilt.js/)μμ μ κ³΅νλ κΈ°μΈκΈ° μ λλ©μ΄μ ν¨κ³Ό λΌμ΄λΈλ¬λ¦¬ μλλ€. <br>
λ§μ°μ€ μμΉμ λ°λΌ κΈ°μΈκΈ° ν¨κ³Όλ₯Ό μ€λλ€.<br>


```js
VanillaTilt.init(document.querySelector("#image-comparison-slider"), {
  max: 5,
  speed: 800,
  scale: 1.02
})
```

μ΄μΈμλ μλμ κ°μ΄ λ€μν μ΅μμ ν΅ν΄ κ°λ, λ°©ν₯, μλ, ν¬κΈ°, μΆ, κ΄νλ±μ μΆκ°νμ¬ ννν  μ μμ΅λλ€.

```js
{
  reverse:                false,  // reverse the tilt direction
  max:                    35,     // max tilt rotation (degrees)
  startX:                 0,      // the starting tilt on the X axis, in degrees.
  startY:                 0,      // the starting tilt on the Y axis, in degrees.
  perspective:            1000,   // Transform perspective, the lower the more extreme the tilt gets.
  scale:                  1,      // 2 = 200%, 1.5 = 150%, etc..
  speed:                  300,    // Speed of the enter/exit transition
  transition:             true,   // Set a transition on enter/exit.
  axis:                   null,   // What axis should be disabled. Can be X or Y.
  reset:                  true,    // If the tilt effect has to be reset on exit.
  easing:                 "cubic-bezier(.03,.98,.52,.99)",    // Easing on enter/exit.
  glare:                  false,   // if it should have a "glare" effect
  "max-glare":            1,      // the maximum "glare" opacity (1 = 100%, 0.5 = 50%)
  "glare-prerender":      false,  // false = VanillaTilt creates the glare elements for you, otherwise
                                  // you need to add .js-tilt-glare>.js-tilt-glare-inner by yourself
  "mouse-event-element":  null,    // css-selector or link to HTML-element what will be listen mouse events
                                  // you need to add .js-tilt-glare>.js-tilt-glare-inner by yourself
  gyroscope:              true,    // Boolean to enable/disable device orientation detection,
  gyroscopeMinAngleX:     -45,     // This is the bottom limit of the device angle on X axis, meaning that a device rotated at this angle would tilt the element as if the mouse was on the left border of the element;
  gyroscopeMaxAngleX:     45,      // This is the top limit of the device angle on X axis, meaning that a device rotated at this angle would tilt the element as if the mouse was on the right border of the element;
  gyroscopeMinAngleY:     -45,     // This is the bottom limit of the device angle on Y axis, meaning that a device rotated at this angle would tilt the element as if the mouse was on the top border of the element;
  gyroscopeMaxAngleY:     45,      // This is the top limit of the device angle on Y axis, meaning that a device rotated at this angle would tilt the element as if the mouse was on the bottom border of the element;
}
```
## Responsive Web

λ°μν λΆκΈ°μ μ μ€μ νμ¬ νΉμ  ν΄μλ λ³νμ λ°λ₯Έ λΉμ¨μ λ³κ²½ ν©λλ€.

```css
@media (max-width: 768px) {
  :root{
    --image-comparison-slider-width: 90vw;
  }   
}
```


## Reference
- https://compressor.io/
- https://www.youtube.com/watch?v=bYh5X0fNYu0
- https://www.youtube.com/watch?v=2KMJxHW21cU