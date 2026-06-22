

# HTML Interview Questions and Answers

## 1. What is HTML?

**Answer:**
HTML (HyperText Markup Language) is the standard markup language used to create the structure of web pages. It defines elements such as headings, paragraphs, links, images, forms, and tables.

---

## 2. Difference Between HTML and HTML5?

**Answer:**

| HTML                       | HTML5                            |
| -------------------------- | -------------------------------- |
| Older version              | Latest version                   |
| Limited multimedia support | Built-in audio and video support |
| Fewer semantic tags        | Semantic tags available          |
| More plugin dependency     | Less plugin dependency           |

HTML5 introduced:

* `<audio>`
* `<video>`
* `<canvas>`
* Semantic tags

---

## 3. What Are Semantic Tags?

**Answer:**
Semantic tags clearly describe the meaning of the content they contain.

Examples:

* `<header>`
* `<nav>`
* `<main>`
* `<section>`
* `<article>`
* `<footer>`

**Benefits:**

* Better SEO
* Better accessibility
* Easier maintenance

---

## 4. Difference Between `div` and `span`?

**Answer:**

| div                       | span                      |
| ------------------------- | ------------------------- |
| Block element             | Inline element            |
| Takes full width          | Takes required width only |
| Used for sections/layouts | Used for small content    |

Example:

```html
<div>Hello</div>
<span>Hello</span>
```

---

## 5. Difference Between `id` and `class`?

**Answer:**

| id                   | class                      |
| -------------------- | -------------------------- |
| Unique               | Reusable                   |
| Used for one element | Used for multiple elements |
| Selected using `#`   | Selected using `.`         |

Example:

```html
<div id="header"></div>

<div class="box"></div>
<div class="box"></div>
```

---

## 6. What Are Block and Inline Elements?

### Block Elements

* Start on a new line
* Occupy full width

Examples:

```html
<div>
<p>
<h1>
<section>
```

### Inline Elements

* Do not start on a new line
* Occupy only required width

Examples:

```html
<span>
<a>
<strong>
```

---

## 7. What is the DOM?

**Answer:**
DOM (Document Object Model) is a tree-like representation of an HTML document. JavaScript uses the DOM to access and modify webpage content, structure, and styles.

Example:

```javascript
document.getElementById("title");
```

---

## 8. What Are Meta Tags?

**Answer:**
Meta tags provide information about a webpage to browsers and search engines.

Example:

```html
<meta charset="UTF-8">
<meta name="description" content="HTML Tutorial">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

**Uses:**

* SEO
* Responsive design
* Browser information

---

## 9. Difference Between localStorage, sessionStorage, and Cookies?

**Answer:**

| Feature        | localStorage  | sessionStorage   | Cookies    |
| -------------- | ------------- | ---------------- | ---------- |
| Size           | ~5MB          | ~5MB             | ~4KB       |
| Expiry         | Until deleted | Until tab closes | Can expire |
| Sent to Server | No            | No               | Yes        |

Example:

```javascript
localStorage.setItem("name", "John");
sessionStorage.setItem("name", "John");
```

---

## 10. What is SEO?

**Answer:**
SEO (Search Engine Optimization) is the process of improving a website's visibility in search engine results.

**SEO Techniques:**

* Semantic HTML
* Meta tags
* Proper heading structure
* Mobile-friendly design
* Fast loading website

Example:

```html
<title>Learn HTML</title>
<meta name="description" content="HTML Tutorial">
```

---

# Frequently Asked Coding Questions

## Create a Form

```html
<form>
  <label>Name:</label>
  <input type="text">

  <label>Email:</label>
  <input type="email">

  <label>Password:</label>
  <input type="password">

  <button type="submit">Submit</button>
</form>
```

---

## Create a Table

```html
<table border="1">
  <tr>
    <th>Name</th>
    <th>Age</th>
    <th>City</th>
  </tr>

  <tr>
    <td>John</td>
    <td>25</td>
    <td>New York</td>
  </tr>
</table>
```

---

# CSS Interview Preparation Guide

## Top 20 CSS Interview Questions

### 1. What is CSS?

**Answer:**
CSS (Cascading Style Sheets) is used to style and layout HTML elements on a webpage.

---

### 2. What are the Types of CSS?

**Answer:**

1. Inline CSS
2. Internal CSS
3. External CSS

Example:

```css
h1{
  color: blue;
}
```

---

### 3. What is the CSS Box Model?

**Answer:**

The Box Model consists of:

```text
Content → Padding → Border → Margin
```

* Content: Actual content of the element
* Padding: Space inside the border
* Border: Surrounds padding and content
* Margin: Space outside the border

---

### 4. Difference Between Margin and Padding?

| Margin                         | Padding                      |
| ------------------------------ | ---------------------------- |
| Outside the border             | Inside the border            |
| Creates space between elements | Creates space around content |

---

### 5. What is CSS Specificity?

**Answer:**
Specificity determines which CSS rule is applied when multiple rules target the same element.

Priority:

```text
Inline > ID > Class > Element
```

Example:

```css
#title{
  color:red;
}

.title{
  color:blue;
}

