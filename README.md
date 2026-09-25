# DocsStock Blog

A [Hugo](https://gohugo.io) site. Posts are committed automatically to
`content/posts/yyyy-mm-dd-slug.md` by the DocsStock platform's GitHub
syndication channel; the date is taken from the filename and each post is
served at `https://blog.docsstock.com/slug/`.

## Cloudflare Pages

Connect this repository in the Cloudflare dashboard (Workers & Pages → Create →
Pages → Connect to Git) with:

| Setting                  | Value            |
| ------------------------ | ---------------- |
| Framework preset         | Hugo             |
| Build command            | `hugo --minify`  |
| Build output directory   | `public`         |
| Production branch        | `main`           |

The Hugo version is pinned in `.tool-versions`. Add a custom domain of
`blog.docsstock.com` under the project's *Custom domains* tab.

## Local preview

```sh
hugo server -D
```
