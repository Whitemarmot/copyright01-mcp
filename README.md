# Copyright01 MCP Server

Copyright deposit API — legally timestamp and protect code, text, websites, and creative content with a Berne Convention certificate recognized in 181 countries.

## What is Copyright01?

[Copyright01.com](https://www.copyright01.com) creates legally binding, timestamped proof of authorship under the **Berne Convention** (recognized in 181 countries). Use this MCP server to protect original code, text, websites, social media content, and GitHub repositories directly from any AI agent.

## Quick Setup

Add to your Claude Desktop, Cursor, or Windsurf configuration:

```json
{
  "mcpServers": {
    "copyright01": {
      "url": "https://www.copyright01.com/mcp",
      "headers": {
        "Authorization": "Bearer YOUR_API_KEY"
      }
    }
  }
}
```

Get your API key at [copyright01.com/profil#api-keys](https://www.copyright01.com/profil#api-keys) (free account includes 3 deposits).

## Available Tools

| Tool | Description |
|------|-------------|
| `create_deposit` | Create a timestamped copyright deposit with legal proof of authorship |
| `list_deposits` | List all deposits with optional filters by type and status |
| `get_deposit` | Get deposit details including certificate and verification URL |
| `verify_hash` | Verify a SHA-256 hash against registered deposits |
| `verify_certificate` | Verify a certificate by its code (public, no auth required) |
| `get_profile` | Check plan, credits remaining, and storage usage |

## Supported Content Types

- **Text** — Code, articles, poems, any written content (min 10 chars)
- **Website** — Screenshot + HTML archive of any URL
- **YouTube** — Videos and channels
- **Social Media** — Instagram, Facebook, X, TikTok, Pinterest, Threads
- **GitHub** — Repository ZIP archive

## How It Works

1. Create a free account at [copyright01.com](https://www.copyright01.com/register)
2. Generate an API key at [profil#api-keys](https://www.copyright01.com/profil#api-keys)
3. Add the MCP server to your AI tool
4. Ask your AI to protect your content — it will create a deposit and return a verification certificate

Each deposit generates:
- SHA-256 and SHA-512 content hashes
- A PDF certificate with QR code
- A unique verification code (format: `XXXX-XXXX-XXXX`)
- A public verification URL

## Pricing

| Plan | Credits | Details |
|------|---------|---------|
| Free | 3 | Included at signup |
| Pack 5 | 5 | One-time purchase |
| Pack 20 | 20 | One-time purchase |
| Subscription | 30/month | Monthly renewal |

Each deposit consumes 1 credit regardless of type.

## Documentation

- [Developer page](https://www.copyright01.com/developpeurs)
- [OpenAPI spec](https://www.copyright01.com/openapi.yaml)
- [llms.txt](https://www.copyright01.com/llms.txt)
- [MCP discovery](https://www.copyright01.com/.well-known/mcp.json)

## License

MIT

