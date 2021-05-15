# performant-shoes
- What I learned:
  - Creating an overlay on top of an image with pseudo-element, opacity, and background-url.
```css
header .content {
  background: var(--orange);
  width: 100%;
  color: var(--black);
  position: relative;
  text-align: center;
  font-weight: var(--emphasis-weight);
}

header .content:before {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  opacity: 0.3;
  background-image: url("src/shoes.jpg");
  background-size: cover;
  background-position: 100%;
}
``` 
  - Without a z-index value, any non-static positioned elements will be on top of the default static positioning elements.
    - [Element's z-index by position property value](https://css-tricks.com/almanac/properties/z/z-index/#:~:text=The%20z-index%20property%20in%20CSS%20controls%20the%20vertical,a%20position%20value%20other%20than%20static%20%28the%20default%29.)
```css
- header .content * {
  position: relative;
}
```
  - Reviewed pseudo-selectors and pseudo-classes such as :active, :focus, and ::before.

## Mobile:
![image](https://user-images.githubusercontent.com/18124536/118374788-ee6af280-b58b-11eb-8e48-016ffa634bf0.png)
## Tablet:
![image](https://user-images.githubusercontent.com/18124536/118374839-03e01c80-b58c-11eb-93f0-c7adeb983543.png)
## Desktop:
![image](https://user-images.githubusercontent.com/18124536/118374912-5d484b80-b58c-11eb-9418-b3addb1c3c25.png)
