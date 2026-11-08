# roadbeat Studio Pro — Documentation

Documentation for [roadbeat Studio Pro](https://studio.roadbeat.dev) commercial plugins.

**Live site:** Published automatically via [Documentation.AI](https://documentation.ai) on push to `main`.

## Structure

```
studio-pro-docs/
├── documentation.json          # Site config, branding, navigation
├── introduction.mdx            # Landing page — plugin overview
├── installation.mdx            # Docker + manual install guides, plugin secrets
├── licensing.mdx               # License tokens, validation, grace period
├── languages.mdx               # 24 EU languages, plural forms, translated errors
├── accessibility.mdx           # WCAG 2.1 AA design rules and how they are tested
├── plugins/                    # Per-plugin documentation
│   ├── ai.mdx                  # AI Provider Gateway
│   ├── ai-recipes.mdx          #   Provider setup recipes
│   ├── ai-governance.mdx       #   AI privacy & governance
│   ├── integrations*.mdx       # Integration Hub (overview, governance, connectors, recipes)
│   ├── workflows.mdx           # Editorial Workflows
│   ├── tasks.mdx               #   Tasks & task board
│   ├── activity-feed.mdx       #   Team activity feed
│   ├── scheduling.mdx          # Content Scheduling
│   ├── locking.mdx             # Content Locking
│   ├── preview.mdx             # Preview API
│   ├── saved-views.mdx         # Saved Views
│   ├── import.mdx              # Content Import
│   ├── export.mdx              # Content Export
│   ├── versioning.mdx          # Version Comparison
│   ├── layouts.mdx             # Custom Layouts
│   ├── advanced-roles.mdx      # Advanced Roles & Permissions
│   ├── sso.mdx                 # SSO Integration
│   ├── audit.mdx               # Audit Logging
│   ├── graphql.mdx             # GraphQL API
│   ├── realtime.mdx            # WebSockets & Real-time
│   ├── webhooks.mdx            # Advanced Webhooks
│   ├── notifications.mdx       # Notifications
│   ├── activitypub.mdx         # ActivityPub Federation
│   ├── environments.mdx        # Environments
│   ├── bulk-ops.mdx            # Bulk Asset Operations
│   ├── media.mdx               # Video Processing
│   ├── whitelabel.mdx          # White-Labeling
│   └── api-explorer.mdx        # API Explorer
├── help-center.mdx             # Help center landing
├── help-center/
│   ├── faq/                    # General + plugin setup FAQs
│   └── troubleshooting/        # Common issues, API error codes
└── changelog.mdx               # Release notes
```

## Editing

All pages are `.mdx` files (Markdown + JSX components). Navigation is defined in `documentation.json`.

## API Documentation

Pro plugin API endpoints are documented in the **Studio CE** documentation site (not here), since all endpoints are part of the same OpenAPI spec served by CE at `/api/docs`. The Pro areas are `studio-docs/api-reference/08-pro-*.json` to `14-pro-*.json`, generated with `pnpm docs:openapi` in `studio` (with the Pro plugins built and `PLUGINS_DIR` pointing at them). This site links to the CE API Reference where relevant.

## Related

- [Studio CE Documentation](../studio-docs/) — full CE docs including API reference
- [Studio Pro source code](../studio-pro/) (private, BSL 1.1)
