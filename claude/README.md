# Applink for Claude

Applink hosts a team's internal apps, integrations and databases. This plugin lets Claude build and publish those apps with you: dashboards and tools that read your organization's integrations, and apps that keep their own data in an Applink database.

## What it adds

- **The Applink connector**, at `https://api.tryapplink.com/mcp`: tools to read the integrations open to Claude, query BigQuery, work with databases, and create, change and publish hosted apps.
- **The "Build Applink apps" skill**: how Applink apps work, and the steps to build, publish and share one.

## Before you start

You need an Applink account in an organization where an Owner or Admin has turned Claude on, in **Settings**, then **Claude**, and a role that may create apps. The first time Claude uses the connector, you sign in to Applink and choose the organization.

## What it sends, and where

Claude calls the connector at `https://api.tryapplink.com/mcp` over HTTPS, signed in as you with OAuth. Each call carries what Claude gives that tool, such as an integration's name, a query, rows or an app's files. Applink acts with your own access and records each change as yours, marked as from Claude. The plugin runs nothing on your computer and sends nothing anywhere else.

Applink's privacy policy: https://tryapplink.com/privacy

## Documentation

https://tryapplink.com/docs/claude

## License

MIT. See [LICENSE](LICENSE).
