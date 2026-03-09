# roadbeat Studio Pro — Documentation

Documentation for [roadbeat Studio Pro](https://studio.roadbeat.dev) commercial plugins.

**Live site:** Published automatically via [Documentation.AI](https://documentation.ai) on push to `main`.

## Structure

```
studio-pro-docs/
├── documentation.json          # Site config, branding, navigation
├── introduction.mdx            # Landing page — plugin overview
├── installation.mdx            # Docker + manual install guides
├── licensing.mdx               # License tokens, validation, grace period
├── plugins/                    # Per-plugin documentation (20 plugins)
│   ├── workflows.mdx           # Editorial Workflows
│   ├── scheduling.mdx          # Content Scheduling
│   ├── locking.mdx             # Content Locking
│   ├── preview.mdx             # Preview API
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
│   ├── environments.mdx        # Environments
│   ├── bulk-ops.mdx            # Bulk Asset Operations
│   ├── media.mdx               # Video Processing
│   ├── whitelabel.mdx          # White-Labeling
│   └── api-explorer.mdx        # API Explorer
├── help-center.mdx             # Help center landing
├── help-center/                # FAQ + troubleshooting
│   ├── faq/
│   └── troubleshooting/
└── changelog.mdx               # Release notes
```

## Editing

All pages are `.mdx` files (Markdown + JSX components). Navigation is defined in `documentation.json`.

## API Documentation

Pro plugin API endpoints are documented in the **Studio CE** documentation site (not here), since all endpoints are part of the same OpenAPI spec served by CE at `/api/docs`. This site links to the CE API Reference where relevant.

## Related

- [Studio CE Documentation](../studio-docs/) — full CE docs including API reference
- [Studio Pro source code](../studio-pro/) (private, BSL 1.1)
