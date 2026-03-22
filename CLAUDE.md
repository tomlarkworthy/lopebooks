# Lopebooks

Content repository for lopecode notebooks. Served via GitHub Pages at `tomlarkworthy.github.io/lopebooks/`.

## Assets

Preview videos and images live in `assets/`. Conventions:

- **Filename**: `@author_notebook-slug.ext` (matches the notebook filename without `.html`)
- **Videos**: Always convert `.mov` to `.mp4` before committing. Use ffmpeg:
  ```
  ffmpeg -i input.mov -c:v libx264 -crf 35 -preset fast -an -movflags +faststart -vf "scale=480:-2" output.mp4
  ```
  - Scale to **480px wide** (`-vf "scale=480:-2"`)
  - Target **under 256KB** per video (`-crf 35`)
  - Strip audio (`-an`)
  - Enable fast start for streaming (`-movflags +faststart`)
- **Images**: PNG or JPEG, no size constraint but keep reasonable
- **Never commit `.mov` files** — they are 10-20x larger than compressed `.mp4`

## content.json

Gallery metadata. Managed via the gallery curator mode or direct edits. Fetched at runtime from `raw.githubusercontent.com` for instant updates.