h1{
  color:green;
}
```

Result: Red

---

### 6. Difference Between id and class?

| id                   | class                      |
| -------------------- | -------------------------- |
| Unique               | Reusable                   |
| Used for one element | Used for multiple elements |
| Selected using #     | Selected using .           |

Example:

```html
<div id="header"></div>

<div class="box"></div>
<div class="box"></div>
```

---

### 7. Difference Between Block, Inline and Inline-Block Elements?

| Block             | Inline               | Inline-Block      |
| ----------------- | -------------------- | ----------------- |
| New line          | Same line            | Same line         |
| Full width        | Required width only  | Width respected   |
| Height/Width work | Height/Width ignored | Height/Width work |

---

### 8. Difference Between display:none and visibility:hidden?

### display:none

* Element removed from layout
* Takes no space

### visibility:hidden

* Element hidden
* Space remains reserved

---

### 9. Explain Positioning

#### Relative

```css
position: relative;
```

Moves relative to its original position.

#### Absolute

```css
position: absolute;
```

Moves relative to nearest positioned parent.

#### Fixed

```css
position: fixed;
```

Stays fixed on screen during scrolling.

#### Sticky

```css
position: sticky;
top: 0;
```

Acts relative until a scroll threshold is reached.

---

### 10. Difference Between Relative and Absolute?

| Relative                 | Absolute                              |
| ------------------------ | ------------------------------------- |
| Relative to itself       | Relative to nearest positioned parent |
| Remains in document flow | Removed from normal flow              |

---

### 11. What is z-index?

**Answer:**
Controls stacking order of elements.

```css
.box{
  z-index:10;
}
```

Higher value appears on top.

---

### 12. What is Flexbox?

**Answer:**
Flexbox is a one-dimensional layout system used to align and distribute items efficiently.

```css
.container{
  display:flex;
}
```

---

### 13. Difference Between justify-content and align-items?

### justify-content

Controls alignment along the main axis.

```css
justify-content:center;
```

### align-items

Controls alignment along the cross axis.

```css
align-items:center;
```

---

### 14. What is flex-direction?

**Answer:**
Determines the direction of flex items.

```css
flex-direction:row;
flex-direction:column;
```

---

### 15. What is flex-wrap?

**Answer:**
Allows items to move to the next line.

```css
flex-wrap:wrap;
```

---

### 16. How Do You Center a Div?

```css
.container{
  display:flex;
  justify-content:center;
  align-items:center;
  height:100vh;
}
```

---

### 17. Flexbox vs Grid?

| Flexbox         | Grid             |
| --------------- | ---------------- |
| One-dimensional | Two-dimensional  |
| Row OR Column   | Rows AND Columns |
| Simpler layouts | Complex layouts  |

---

### 18. What are Media Queries?

**Answer:**
Media queries apply styles based on screen size.

```css
@media(max-width:768px){
  body{
    font-size:14px;
  }
}
```

---

### 19. What is Responsive Design?

**Answer:**
Responsive design allows websites to adapt to different screen sizes and devices.

---

### 20. Difference Between em and rem?

### em

Relative to parent element.

### rem

Relative to root (`html`) element.

---

# Top CSS Coding Questions

## 1. Center a Div

```css
.container{
  display:flex;
  justify-content:center;
  align-items:center;
  height:100vh;
}
```

---

## 2. Create a Navbar

### HTML

```html
<nav>
  <a href="#">Home</a>
  <a href="#">About</a>
  <a href="#">Contact</a>
</nav>
```

### CSS

```css
nav{
  display:flex;
  gap:20px;
}
```

---

## 3. Two Column Layout

```css
.container{
  display:flex;
}

.left,
.right{
  flex:1;
}
```

---

## 4. Three Column Layout

```css
.container{
  display:grid;
  grid-template-columns:1fr 1fr 1fr;
}
```

---

## 5. Responsive Layout

```css
@media(max-width:768px){
  .container{
    flex-direction:column;
  }
}
```

---

## 6. Fixed Navbar

```css
nav{
  position:fixed;
  top:0;
  width:100%;
}
```

---

## 7. Card Hover Effect

```css
.card:hover{
  transform:scale(1.05);
}
```

---

## 8. Center Text Inside Div

```css
.box{
  display:flex;
  justify-content:center;
  align-items:center;
}
```

---

# CSS Interview Preparation Guide 🚀

## Top 20 CSS Interview Questions

### 1. What is CSS?

**Answer:**
CSS (Cascading Style Sheets) ka use HTML elements ko style karne aur webpage ka layout design karne ke liye hota hai.

---

### 2. What are the Types of CSS?

**Answer:**

1. Inline CSS
2. Internal CSS
3. External CSS

Example:

```css
h1{
  color: blue;
}
```

---

### 3. What is the CSS Box Model?

**Answer:**

Box Model 4 parts se milkar banta hai:

```text
Content → Padding → Border → Margin
```

- Content: Actual content
- Padding: Content aur border ke beech ki space
- Border: Content ko surround karta hai
- Margin: Element ke bahar ki space

---

### 4. Difference Between Margin and Padding?

| Margin | Padding |
|---------|---------|
| Border ke bahar ki space | Border ke andar ki space |
| Elements ke beech gap banata hai | Content ke around space deta hai |

---

### 5. What is CSS Specificity?

**Answer:**
Jab ek element par multiple CSS rules lagti hain, to specificity decide karti hai kaunsi rule apply hogi.

Priority:

```text
Inline > ID > Class > Element
```

Example:

```css
#title{
  color:red;
}

