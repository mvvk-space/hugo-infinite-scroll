---
title: "Glassmorphism and Modern aesthetics"
date: 2023-10-10T09:15:00-05:00
draft: false
---

You might have noticed the header of this site. It uses a technique called **Glassmorphism**. This is achieved using CSS backdrop-filter.

```css
header {
    background: rgba(255, 255, 255, 0.8);
    backdrop-filter: blur(12px);
}
```

It creates a sense of depth and context, allowing the content to gently slide behind the navigation while keeping the menu legible.

## Dark Mode Support

This theme also supports dark mode automatically based on your system preferences. The CSS variables handle the switch seamlessly.

*   **Backgrounds** become dark slate.
*   **Text** turns into a soft white/blocks.
*   **Accents** shift to be more luminous.

It's important to test your designs in both modes to ensure accessibility and visual hierarchy remain intact.

![Placeholder Image](https://picsum.photos/seed/picsum/800/400)

Images in this theme are given a subtle shadow and rounded corners to lift them off the page.
