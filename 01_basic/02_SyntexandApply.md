
# ✅ CSS Syntax Structure
```css
p {
  color: red;
}
```


## Step-by-Step Breakdown

| What You See  | What It Is Called     | What It Means (Very Simple)          |
| ------------- | --------------------- | ------------------------------------ |
| `p`           | **Selector**          | Which element to style               |
| `{ }`         | **Declaration Block** | Area where styling rules are written |
| `color: red;` | **Declaration**       | One styling instruction              |
| `color`       | **Property**          | What you want to change              |
| `red`         | **Value**             | The result you want                  |

---


# ✅ 3 Ways to Apply CSS
## 1️⃣ Inline CSS

CSS written directly inside the HTML element using the `style` attribute.

Example:

```html
<p style="color: red;">Hello World</p>
```

🔹 Applied to only that specific element
🔹 Not reusable
🔹 Not recommended for large projects

Use case: Quick testing only.

---

# 2️⃣ Internal CSS

CSS written inside `<style>` tag in the `<head>` section of HTML.

Example:

```html
<!DOCTYPE html>
<html>
<head>
  <style>
    p {
      color: blue;
    }
  </style>
</head>
<body>

  <p>Hello World</p>

</body>
</html>
```

🔹 Works for that single HTML file
🔹 Better than inline
🔹 Still not good for big projects

---

# 3️⃣ External CSS ✅ (Best Method)

CSS written in a separate `.css` file.

Example:

### Step 1 → Create `style.css`

```css
p {
  color: green;
}
```

### Step 2 → Link in HTML

```html
<head>
  <link rel="stylesheet" href="style.css">
</head>
```

🔹 Most professional method
🔹 Reusable
🔹 Clean separation of HTML and CSS
🔹 Used in real projects & React apps

---


