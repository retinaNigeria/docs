# TruHuddle documentation

Customer documentation for [TruHuddle](https://truhuddle.com), powered by Mintlify and maintained in [retinaNigeria/docs](https://github.com/retinaNigeria/docs). The application source stays in its own repository.

## Preview locally

Requires Node.js 20.17.0 or newer. Install the CLI once:

```bash
npm i -g mint
```

From this repository:

```bash
mint dev --port 3002
```

Port 3002 avoids the application’s local port 3000. On a Mac where npm’s system global directory is not writable, use a user-owned installation instead of sudo:

```bash
npm install --global --prefix "$HOME/.local" mint
"$HOME/.local/bin/mint" dev --port 3002
```

## Update through Git

Edit the relevant .mdx page or docs.json, then check the documentation:

```bash
mint validate
mint broken-links
git add .
git commit -m "Update TruHuddle documentation"
git push origin main
```

In Mintlify, connect the retinaNigeria/docs repository, branch main, and repository root. Once the Mintlify GitHub App is authorized for this repository, pushes to main trigger documentation deployments. This does not require rebuilding or restarting the PM2 application.

## Branding and SEO

docs.json sets the brand blue, unmodified hosted logo, local favicon, League Spartan fonts, light/dark appearance, navigation, social previews and publisher metadata. Each page has its own title, description and keywords. Mintlify generates page canonicals, sitemap and robots metadata from the deployed site URL. Do not set one canonical URL for every page.

The intended custom hostname is docs.truhuddle.com. Add it under Mintlify’s domain settings and use the DNS record Mintlify supplies. Its dashboard connection, GitHub authorization and DNS are external setup steps; this commit does not configure them.

## Content

- [index](index.mdx)
- [quickstart](quickstart.mdx)
- [guides/plans-and-credits](guides/plans-and-credits.mdx)
- [guides/writing-and-publishing](guides/writing-and-publishing.mdx)
- [guides/blog-settings](guides/blog-settings.mdx)
- [guides/ai-and-voice](guides/ai-and-voice.mdx)
- [guides/authors-and-analytics](guides/authors-and-analytics.mdx)
- [domains/connect-a-domain](domains/connect-a-domain.mdx)
- [domains/cloudflare-worker](domains/cloudflare-worker.mdx)
- [domains/search-and-seo](domains/search-and-seo.mdx)
- [api-reference/authentication](api-reference/authentication.mdx)
- [api-reference/articles](api-reference/articles.mdx)
- [api-reference/categories-and-authors](api-reference/categories-and-authors.mdx)
- [api-reference/errors-and-pagination](api-reference/errors-and-pagination.mdx)
- [help/troubleshooting](help/troubleshooting.mdx)

Keep account secrets and private operational documentation out of this repository. Follow AGENTS.md before editing.
