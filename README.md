# 👋 Hi, I'm Kanawut

A senior full-stack developer from Thailand 🇹🇭, and the creator and maintainer of
**[Easy CMS](https://easycms.dev)**, an open-source project I build on nights and weekends.

I like TypeScript all the way down, developer tools that stay out of the way, and software that
works as well in Thai as in English. I maintain open source the way I'd want to depend on it:
tested on every platform, upgrades that don't break, and docs that answer the question.

---

### 🌟 Easy CMS

**The code-first CMS and app backend for Nuxt and Next.js.**
It runs inside your app: the content model is TypeScript in your repo, the admin and API come
with it, and there is no extra server to run.

[![npm](https://img.shields.io/npm/v/@easy-cms/core?label=npm&color=2f6f5e)](https://www.npmjs.com/package/@easy-cms/core)
[![Downloads](https://img.shields.io/npm/dm/@easy-cms/core?label=downloads&color=2f6f5e)](https://www.npmjs.com/package/@easy-cms/core)
[![CI](https://github.com/maritonx/easy-cms/actions/workflows/ci.yml/badge.svg)](https://github.com/maritonx/easy-cms/actions/workflows/ci.yml)
[![Docs](https://img.shields.io/badge/docs-EN%20%7C%20TH-2f6f5e)](https://easycms.dev/docs)
[![License: MIT](https://img.shields.io/badge/license-MIT-555)](https://github.com/maritonx/easy-cms/blob/main/LICENSE)

**C**ode-first · **M**any systems, one app · **S**ecure

- 🛠️ **Code-first:** collections, fields, access rules and hooks in TypeScript, with a typed
  Local API and REST at `/api/cms`. SQLite or Postgres, migrations reviewed like code.
- 🧩 **Many systems, one app:** an admin editors like (drafts, live preview, media, calendar, in
  English and Thai), site members, jobs, events and realtime built in, and plugins for a shop,
  forms, SEO, several sites in one CMS and AI assistants (MCP).
- 🔒 **Secure:** secure defaults, self-reviewed against OWASP ASVS level 1, and an audit log signed
  against tampering.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/maritonx/easy-cms/main/website/public/screenshots/dashboard-en-dark.webp">
  <img src="https://raw.githubusercontent.com/maritonx/easy-cms/main/website/public/screenshots/dashboard-en-light.webp" alt="The Easy CMS admin dashboard: content at a glance, recently edited pages and drafts to review">
</picture>

#### Quick start

```bash
npm create easy-cms@latest     # in a Nuxt 4 or Next.js 15+ project, or an empty folder
npm run dev                    # then open /admin
```

```ts
// easy-cms.config.ts
export default defineConfig({
  secret: process.env.EASY_CMS_SECRET!,
  db: sqlite({ url: 'file:./cms.db' }),
  collections: [
    { slug: 'posts', drafts: true, fields: [{ name: 'title', type: 'text', required: true }] },
  ],
})
```

<details>
<summary><b>Official plugins</b></summary>

| Plugin | What it adds |
|---|---|
| Shop (experimental) | Products and variants, carts, checkout with Stripe or bank transfer, orders and stock |
| Forms | Forms built in the admin, submissions, email notifications, spam protection |
| SEO | Meta fields, sitemap, robots.txt, structured data, `llms.txt` |
| Multi-tenant | Several sites or clients in one CMS, each with its own content, members and roles |
| Redirects | Redirects from the admin, automatic ones when a page moves |
| Nested pages | Parents, full paths, breadcrumbs and a tree in the admin |
| AI | Claude, GPT, Gemini or an OpenAI-compatible server for the admin's AI features |
| MCP (experimental) | A Model Context Protocol server, so AI assistants can read and draft content |
| GraphQL (experimental) | Queries and mutations for every collection, with your access rules |
| Notify | Telegram messages when a form is sent, an order comes in or something fails |

</details>

<details>
<summary><b>How it's built</b></summary>

- Tests on Linux, macOS and Windows, on SQLite, Postgres and PGlite, for every pull request
- Upgrades tested in CI: databases made by older releases migrate to the current one
- A nightly load test: 200 editors on 1 million posts, compared with the last good night
- Self-reviewed against OWASP ASVS level 1, with CodeQL on every change
- Every design decision written down as an [architecture decision record](https://github.com/maritonx/easy-cms/tree/main/docs/adr)
- Full docs in English and Thai, from the same repository as the code

</details>

#### Now working on

Keeping 1.x stable, and the [roadmap](https://easycms.dev/roadmap): from managing content to a
backend that people and AI agents work in under the same rules.

[Website](https://easycms.dev) · [Docs](https://easycms.dev/docs) ·
[เอกสารภาษาไทย](https://easycms.dev/th/docs) · [GitHub](https://github.com/maritonx/easy-cms) ·
[Sponsor ❤](https://github.com/sponsors/maritonx)

---

### 🇹🇭 ภาษาไทย

สวัสดีครับ ผม Kanawut นักพัฒนา full-stack จากประเทศไทย ผู้สร้างและดูแล
**[Easy CMS](https://easycms.dev/th/docs)**: CMS และ app backend แบบ code-first ที่อยู่ในแอป Nuxt หรือ
Next.js ของคุณเลย ไม่ต้องมี server แยก มีทั้งเนื้อหา สมาชิก ร้านค้า และฟอร์ม และรองรับภาษาไทยตั้งแต่หน้า
admin ไปจนถึงเอกสาร ถ้า Easy CMS ช่วยงานคุณได้ ฝาก ⭐ หรือ[สนับสนุน](https://github.com/sponsors/maritonx)ได้ครับ

---

### ⚙️ Tech stack

- **Languages & frameworks:** TypeScript | JavaScript | PHP | Node.js | Next.js | Nuxt | React | Laravel | AdonisJS | NestJS
- **Databases:** PostgreSQL | SQLite | MongoDB | Elasticsearch | Redis | MariaDB
- **DevOps:** Git | GitHub Actions | Docker | CI/CD

---

### 📫 Connect

- 🌐 **Easy CMS:** [easycms.dev](https://easycms.dev)
- ❤️ **Sponsor:** [github.com/sponsors/maritonx](https://github.com/sponsors/maritonx)
- 📧 **Email:** [scton54@gmail.com](mailto:scton54@gmail.com)
- 💼 **LinkedIn:** [linkedin.com/in/kanawut-korsang-425a45440](https://linkedin.com/in/kanawut-korsang-425a45440)
