# Typography

Typography system built with fluid scaling using clamp().

Viewport range:
min: 375px
max: 1440px

Scaling rules:
- headings scale aggressively
- body text remains stable
- interaction text prioritizes readability

---

## Headings

### H1
- **font-family:** Google Sans
- **font-weight:** 500
- **font-size:** `clamp(36px, 4.4vw, 64px)`
- **line-height:** `clamp(44px, 5vw, 72px)`
- **letter-spacing:** 0
- **paragraph-spacing:** 0

### H2
- **font-family:** Google Sans
- **font-weight:** 500
- **font-size:** `clamp(28px, 3.3vw, 48px)`
- **line-height:** `clamp(34px, 3.9vw, 56px)`
- **letter-spacing:** 0
- **paragraph-spacing:** 0

### H3
- **font-family:** Google Sans
- **font-weight:** 500
- **font-size:** `clamp(22px, 2vw, 28px)`
- **line-height:** `clamp(26px, 2.3vw, 32px)`
- **letter-spacing:** 0
- **paragraph-spacing:** 0

### H4
- **font-family:** Google Sans
- **font-weight:** 500
- **font-size:** `clamp(18px, 1.4vw, 20px)`
- **line-height:** `clamp(22px, 1.6vw, 24px)`
- **letter-spacing:** 0
- **paragraph-spacing:** 0

### H5
- **font-family:** Google Sans
- **font-weight:** 500
- **font-size:** `clamp(16px, 1.2vw, 16px)`
- **line-height:** `clamp(20px, 1.5vw, 24px)`
- **letter-spacing:** 0
- **paragraph-spacing:** 0

### H6
- **font-family:** Google Sans
- **font-weight:** 500
- **font-size:** `clamp(12px, 0.9vw, 12px)`
- **line-height:** `clamp(16px, 1.2vw, 20px)`
- **letter-spacing:** 0.03em
- **paragraph-spacing:** 0

---

## Text

### Text XL
- **font-family:** Google Sans
- **font-weight:** 700
- **font-size:** `clamp(22px, 1.9vw, 28px)`
- **line-height:** `clamp(34px, 3.3vw, 48px)`
- **letter-spacing:** 0
- **paragraph-spacing:** `clamp(12px, 1.5vw, 24px)`

### Text L
- **font-family:** Inter
- **font-weight:** 500
- **font-size:** `clamp(18px, 1.4vw, 20px)`
- **line-height:** `clamp(28px, 2.5vw, 36px)`
- **letter-spacing:** 0
- **paragraph-spacing:** `clamp(8px, 1vw, 16px)`

### Text M (Body)
- **font-family:** Inter
- **font-weight:** 400
- **font-size:** `clamp(16px, 1.2vw, 16px)`
- **line-height:** `clamp(22px, 1.7vw, 24px)`
- **letter-spacing:** 0
- **paragraph-spacing:** `clamp(6px, 0.75vw, 12px)`

### Text S
- **font-family:** Inter
- **font-weight:** 400
- **font-size:** `clamp(14px, 1vw, 14px)`
- **line-height:** `clamp(18px, 1.5vw, 22px)`
- **letter-spacing:** 0
- **paragraph-spacing:** `clamp(6px, 0.75vw, 12px)`

---

## Interactive elements

### Interaction XL
- **font-family:** Inter
- **font-weight:** 500
- **font-size:** `clamp(18px, 1.6vw, 22px)`
- **line-height:** `clamp(22px, 2vw, 28px)`
- **letter-spacing:** -0.01em
- **paragraph-spacing:** 0

### Interaction L
- **font-family:** Inter
- **font-weight:** 500
- **font-size:** `clamp(16px, 1.3vw, 18px)`
- **line-height:** `clamp(20px, 1.7vw, 24px)`
- **letter-spacing:** -0.01em
- **paragraph-spacing:** 0

### Interaction M
- **font-family:** Inter
- **font-weight:** 400
- **font-size:** `clamp(16px, 1.2vw, 16px)`
- **line-height:** `clamp(20px, 1.6vw, 22px)`
- **letter-spacing:** 0
- **paragraph-spacing:** 0

### Interaction S
- **font-family:** Inter
- **font-weight:** 400
- **font-size:** `clamp(14px, 1vw, 14px)`
- **line-height:** `clamp(18px, 1.4vw, 20px)`
- **letter-spacing:** 0
- **paragraph-spacing:** 0

---

## Spacing scale

Paragraph spacing between typography blocks (use `margin-bottom` or `gap`):

| Token        | Value                      | Use case               |
|--------------|----------------------------|------------------------|
| spacing-none | 0                          | Headings, interactions |
| spacing-s    | `clamp(6px, 0.75vw, 12px)` | Text M, Text S         |
| spacing-m    | `clamp(8px, 1vw, 16px)`    | Text L                 |
| spacing-l    | `clamp(12px, 1.5vw, 24px)` | Text XL                |

---

## CSS variables (optional)

For convenience, you can use CSS variables:

