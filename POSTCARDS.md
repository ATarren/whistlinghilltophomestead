# Creating and archiving postcards

Postcards are Jekyll posts in the `_posts/` folder. The newest dated postcard automatically appears in the **Today's Postcard** section on the homepage. When you add a newer one, the previous postcard remains saved and appears under **Past Postcards**. No old post needs to be moved or deleted.

## Add a postcard

1. Upload its photo into the `images/` folder.
2. Add a Markdown file in `_posts/` named with its date and a short, lowercase slug, for example `2026-12-01-first-snow.md`. Use a new date/filename each time.
3. Copy this template and replace the example values and story:

```yaml
---
layout: postcard
title: First Snow on the Homestead
date: 2026-12-01
image: /images/first-snow.jpeg
image_alt: The first snow covering the homestead garden
excerpt: A short sentence or two to preview the postcard on the homepage and in the archive.
---

Write the full postcard here. You can use Markdown for paragraphs, links, and lists.
```

The date and filename determine the order, with the most recent date displayed first. Keep the image path and filename matched to the photo you uploaded. After the site rebuilds, the new postcard will be featured on the homepage, and the previous one will appear in **Past Postcards**.
