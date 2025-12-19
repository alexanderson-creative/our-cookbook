# 🍳 Our Cookbook

A collaborative digital cookbook where friends and family can share their favorite recipes. Built with simple HTML & CSS, hosted free on GitHub Pages.

**Live Site:** `https://brianokarski-shopify.github.io/our-cookbook/`

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

## 🖥️ Getting Started with Cursor

Everyone on the team needs to do this **one time** to get set up.

### Step 1: Clone the Repository

1. Open **Cursor**
2. Press `Cmd + Shift + P` (Mac) or `Ctrl + Shift + P` (Windows)
3. Type **"Git: Clone"** and hit Enter
4. Paste the repo URL: `https://github.com/brianokarski-shopify/our-cookbook.git`
5. Choose where to save it (Desktop or Documents works great)
6. Click **Open** when prompted

### Step 2: Sign into GitHub

The first time you push changes, Cursor will ask you to sign into GitHub. Click the prompt and sign in with your Google account — Cursor handles everything automatically!

---

## 🚀 How to Add Your Recipe

### The Easy Way: Ask Cursor AI! ✨

Just open the chat and say something like:

> *"Add a new recipe for chicken tikka masala to the cookbook"*

Cursor will create the recipe file AND update the homepage for you. Then just commit and push (see Step 4 below)!

---

### The Manual Way

#### Step 1: Copy the Template

1. In the Cursor file explorer (left sidebar), right-click `recipe-template.html`
2. Click **Copy**
3. Right-click in an empty area → **Paste**
4. Rename the file using **lowercase with hyphens**: `your-recipe-name.html`

**Good names:** `grandmas-meatballs.html`, `spicy-thai-curry.html`
**Bad names:** `Grandmas Meatballs.html`, `spicy thai curry.html`

#### Step 2: Fill In Your Recipe

Open your new file and replace the placeholder text:
- Recipe title
- Your name
- Category (Breakfast, Lunch, Dinner, Dessert, etc.)
- Prep/cook times and servings
- Ingredients (one per line)
- Instructions (one step per line)
- Chef's notes (optional)

> 💡 **Tip:** You can ask Cursor AI to help fill it in! Just say: *"Fill in this recipe template for grandma's banana bread"*

#### Step 3: Add a Card to the Homepage

Open `index.html` and find the comment that says `ADD YOUR RECIPE CARD HERE`. Add this code (update with your details):

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

#### Step 4: Commit & Push to GitHub

1. Click the **Source Control** icon in the left sidebar (looks like a branch 🌿)
2. You'll see your changed files listed
3. Type a commit message: `Add grandma's meatballs recipe`
4. Click the **✓ Commit** button
5. Click **Sync Changes** (or the ↑ push arrow)

Your recipe is now live! The site updates automatically in about 1 minute.

---

## 📸 Adding Photos

Want to include a photo of your dish?

1. **Prepare your image:**
   - Use JPG or PNG format
   - Resize to ~1200px wide (keeps the site fast)
   - Name it to match your recipe: `grandmas-meatballs.jpg`

2. **Add to the images folder:**
   - Drag your photo into the `images` folder in Cursor

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

5. **Commit & push** your changes!

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

## 🌐 Previewing Your Changes

Before pushing, you can preview locally:

1. Right-click `index.html` in Cursor
2. Click **Reveal in Finder** (Mac) or **Reveal in Explorer** (Windows)
3. Double-click the file to open in your browser
4. Click around to test your links!

Or just push and check the live site — it updates in about a minute!

---

## 🆘 Troubleshooting

### "My recipe isn't showing up on the site"
- Make sure you **pushed** your changes (check Source Control for pending changes)
- Wait 1-2 minutes for GitHub Pages to update
- Check that the filename matches the link in `index.html` exactly

### "The page looks broken"
- Make sure you have `<link rel="stylesheet" href="styles.css">` in the `<head>`
- Check that you didn't accidentally delete any closing tags (`</div>`, `</section>`, etc.)
- Ask Cursor AI to check for errors!

### "My image isn't loading"
- Check the path: it should be `images/your-image.jpg`
- Make sure the filename matches exactly (including capitalization)
- Verify the image was committed and pushed

### "Git is asking for a password"
- Cursor should prompt you to sign in via browser — click the popup
- If issues persist, try: `Cmd + Shift + P` → "GitHub: Sign In"

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