```css
:root {
  /* Font families */
  --font-heading: "Google Sans", sans-serif;
  --font-body: "Inter", sans-serif;

  /* Headings */
  --h1-font-family: var(--font-heading);
  --h1-font-weight: 500;
  --h1-font-size: clamp(36px, 4.4vw, 64px);
  --h1-line-height: clamp(44px, 5vw, 72px);
  --h1-letter-spacing: 0;
  --h1-paragraph-spacing: 0;
  
  --h2-font-family: var(--font-heading);
  --h2-font-weight: 500;
  --h2-font-size: clamp(28px, 3.3vw, 48px);
  --h2-line-height: clamp(34px, 3.9vw, 56px);
  --h2-letter-spacing: 0;
  --h2-paragraph-spacing: 0;
  
  --h3-font-family: var(--font-heading);
  --h3-font-weight: 500;
  --h3-font-size: clamp(22px, 2vw, 28px);
  --h3-line-height: clamp(26px, 2.3vw, 32px);
  --h3-letter-spacing: 0;
  --h3-paragraph-spacing: 0;
  
  --h4-font-family: var(--font-heading);
  --h4-font-weight: 500;
  --h4-font-size: clamp(18px, 1.4vw, 20px);
  --h4-line-height: clamp(22px, 1.6vw, 24px);
  --h4-letter-spacing: 0;
  --h4-paragraph-spacing: 0;
  
  --h5-font-family: var(--font-heading);
  --h5-font-weight: 500;
  --h5-font-size: clamp(16px, 1.2vw, 16px);
  --h5-line-height: clamp(20px, 1.5vw, 24px);
  --h5-letter-spacing: 0;
  --h5-paragraph-spacing: 0;
  
  --h6-font-family: var(--font-heading);
  --h6-font-weight: 500;
  --h6-font-size: clamp(12px, 0.9vw, 12px);
  --h6-line-height: clamp(16px, 1.2vw, 20px);
  --h6-letter-spacing: 0.03em;
  --h6-paragraph-spacing: 0;
  
  /* Text */
  --text-xl-font-family: var(--font-heading);
  --text-xl-font-weight: 700;
  --text-xl-font-size: clamp(22px, 1.9vw, 28px);
  --text-xl-line-height: clamp(34px, 3.3vw, 48px);
  --text-xl-letter-spacing: 0;
  --text-xl-paragraph-spacing: clamp(12px, 1.5vw, 24px);
  
  --text-l-font-family: var(--font-body);
  --text-l-font-weight: 500;
  --text-l-font-size: clamp(18px, 1.4vw, 20px);
  --text-l-line-height: clamp(28px, 2.5vw, 36px);
  --text-l-letter-spacing: 0;
  --text-l-paragraph-spacing: clamp(8px, 1vw, 16px);
  
  --text-m-font-family: var(--font-body);
  --text-m-font-weight: 400;
  --text-m-font-size: clamp(16px, 1.2vw, 16px);
  --text-m-line-height: clamp(22px, 1.7vw, 24px);
  --text-m-letter-spacing: 0;
  --text-m-paragraph-spacing: clamp(6px, 0.75vw, 12px);
  
  --text-s-font-family: var(--font-body);
  --text-s-font-weight: 400;
  --text-s-font-size: clamp(14px, 1vw, 14px);
  --text-s-line-height: clamp(18px, 1.5vw, 22px);
  --text-s-letter-spacing: 0;
  --text-s-paragraph-spacing: clamp(6px, 0.75vw, 12px);
  
  /* Interaction */
  --interaction-xl-font-family: var(--font-body);
  --interaction-xl-font-weight: 500;
  --interaction-xl-font-size: clamp(18px, 1.6vw, 22px);
  --interaction-xl-line-height: clamp(22px, 2vw, 28px);
  --interaction-xl-letter-spacing: -0.01em;
  --interaction-xl-paragraph-spacing: 0;
  
  --interaction-l-font-family: var(--font-body);
  --interaction-l-font-weight: 500;
  --interaction-l-font-size: clamp(16px, 1.3vw, 18px);
  --interaction-l-line-height: clamp(20px, 1.7vw, 24px);
  --interaction-l-letter-spacing: -0.01em;
  --interaction-l-paragraph-spacing: 0;
  
  --interaction-m-font-family: var(--font-body);
  --interaction-m-font-weight: 400;
  --interaction-m-font-size: clamp(16px, 1.2vw, 16px);
  --interaction-m-line-height: clamp(20px, 1.6vw, 22px);
  --interaction-m-letter-spacing: 0;
  --interaction-m-paragraph-spacing: 0;
  
  --interaction-s-font-family: var(--font-body);
  --interaction-s-font-weight: 400;
  --interaction-s-font-size: clamp(14px, 1vw, 14px);
  --interaction-s-line-height: clamp(18px, 1.4vw, 20px);
  --interaction-s-letter-spacing: 0;
  --interaction-s-paragraph-spacing: 0;

  /* Spacing scale */
  --spacing-none: 0;
  --spacing-s: clamp(6px, 0.75vw, 12px);
  --spacing-m: clamp(8px, 1vw, 16px);
  --spacing-l: clamp(12px, 1.5vw, 24px);
}
```

---

## Notes

- All sizes use `clamp()` for smooth responsive typography
- Minimum value — for small screens
- Middle value (vw) — for smooth scaling
- Maximum value — for large screens
- Use Text M as default paragraph style
