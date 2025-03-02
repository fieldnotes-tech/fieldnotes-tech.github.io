# FieldNotes.Tech

This repository contains the content for [FieldNotes.Tech](https://fieldnotes.tech/) powered by [BearBlog](https://github.com/samsalisbury/bearblog).

## How to Use

1. Create a new Bear note with your content
2. Export it as a TextBundle
3. Use the BearBlog CLI to deploy:
   ```
   bearblog -input /path/to/exported/notes -deploy -gh-repo samsalisbury/fieldnotes.tech
   ```

## Configuration

The site is automatically deployed to the `gh-pages` branch using GitHub Pages.

To update site configuration, create a `config.yml.textbundle` note in Bear with the following content:

```yaml
title: FieldNotes.Tech
base-url: https://fieldnotes.tech/
author: Your Name
```

## Deployment

Content is deployed when a new release is created with a `content.zip` asset.
This happens automatically when using the BearBlog CLI with the `-deploy` flag.

For more information, see the [BearBlog documentation](https://github.com/samsalisbury/bearblog).
