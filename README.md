# ElvisDev - Portfolio CMS

Sanity Studio for managing portfolio project content. The frontend portfolio lives in a separate codebase.

## Tech Stack

- Sanity v6.2.0
- React 19
- TypeScript
- pnpm

## Getting Started

```bash
pnpm install
pnpm dev
```

### Build & Deploy

```bash
pnpm build
pnpm deploy
```

## Schema: Project

| Field | Type | Required | Description |
|---|---|---|---|
| title | string | yes | Project title |
| subtitle | string | no | Project subtitle |
| slug | slug | yes | URL-friendly identifier |
| status | string (radio) | yes | `unfinished` / `finished` |
| techStack | array[string] | no | Tags for technologies used |
| projectLink | url | no | Link to live project |
| previewImage | image | no | Thumbnail with alt text |
| heroImage | image | no | Hero image with alt text |
| content | array[block] | no | Rich text (Portable Text) |

## Scripts

- `pnpm dev` — Start development server
- `pnpm build` — Build for production
- `pnpm deploy` — Deploy Studio
- `pnpm deploy-graphql` — Deploy GraphQL API
