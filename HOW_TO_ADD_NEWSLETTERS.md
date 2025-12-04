# How to Add Newsletters

## Basic Structure

Edit `newsletters/newsletters.json` and add a new entry:

```json
{
  "id": "2025-12",
  "title": "December 2025 - Holiday Season",
  "date": "2025-12-20",
  "month": "December",
  "year": 2025,
  "featuredImage": "images/december-2025.jpg",
  "content": "<p>Your newsletter content here...</p>"
}
```

## Adding Images

### Featured Image (Optional)
Add a `featuredImage` field with the path to your image:
```json
"featuredImage": "images/thanksgiving-2025.jpg"
```

### Images in Content
You can add images directly in the HTML content:
```html
<img src="images/family-photo.jpg" alt="Family photo" />
<p class="image-caption">Our family at Thanksgiving</p>
```

**Image Paths:**
- Store images in an `images/` folder in your repository
- Use relative paths like `images/photo.jpg`
- For GitHub Pages, paths are relative to the root

## HTML Content Styling

You can use these HTML elements in your `content` field:

### Text Formatting
- `<p>` - Paragraphs
- `<h2>`, `<h3>` - Headings
- `<strong>` or `<b>` - Bold text
- `<em>` or `<i>` - Italic text
- `<a href="url">` - Links

### Lists
```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
</ul>

<ol>
  <li>First</li>
  <li>Second</li>
</ol>
```

### Blockquotes
```html
<blockquote>
  "A memorable quote from the month"
</blockquote>
```

### Images with Captions
```html
<img src="images/photo.jpg" alt="Description" />
<p class="image-caption">Caption text here</p>
```

## Example Newsletter

```json
{
  "id": "2025-11",
  "title": "November 2025",
  "date": "2025-11-30",
  "month": "November",
  "year": 2025,
  "featuredImage": "images/november-featured.jpg",
  "content": "<p>This November was wonderful!</p><h2>Thanksgiving</h2><p>We had a great time at Carmen's.</p><img src=\"images/thanksgiving.jpg\" alt=\"Thanksgiving dinner\" /><p class=\"image-caption\">Our Thanksgiving feast</p><h2>Birthdays</h2><p>We celebrated Marion and Jacob's birthdays!</p><ul><li>Marion's birthday party</li><li>Jacob's celebration</li></ul>"
}
```

## Buttondown Integration

The signup form on the homepage uses Buttondown. Make sure to:
1. Update the form action URL with your Buttondown username
2. Update the `onsubmit` popup URL with your username
3. Both are currently set to `ryan-notes` - change if needed

