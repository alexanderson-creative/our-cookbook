# 🍳 Our Cookbook

A collaborative digital cookbook where friends and family can share their favorite recipes. Built with simple HTML & CSS, hosted free on GitHub Pages.

**Live Site:** `https://YOUR-USERNAME.github.io/our-cookbook/`

---

## 📁 Project Structure

```
our-cookbook/
├── index.html              ← Homepage (recipe grid)
├── styles.css              ← Shared styles (don't edit unless agreed!)
├── recipe-template.html    ← Copy this to make new recipes
├── images/                 ← Folder for recipe photos
│   └── (your-photo.jpg)
├── lemon-garlic-pasta.html ← Example recipe
├── chocolate-chip-cookies.html
├── smoothie-bowl.html
└── README.md               ← You are here!
```

---

## 🚀 How to Add Your Recipe

### Step 1: Get the Template
1. Go to the repository on GitHub
2. Click on `recipe-template.html`
3. Click the **Raw** button, then save the file (Ctrl+S / Cmd+S)
4. Rename it using the naming convention below

### Step 2: Name Your File
Use **lowercase letters with hyphens** (no spaces!):
- ✅ `grandmas-meatballs.html`
- ✅ `spicy-thai-curry.html`
- ❌ `Grandmas Meatballs.html`
- ❌ `spicy thai curry.html`

### Step 3: Edit the Template
Open the file in any text editor and fill in:
1. **Recipe title** (in `<title>` and `<h1>`)
2. **Your name** (in the author section)
3. **Category** (Breakfast, Lunch, Dinner, Dessert, Drinks, etc.)
4. **Times and servings**
5. **Ingredients** (one `<li>` per ingredient)
6. **Instructions** (one `<li>` per step)
7. **Chef's notes** (optional tips)

### Step 4: Add a Card to the Homepage
Open `index.html` and find the comment that says `ADD YOUR RECIPE CARD HERE`. Copy this template:

```html
<a href="your-recipe-name.html" class="recipe-card">
  <div class="recipe-card-image placeholder">🍽️</div>
  <div class="recipe-card-content">
    <span class="category-badge">Category</span>
    <h3>Your Recipe Title</h3>
    <p>A short, enticing description of your dish.</p>
    <div class="recipe-card-meta">
      <span>⏱️ XX min</span>
      <span>👤 By YourName</span>
    </div>
  </div>
</a>
```

**Important:** The `href="your-recipe-name.html"` must exactly match your recipe filename!

### Step 5: Upload to GitHub
1. Go to the repository on GitHub
2. Click **Add file** → **Upload files**
3. Drag and drop your new recipe file (and updated `index.html`)
4. Write a short commit message like "Add grandma's meatballs recipe"
5. Click **Commit changes**

---

## 📸 Adding Photos

Want to include a photo of your dish? Here's how:

1. **Prepare your image:**
   - Use JPG or PNG format
   - Resize to ~1200px wide (keeps the site fast)
   - Name it to match your recipe: `grandmas-meatballs.jpg`

2. **Upload to the images folder:**
   - In GitHub, navigate to the `images` folder
   - Click **Add file** → **Upload files**
   - Upload your image

3. **Add it to your recipe:**
   Find this section in your recipe file and uncomment it:
   ```html
   <div class="recipe-image-container">
     <img src="images/your-image.jpg" alt="Your Recipe Name" class="recipe-image">
   </div>
   ```

4. **Update the homepage card (optional):**
   Replace the emoji placeholder with your image:
   ```html
   <img src="images/your-image.jpg" alt="Recipe Name" class="recipe-card-image">
   ```

---

## 🎨 Style Guide

To keep the cookbook cohesive, please follow these guidelines:

| Element | How to Write It |
|---------|-----------------|
| Measurements | `1 cup`, `2 tablespoons`, `½ teaspoon` |
| Temperatures | `375°F (190°C)` - include both! |
| Times | `15-20 minutes` or `about 1 hour` |
| Instructions | Start with a **bold action verb** |

### Category Badges
Use one of these standard categories:
- `Breakfast`
- `Lunch`
- `Dinner`
- `Dessert`
- `Snack`
- `Drinks`
- `Pasta`
- `Soup`
- `Salad`
- `Vegetarian`

---

## 🌐 Viewing the Site Locally

Want to preview changes before uploading? Simply:
1. Download/clone the repository
2. Open `index.html` in any web browser
3. Click around to test your links!

---

## 🆘 Troubleshooting

### "My recipe isn't showing up"
- Check that the filename matches the link in `index.html` exactly
- Make sure there are no typos (capitalization matters!)
- Wait 1-2 minutes for GitHub Pages to update

### "The page looks broken"
- Make sure you have `<link rel="stylesheet" href="styles.css">` in the `<head>`
- Check that you didn't accidentally delete any closing tags (`</div>`, `</section>`, etc.)

### "My image isn't loading"
- Check the path: it should be `images/your-image.jpg`
- Make sure the filename matches exactly (including capitalization)
- Verify the image was uploaded to the `images` folder

---

## 👨‍👩‍👧‍👦 Contributors

- **Brian** - Lemon Garlic Pasta
- **Tasha** - *Add your recipe!*
- **Alex** - Berry Smoothie Bowl
- **Julia** - *Add your recipe!*
- **Madison** - Chocolate Chip Cookies
- **Caroline** - *Add your recipe!*

---

## 📜 License

This cookbook is for personal use by our friends and family. Share the love, not the repo! 🍝❤️

