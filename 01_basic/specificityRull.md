# CSS Specificity Rull (Highest → Lowest)

```
!important
Inline (1000)
ID (100)
Class (10)
Element (1)
Universal (0)
Same specificity → Bottom rule wins
```

---

## Short Explanation Table

| Priority | Type            | Value   | Simple Meaning                              |
| -------- | --------------- | ------- | ------------------------------------------- |
| 1     | `!important`    | Special | Forces rule to win                          |
| 2        | Inline          | 1000    | Written inside HTML `style=""`              |
| 3        | ID              | 100     | `#id` selector                              |
| 4        | Class           | 10      | `.class`, `:hover`, `[type]`                |
| 5        | Element         | 1       | `p`, `div`, `h1`                            |
| 6        | Universal       | 0       | `*` selector                                |
| ⚡ Rule   | Normal CSS Flow | —       | If specificity same → **last written wins** |

---

### One Line Memory Trick

```
!important > Inline > ID > Class > Element > *
If equal → Down wins 👇
```

---

###  Example (Top to Bottom Rule)

```css
p { color: blue; }
p { color: red; }
```

Specificity same (1 vs 1)

👉 **Red wins** (because written later)

---

### Example (Specificity Rule)

```css
p { color: blue; }        /* 1 */
.text { color: red; }     /* 10 */
#main { color: green; }   /* 100 */
```

👉 `#main` wins (highest specificity)



### Example (`!important` Rule)

```css
#main { color: green; }
p { color: blue !important; }
```

👉 `!important` wins

---

