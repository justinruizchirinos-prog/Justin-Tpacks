# Step-by-Step: Build Your Front Page

This guide will help you make a simple first page with an intro like:

**"Welcome to Justin Tpacks"**

You will create 3 files:
- `index.html`
- `style.css`
- `script.js`

---

## 1) Make a project folder
Create a folder called `justin-tpacks-site`.

Inside it, create:
- `index.html`
- `style.css`
- `script.js`

Open this folder in VS Code.

---

## 2) Add your HTML (`index.html`)
Copy this into `index.html`:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Justin Tpacks</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header class="site-header">
    <h1>Justin Tpacks</h1>
    <nav>
      <a href="#home">Home</a>
      <a href="#about">About</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <main>
    <section id="home" class="hero">
      <h2>Welcome to Justin Tpacks</h2>
      <p>This is my official website. Thanks for visiting!</p>
      <button id="helloBtn">Say Hello</button>
    </section>

    <section id="about" class="card">
      <h3>About Me</h3>
      <p>I’m building my website step by step and sharing my work.</p>
    </section>

    <section id="contact" class="card">
      <h3>Contact</h3>
      <p>Email: yourname@example.com</p>
    </section>
  </main>

  <footer>
    <p>© 2026 Justin Tpacks</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
```

---

## 3) Add your styling (`style.css`)
Copy this into `style.css`:

```css
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: #0f172a;
  color: #e2e8f0;
  line-height: 1.6;
}

.site-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 16px 24px;
  background: #1e293b;
  position: sticky;
  top: 0;
}

.site-header h1 {
  margin: 0;
  font-size: 1.2rem;
}

nav a {
  color: #e2e8f0;
  text-decoration: none;
  margin-left: 14px;
}

.hero {
  text-align: center;
  padding: 72px 20px;
  background: linear-gradient(135deg, #1d4ed8, #7c3aed);
}

.hero h2 {
  font-size: 2rem;
  margin-bottom: 12px;
}

button {
  margin-top: 14px;
  padding: 10px 18px;
  border: none;
  border-radius: 8px;
  cursor: pointer;
  font-weight: 600;
}

.card {
  background: #1e293b;
  margin: 20px;
  padding: 20px;
  border-radius: 12px;
}

footer {
  text-align: center;
  padding: 20px;
  opacity: 0.8;
}

@media (max-width: 700px) {
  .site-header {
    flex-direction: column;
    gap: 10px;
  }

  nav a {
    margin: 0 8px;
  }

  .hero h2 {
    font-size: 1.5rem;
  }
}
```

---

## 4) Add interactivity (`script.js`)
Copy this into `script.js`:

```javascript
const helloBtn = document.getElementById("helloBtn");

helloBtn.addEventListener("click", () => {
  alert("Welcome to Justin Tpacks!");
});
```

---

## 5) Run your website
- In VS Code, right-click `index.html`.
- Click **Open with Live Server** (install the Live Server extension first if needed).
- Your page should open in the browser.

---

## 6) First edits to personalize it
Change these right away:
- Update the intro sentence in the hero section.
- Replace `yourname@example.com` with your real contact.
- Change colors in `style.css` to your favorite theme.

---

## 7) Publish for free (GitHub Pages)
1. Create a GitHub repo named `justin-tpacks-site`.
2. Upload your 3 files.
3. In GitHub repo settings, open **Pages**.
4. Set source to `main` branch root.
5. Save, then open your live URL.

---

## 8) What to add next
After your front page works, add:
- A projects section with images.
- Social links (YouTube, Instagram, etc.).
- A custom domain later.

If you want, next I can generate a **Version 2 front page** with animations and a cleaner modern design.
