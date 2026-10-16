<p align="center">
  <a href="https://groundmail.dev">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://app.groundmail.dev/images/github/readme-logo-dark.png">
      <img alt="Groundmail" src="https://app.groundmail.dev/images/github/readme-logo-light.png" height="48">
    </picture>
  </a>
</p>

<p align="center">
  <strong>Transactional email, on solid ground.</strong><br>
  Password resets, receipts and alerts, sent from our own mail servers and our own IP space.
</p>

<p align="center">
  <a href="https://groundmail.dev">Website</a> ·
  <a href="https://docs.groundmail.dev">Docs</a> ·
  <a href="https://groundmail.dev/pricing">Pricing</a> ·
  <a href="https://app.groundmail.dev/signup">Sign up free</a>
</p>

---

### Send your first email

```bash
npm install groundmail
```

```ts
import { Groundmail } from 'groundmail'

const groundmail = new Groundmail(process.env.GROUNDMAIL_API_KEY)

await groundmail.emails.send({
  from: 'hello@mail.yourcompany.com',
  to: 'ada@example.com',
  subject: 'Reset your password',
  html: '<p>Click the link to reset it.</p>',
})
```

Or let your coding agent do it: `npx skills add Groundmail/groundmail-skills -y`, then ask it to "add Groundmail to this app".

### Libraries and tools

| | |
|---|---|
| **Node.js / TypeScript** | [`groundmail`](https://www.npmjs.com/package/groundmail) |
| **Python, Go, Ruby** | [groundmail-sdks](https://github.com/Groundmail/groundmail-sdks) |
| **PHP · Laravel · Symfony** | [groundmail-php](https://github.com/Groundmail/groundmail-php) · [groundmail-laravel](https://github.com/Groundmail/groundmail-laravel) · [groundmail-symfony-mailer](https://github.com/Groundmail/groundmail-symfony-mailer) |
| **Nodemailer** | [groundmail-nodemailer](https://github.com/Groundmail/groundmail-nodemailer) |
| **CLI** | [`groundmail-cli`](https://www.npmjs.com/package/groundmail-cli) |
| **MCP server** for Claude, ChatGPT and Cursor | [groundmail-mcp](https://github.com/Groundmail/groundmail-mcp) · hosted at `https://mcp.groundmail.dev/mcp` |
| **Agent skills** and Claude Code plugin | [groundmail-skills](https://github.com/Groundmail/groundmail-skills) |

### Why Groundmail

- **Our own infrastructure.** Our own mail servers and IP space, not a resold shared pool.
- **Transactional only.** No newsletters or cold outreach on the platform.
- **Start free.** 3,000 emails a month free; Pro is 50,000 for $20/month; dedicated IPs on Scale.
- **Switching?** Migration guides for [SendGrid](https://docs.groundmail.dev/migration/sendgrid), [Postmark](https://docs.groundmail.dev/migration/postmark) and [Amazon SES](https://docs.groundmail.dev/migration/ses).
