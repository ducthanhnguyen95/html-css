# 🎨 Typography Guide

## 📚 Key Terms

| **Web Concepts**                 | **Font & Display** |
| -------------------------------- | ------------------ |
| `Browser cache`                  | `Retina display`   |
| `Query string parameters`        | `Sans-serif Fonts` |
| `Flash of invisible text (FOIT)` | `Serif Fonts`      |
| `Flash of unstyled text (FOUT)`  | `System fonts`     |
| `Font services`                  | `Monospace fonts`  |
| `Font stack`                     | `Web safe fonts`   |
| `Law of proximity`               | `Throttling`       |

---

## 📝 Summary

### 🌟 **Core Principles**

- **Typography** is the art of creating beautiful and readable text.
  > 💡 **95% of web content is text** → Ensure it’s visually appealing and legible across devices.

---

### 🖋️ **Font Categories**

| Type           | Characteristics            | Use Case                 |
| -------------- | -------------------------- | ------------------------ |
| **Serif**      | Stroke edges, professional | Formal documents         |
| **Sans-serif** | Clean, modern, friendly    | Web content, UI          |
| **Monospace**  | Equal-width characters     | Code displays, terminals |

🔔 **Pro Tip**: Avoid pure black (`#000`) for body text → Use dark grey instead.

---

### 🛠️ **Font Implementation**

- **`font-family`**: Use a **font stack** for fallbacks.  
  Example:
  ```css
  font-family: "Helvetica Neue", Arial, sans-serif;
  ```
