

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

# Top 5 Most Asked HTML Interview Questions

1. Difference between HTML and HTML5?
2. What are semantic tags?
3. Difference between id and class?
4. What is DOM?
5. Difference between localStorage, sessionStorage, and Cookies?
