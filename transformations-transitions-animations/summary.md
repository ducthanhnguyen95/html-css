# Animations Cheat Sheet

## Summary

- **Transformations:**  
  Using the `transform` property, we can apply one or more transformations to an element.

- **Common Transformation Functions:**  
  The most common transformation functions are:

  - `rotate()`
  - `skew()`
  - `translate()`
  - `scale()`

- **Transitions:**  
  The `transition` property is used to animate one or more properties.

- **Custom Animations:**  
  To create a custom animation, first, we need to define the keyframes. Each keyframe includes the list of styles to be applied at a given moment in time. Once we define the keyframes, we can use the `animation` property to animate an element.

---

## CSS Cheat Sheet

### Transformations

```css
transform: rotate(15deg);
transform: rotate(-15deg);
transform: scale(1.3);
transform: skew(15deg);
transform: translate(10px, 20px);
transform: translateX(10px);
transform: translateY(20px);
transform: rotate(15deg) scale(1.3);
```

### Transitions

```css
transition: transform 0.5s;
transition: transform 0.5s ease-out;
transition: transform 0.5s ease-out 1s; /* 1s delay */
transition: transform 0.5s, color 0.3s;
```

### Animations

```css
@keyframes pop {
  0% {
    transform: scale(1);
  }
  50% {
    transform: scale(1.5);
  }
  75% {
    transform: rotate(45deg);
    background: tomato;
  }
  100% {
    transform: rotate(0);
  }
}
.box {
  animation: pop 3s ease-out;
}
```