.title{
  color:blue;
}

h1{
  color:green;
}
```

Result: Red

---

### 6. Difference Between id and class?

| id | class |
|-----|--------|
| Unique hoti hai | Reuse kar sakte hain |
| Ek element ke liye | Multiple elements ke liye |
| # selector use hota hai | . selector use hota hai |

Example:

```html
<div id="header"></div>

<div class="box"></div>
<div class="box"></div>
```

---

### 7. Difference Between Block, Inline and Inline-Block Elements?

| Block | Inline | Inline-Block |
|---------|---------|--------------|
| New line se start hota hai | Same line me rehta hai | Same line me rehta hai |
| Full width leta hai | Sirf required width leta hai | Width respect karta hai |
| Height/Width work karte hain | Height/Width ignore hote hain | Height/Width work karte hain |

---

### 8. Difference Between display:none and visibility:hidden?

#### display:none

- Element page se remove ho jata hai
- Space nahi leta

#### visibility:hidden

- Element hidden hota hai
- Space reserve rehti hai

---

### 9. Explain Positioning

#### Relative

```css
position: relative;
```

Apni original position ke relative move karta hai.

#### Absolute

```css
position: absolute;
```

Nearest positioned parent ke relative move karta hai.

#### Fixed

```css
position: fixed;
```

Screen par fixed rehta hai.

#### Sticky

```css
position: sticky;
top: 0;
```

Scroll ke baad fixed jaisa behave karta hai.

---

### 10. Difference Between Relative and Absolute?

| Relative | Absolute |
|------------|------------|
| Apni position ke relative | Parent ke relative |
| Document flow me rehta hai | Flow se bahar ho jata hai |

---

### 11. What is z-index?

**Answer:**
Elements ki stacking order control karta hai.

```css
.box{
  z-index:10;
}
```

Jiska z-index zyada hoga wo upar dikhega.

---

### 12. What is Flexbox?

**Answer:**
Flexbox ek one-dimensional layout system hai jo items ko align aur distribute karne ke liye use hota hai.

```css
.container{
  display:flex;
}
```

---

### 13. Difference Between justify-content and align-items?

#### justify-content

Main axis par alignment control karta hai.

```css
justify-content:center;
```

#### align-items

Cross axis par alignment control karta hai.

```css
align-items:center;
```

---

### 14. What is flex-direction?

**Answer:**

```css
flex-direction:row;
flex-direction:column;
```

Items kis direction me arrange honge ye decide karta hai.

---

### 15. What is flex-wrap?

**Answer:**

```css
flex-wrap:wrap;
```

Items ko next line me move hone deta hai.

---

### 16. How Do You Center a Div?

```css
.container{
  display:flex;
  justify-content:center;
  align-items:center;
  height:100vh;
}
```

---

### 17. Flexbox vs Grid?

| Flexbox | Grid |
|----------|----------|
| One-dimensional | Two-dimensional |
| Row ya Column | Rows aur Columns |
| Simple layouts | Complex layouts |

---

### 18. What are Media Queries?

**Answer:**
Screen size ke hisab se CSS apply karne ke liye use hoti hain.

```css
@media(max-width:768px){
  body{
    font-size:14px;
  }
}
```

---

### 19. What is Responsive Design?

**Answer:**
Responsive Design aisi design hoti hai jo mobile, tablet aur desktop sab devices par properly adjust ho jaye.

---

### 20. Difference Between em and rem?

#### em

Parent element ke relative hota hai.

#### rem

Root (html) element ke relative hota hai.

---

# Top CSS Coding Questions

## 1. Center a Div

```css
.container{
  display:flex;
  justify-content:center;
  align-items:center;
  height:100vh;
}
```

---

## 2. Create a Navbar

### HTML

```html
<nav>
  <a href="#">Home</a>
  <a href="#">About</a>
  <a href="#">Contact</a>
</nav>
```

### CSS

```css
nav{
  display:flex;
  gap:20px;
}
```

---

## 3. Two Column Layout

```css
.container{
  display:flex;
}

.left,
.right{
  flex:1;
}
```

---

## 4. Three Column Layout

```css
.container{
  display:grid;
  grid-template-columns:1fr 1fr 1fr;
}
```

---

## 5. Responsive Layout

```css
@media(max-width:768px){
  .container{
    flex-direction:column;
  }
}
```

---

## 6. Fixed Navbar

```css
nav{
  position:fixed;
  top:0;
  width:100%;
}
```

---

## 7. Card Hover Effect

```css
.card:hover{
  transform:scale(1.05);
}
```

---

## 8. Center Text Inside Div

```css
.box{
  display:flex;
  justify-content:center;
  align-items:center;
}
```

---


---



---



