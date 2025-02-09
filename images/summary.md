# 📸 **Images Summary**

## 🗂️ **Categories of Images**

- **Raster Images** 🖼️

  - Made up of pixels
  - Common formats: **JPG, PNG, GIF**
  - Sources: Cameras, scanners, software
  - Used mainly for photos

- **Vector Images** ✏️
  - Defined by mathematical vectors (lines & curves)
  - Exported from tools like **Adobe Illustrator**
  - Format: **SVG** (Scalable Vector Graphics)

---

## 🖼️ **Displaying Images**

- **`<img>` Element** 📷
  - Displays content images (meaningful or decorative)
  - For decorative images: `alt=""` to avoid screen reader distractions

---

## 🎨 **Optimizing Images with CSS**

- **CSS Sprites** 🧩

  - Combine multiple images into one sprite
  - Reduces HTTP requests
  - Use [CSS Sprites Tool](https://cssspritestool.com)

- **Data URLs** 📄

  - Embed image data directly in HTML or CSS
  - Makes code larger and harder to maintain

- **Clipping** ✂️

  - Use `clip-path` in CSS
  - Tool: [Clippy](https://bennettfeely.com/clippy)

- **Filters** 🎛️
  - Apply effects: `grayscale`, `blur`, `saturate`, `brightness`, etc.

---

## 📱 **High-Density Screens & Resolution Switching**

- **High-Density Screens** 🖥️

  - Retina displays have more, smaller pixels
  - Use `srcset` with `2x` or `3x` images to maintain clarity

- **Resolution Switching** 🔄
  - Provide multiple image sizes for different devices
  - Tool: [Responsive Breakpoints](https://responsivebreakpoints.com)

```html
<img
  srcset="images/meal.jpg 1x, images/meal@2x.jpg 2x, images/meal@3x.jpg 3x"
  src="images/meal.jpg"
/>
```

---

## 🌐 **Modern Image Formats**

- **WebP Format** 🌍
  - Created by Google, supported widely (except IE)
  - Use `<picture>` with multiple sources

```html
<picture>
  <source type="image/webp" srcset="..." />
  <source type="image/jpeg" srcset="..." />
  <img src="..." alt="..." />
</picture>
```

- **Art Direction** 🎯
  - Show zoomed/cropped versions for specific viewports

```html
<picture>
  <source media="(max-width: 500px)" srcset="..." />
  <source media="(min-width: 501px)" srcset="..." />
  <img src="..." alt="..." />
</picture>
```

---

## 📊 **SVGs & Icon Fonts**

- **SVGs** 🖍️

  - Ideal for logos, icons, simple graphics
  - Scalable without losing quality
  - Resource: [SVG Backgrounds](https://svgbackgrounds.com)

- **Icon Fonts** 🔤
  - Popular libraries: **Font Awesome, Ionicons, Material Design Icons**

---

## 📝 **CSS Cheat Sheet**

### 🎨 **Background Images**

```css
background: url(../images/bg.jpg);
background-repeat: no-repeat;
background-position: 100px 100px;
background-size: cover;
background-attachment: fixed;
```

### ✂️ **Clipping**

```css
clip-path: polygon(50% 0%, ...);
```

### 🔍 **Filters**

```css
filter: grayscale(70%);
filter: blur(3px);
filter: brightness(0.5);
filter: contrast(200%);
filter: drop-shadow(10px 10px 10px grey);
filter: hue-rotate(90deg);
filter: invert(50%);
filter: saturate(25%);
filter: sepia(50%);
filter: opacity(50%);
filter: grayscale(70%) blur(3px);
```

---

✨ **End of Summary** ✨
