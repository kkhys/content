# Content

This directory manages the content for [kkhys.me](https://kkhys.me).

## Directory Structure

```
content/
├── blog/           # Blog posts (MDX)
├── bucket-list/    # Bucket list (YAML)
└── LICENSE.md      # License
```

## Blog Posts

Blog posts are organized in the `blog/YYYY-MM-DD/index.mdx` format. Images are co-located in the same directory.

```
blog/
└── 2024-01-20/
    ├── index.mdx
    ├── 01.png
    └── 02.png
```

### Frontmatter

| Field                  | Required | Description                              |
| ---------------------- | -------- | ---------------------------------------- |
| `title`                | Yes      | Post title                               |
| `description`          | Yes      | Post description                         |
| `emoji`                | Yes      | Emoji representing the post              |
| `category`             | Yes      | Category (Tech / Life / Object / DIY)    |
| `publishedAt`          | Yes      | Publication date                         |
| `tags`                 | No       | Tags (scoped per category)               |
| `status`               | No       | draft / published (default: published)   |
| `updatedAt`            | No       | Last updated date                        |
| `sourceUrl`            | No       | Source code URL                          |
| `editUrl`              | No       | Edit page URL                            |
| `revisionHistoryUrl`   | No       | Revision history URL                     |

### Categories and Tags

There are 4 categories, and tags are hierarchically scoped per category. Invalid category-tag combinations will cause build failures.

## Bucket List

Managed in `bucket-list/data.yaml`.

## License

Content is licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/). See [LICENSE.md](./LICENSE.md) for details.
