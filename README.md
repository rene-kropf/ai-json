# ai-json
A simple structured data format for helping AI understand your website

## What it is

`ai.json` is a plain structured file you place at the root of your website. It tells AI assistants, LLMs, and crawlers exactly what your business does, what you offer, and how to reach you — in clean machine-readable form.

No algorithm to game. No keyword counts. No SEO theater. Just honest information about your business, published in a format AI can actually use.

## Why it exists

Search engines trained a generation of website owners to optimize their content for crawlers — for free, on someone else's terms, with rules that changed without notice. AI is the new layer on top of the web. The question is whether we repeat that mistake or do something cleaner this time.

`ai.json` is the cleaner version. You publish what you want AI to know. It lives at a known URL. You control it. Done.

## How it works

1. Fill in the template below with your business information
2. Save it as `ai.json`
3. Place it at the root of your website: `yourdomain.com/ai.json`

That's it. No registration. No submission. No dependency.

## The minimal template

Copy this, fill in your answers, delete anything that doesn't apply.

```json
{
  "schema": "ai-site-info/1.0",
  "generated": "YYYY-MM-DD",
  "site": {
    "name": "Your Business Name",
    "url": "https://yourdomain.com",
    "tagline": "One sentence that captures what you do",
    "description": "Two or three sentences. What you do, who you do it for, what makes you different.",
    "contact": "https://yourdomain.com/contact"
  },
  "services": [
    {
      "name": "Service or product name",
      "description": "What it is and who it helps.",
      "price": "Optional — exact price or range"
    }
  ],
  "faq": [
    {
      "q": "The question your customers ask most",
      "a": "Your honest answer"
    },
    {
      "q": "Second most common question",
      "a": "Your honest answer"
    }
  ]
}
```

## Optional fields

Add these if they apply to your business:

```json
{
  "location": {
    "city": "Your City",
    "region": "State or Province",
    "country": "US",
    "serves": "Description of service area if relevant"
  },
  "hours": "Mon-Fri 9am-5pm CT",
  "founded": "2020",
  "philosophy": "Optional — your approach or values in plain language"
}
```

## Principles

**Keep it honest.** This file is read by AI, not gamed by it. Accurate information serves you better than optimized information.

**Keep it simple.** Ten good fields beat fifty empty ones. Start minimal and add only what's genuinely useful.

**Keep it current.** Stale data is worse than no data. Update it when your business changes.

**You own it.** No platform controls this. No algorithm penalizes you. It lives on your server, under your domain, on your terms.

## The full example

A complete real-world example is at [emmausdev.com/ai.json](https://emmausdev.com/ai.json)

## Background

This convention was proposed by Rene Kropf at [Emmaus Development](https://emmausdev.com) as a simpler alternative to the growing complexity of AI visibility optimization. The thinking behind it is covered on [Clarity Signal](https://www.youtube.com/channel/UCMYg2c98FEM8ijlVbyMijQA).

## License

Public domain. Use it, fork it, build on it.
